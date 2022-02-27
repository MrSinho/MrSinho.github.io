# Gaia Archive Tools C Definitions

Types and structures:
* [Types and structures](#types-and-structures)
* [gaia_real](#gaia_real)
* [GaiaCelestialBodyFlags](#gaiacelestialbodyflags)
* [GaiaCelestialBody](#gaiacelestialbody)

Functions:
* [GaiaUniverseModelGetID](#gaiauniversemodelgetid)
* [GaiaReadBinaryFile](#gaiareadbinaryfile)
* [GaiaReadWeb](#gaiareadweb)


# Types and structures


## gaia_real
```c
#ifndef GAIA_DOUBLE_PRECISION
    typedef float gaia_real;
#else
    typedef double gaia_real;
#endif//GAIA_DOUBLE_PRECISION
```
### ***Description***
By default a type definition of float, unless GAIA_DOUBLE_PRECISION is defined.
---


## GaiaCelestialBodyFlags
```c
typedef enum GaiaCelestialBodyFlags {
    GAIA_SOURCE_EXTENDED_ID = 1 << 0,
    GAIA_SOURCE_ID = 1 << 1,
    GAIA_SOLUTION_ID = 1 << 2,
    GAIA_RA = 1 << 3,
    GAIA_DEC = 1 << 4,
    GAIA_BARYCENTRIC_DISTANCE = 1 << 5,
    GAIA_PMRA = 1 << 6,
    GAIA_PMDEC = 1 << 7,
    GAIA_RADIAL_VELOCITY = 1 << 8,
    GAIA_MAG_G = 1 << 9,
    GAIA_MAG_BP = 1 << 10,
    GAIA_MAG_RP = 1 << 11,
    GAIA_MAG_RVS = 1 << 12,
    GAIA_V_I = 1 << 13,
    GAIA_MEAN_ABSOLUTE_V = 1 << 14,
    GAIA_AG = 1 << 15,
    GAIA_AV = 1 << 16,
    GAIA_TEFF = 1 << 17,
    GAIA_SPECTRAL_TYPE = 1 << 18,
    GAIA_LOGG = 1 << 19,
    GAIA_FEH = 1 << 20,
    GAIA_ALPHAFE = 1 << 21,
    GAIA_MBOL = 1 << 22,
    GAIA_AGE = 1 << 23,
    GAIA_MASS = 1 << 24,
    GAIA_RADIUS = 1 << 25,
    GAIA_VSINI = 1 << 26,
    GAIA_POPULATION = 1 << 27,
    GAIA_HAS_PHOTOCENTER_MOTION = 1 << 28,
    GAIA_NC = 1 << 29,
    GAIA_NT = 1 << 30,
    GAIA_SEMIMAJOR_AXIS = 1 << 31,
    GAIA_ECCENTRICITY = 1 << 32,
    GAIA_INCLINATION = 1 << 33,
    GAIA_LONGITUDE_ASCENDING_NODE = 1 << 34,
    GAIA_ORBIT_PERIOD = 1 << 35,
    GAIA_PERIASTRON_DATE = 1 << 36,
    GAIA_PERIASTRON_ARGUMENT = 1 << 37,
    GAIA_VARIABILITY_AMPLITUDE = 1 << 38,
    GAIA_VARIABILITY_PERIOD = 1 << 39,
    GAIA_VARIABILITY_PHASE = 1 << 40,
    GAIA_FULL_BODY = UINT64_MAX
}GaiaCelestialBodyFlags;
```
### ***Description***
Enum useful when managing the source files.
---

## gaiaCelestialBody
```c
typedef struct GaiaCelestialBody {
    char        source_extended_id[20];
    uint64_t    source_id;
    uint64_t    solution_id;
    gaia_real   ra;
    gaia_real   dec;
    float       barycentric_distance;
    float       pmra;
    float       pmdec;
    float       radial_velocity;
    float       mag_g;
    float       mag_bp;
    float       mag_rp;
    float       mag_rvs;
    float       v_i;
    float       mean_absolute_v;
    float       ag;
    float       av;
    float       teff;
    float       logg;
    float       feh;
    float       alphafe;
    float       mbol;
    float       age;
    float       mass;
    float       radius;
    float       vsini;
    uint8_t     population;
    uint8_t     has_photocenter_motion;
    uint32_t    nc;
    uint32_t    nt;
    float       semimajor_axis;
    float       eccentricity;
    float       inclination;
    float       longitude_ascending_node;
    float       orbit_period;
    float       periastron_date;
    float       periastron_argument;
    float       variability_amplitude;
    float       variability_period;
    float       variability_phase;
} GaiaCelestialBody;
```
### ***Description***
A reference structure that used in practice.
---


# Functions


## gaiaUniverseModelGetId
```c
void gaiaUniverseModelGetId(const uint32_t id, char* s_dst);
```
### ***Description***
Converts an integer to the string version of the GEDR3 Universe Model file id.

### ***Parameters***
 * **`id`**: integer referred the GEDR3 Universe Model file at [`Index of Gaia`](http://cdn.gea.esac.esa.int/Gaia/gedr3/simulation/gaia_universe_model/);
 * **`s_dst`**: pointer to a valid array of 5 bytes;

### ***Usage example***
```c
char src_id[5];
gaiaUniverseModelGetId(25, src_id); //src_id is equal to "0025"
// "0025" is the id of GaiaUniverseModel_0025.bin, that corresponds to http://cdn.gea.esac.esa.int/Gaia/gedr3/simulation/gaia_universe_model/GaiaUniverseModel_0025.csv.gz
```
---


## gaiaReadBinaryFile
```c
void gaiaReadBinaryFile(const char* src_path, const GaiaCelestialBodyFlags flags, const uint32_t offset, const uint32_t size, uint32_t* p_dst_size, void** pp_dst);
```
### ***Description***
Reads and extracts the queried values from a source file.

### ***Parameters***
 * **`src_path`**: absolute or relative path to the source file;
 * [**`flags`**](#gaiacelestialbodyflags): used to sort the data to copy to the destination `*pp_dst`;
 * **`offset`**: offset of the source file;
 * **`size`**: number of bytes to read (entire file if set to `0`);
 * **`p_dst_size`**: pointer to the size of `*pp_dst`;
 * **`pp_dst`**: pointer to a valid destination pointer (no memory allocation is required).

### ***Usage example***
```c
const char* src_path = "../gaia_bin/GaiaUniverseModel_0000.bin"; 
uint32_t bytes_read = 0;
float* values;

gaiaReadBinaryFile(src_path, GAIA_RA | GAIA_DEC, 0, 0, &bytes_read, &values); //if size is set to 0, the entire file will be read. 

gaiaFree(values);
```
---


## gaiaReadWeb
```c
void gaiaReadWeb(const char* src_id, const GaiaCelestialBodyFlags flags, const uint32_t offset, const uint32_t size, uint32_t* p_dst_size, void** pp_dst);
```
### ***Description***
Downloads using a `system` command, reads and extracts the queried values from a source file.

### ***Parameters***
 * **`src_id`**: string equal to a Gaia Universe Model id;
 * [**`flags`**](#gaiacelestialbodyflags): used to sort the data to copy to the destination `*pp_dst`;
 * **`offset`**: offset of the source file;
 * **`size`**: number of bytes to read (entire file if set to `0`);
 * **`p_dst_size`**: pointer to the size of `*pp_dst`;
 * **`pp_dst`**: pointer to a valid destination pointer (no memory allocation is required).

### ***Usage example***
```c
uint32_t read_data = 0;
	
char src_id[5];
gaiaUniverseModelGetId(25, src_id); //"0025"

float* values;
gaiaReadWeb(src_id, GAIA_RA | GAIA_DEC, 0, 16, &read_data, &values); //if size is set to 0, the entire file will be read. 

gaiaFree(values);
```
---