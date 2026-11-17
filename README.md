# CMIP7_mirror_ESGF
Project to establish a download stream for CMIP7 data to the Norwegian national computing infrastructure (nird)

At this point this is just a potential starting point.

## Tech used
- Python
- downloads are done via the package `intake-esgf`
- data localtions are split between a central mirror and user specific cache locations
- Central mirror location that can only be written by a selected group of people
- users need a local cache from where an ingestion script will copy the data to the central mirror location above (to avoid file locking problems)
- users need to tell an admin the location of their local cache directory and make sure it's acessible
