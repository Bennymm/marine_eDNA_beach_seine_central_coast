Overview:
We assessed fish biodiversity, abundance and length distributions across habitat gradients on the 
BC Central Coast from 2014-2018. Beach seines were used to sample fish at 71 sites between rivers 
Inlet and the McMullins Islands. 16 sites were sampled annually in mid-summer. 6 sites were sampled 
monthly or bimonthly from May-September and opportunistically between October and April. 49 sites 
were sampled in the summer months of 2014 and 2015.
This dataset consists of several CSV files that contain spatial and habitat data, species abundance, 
species length, environmental data and seine set dimensions. All files are linked by common fields 
(e.g. site; date; replicate; species). There is also a methods protocol ("hakaiBS_protocol")

The following gives an overview of the data and their file names. 

Protocols: This word document describes field methods for the collection of the following data.
	Location: protocol.pdf	

Data Dictionary: Further descriptions of the variables are provided in dictionary CSV file.
	Location: datadictionary.csv

Spatial data: These files contain the locations of all sites surveyed. Coordinate system is 
Latitude/Longitude NAD83. Sites are represented as points collected using a handheld GPS unit 
(Garmin 62s). These data are included in the Habitat CSV file. 
       Location: habitat.csv

Habitat data: These data describe the abiotic and biotic habitat characteristics of each site. These 
include site aspect (degrees), intertidal and subtidal slope (degrees), freshwater input (y/n), 
beach/habitat length (meters along shore), substrate composition and vegetation composition.
Substrate Composition: Primary and secondary intertidal and subtidal substrates are defined by 
composition (mud, sand, shell hash, gravel, cobble or bolder), and their respective area coverage 
(percentage).Vegetation Composition: Primary and secondary intertidal and subtidal vegetation are 
defined by species or higher categories (see supplemental) and their respective area coverage 
(percentage). Note: missing data is indicated by "n/a" and an absence is incicated by "none".
       Location: habitat.csv

Species abundance data: These data are all species (or higher classification) and their abundance 
(count) by replicate, site and date. Note: A placehoder "-" was used for surveys where no fish were caught.
       Location: speciesabundance.csv

Species length data: These data are fork length measurements of a subsample (~20) of all species 
(or higher classification) sampled by replicate, site and date. 
		Location: specieslength.csv

Environmental data: These data are climatic variables [Temperature (Celsius), salinity (parts per 
thousand), and (pH)] collected at site relative distances from shore (depth = 0.5m, centre of seine, 
extent of seine and at 100m from shore). These locations are defined categorically (A, B, C and D, 
respectively). Observations were made along depth profiles taken at each location (A: surface, B: surface 
and 1m, C: surface, 1m and 3m. D: surface, 1m, 5m, and 10m.
		Location: environmental.csv

Seine set dimensions: These data describe the spatial dimensions of each seine set. Length and width 
(meters) of each seine set approximate the area covered by the seine. A depth at the extent of the seine 
set is also given.
		Location: netdimensions.csv

Sediment characteristics data: These data describe the size fractions of sediment cores taken at each site.
		Location: sediment.csv

Bycatch data: These data describe the organisms caught in the seine other than fish. Note: A placehoder "-" was used for surveys where there was no bycatch.
		Location: bycatch.csv

Species identification: Species are described by their field code, common name, genus and species or higher 
level of classification. Morphologically similar species were occasionally agglomerated to form an informal grouping. These groups are described by a list of species that the grouping contains.
		Location: fishcodes.csv, bycatchcodes.csv and vegetationcodes.csv

Change log: These data will use version controlling to track changes or additions to this data package.
		Location: changelog.txt

















