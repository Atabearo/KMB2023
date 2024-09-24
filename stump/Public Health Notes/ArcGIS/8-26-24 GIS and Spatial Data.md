Types of data: observations with explicit location
- buildings, events (crime), weather, roads, gas lines
Formats
- vector (object/discrete)
- raster (continuous/field --  saved as an array of cells)
	- suited for cont. data (ex: satellite imagery, aerial photos, temperature)

Vector data (features)
- Points
- Lines
- Polygons (boundaries)

**Attributes** (non-spatial data): description about a space
- demographic info (e.g. population size, household income, birth/death rates)
- Attribute info (e.g. year built, number of lanes)
	Stored in a table, often linked to spatial data

**Metadata**: data describing the data

###### Target Table and Source Table
**Target**: the OG table that has the spatial data that you are actively working on
**Source**: containing the additional attribute data linked to incorporate
- can be joined with a common field (such as FIPS)
Merging/Joining Data
- Target-to-source
	- One-to-one
	- Many-to-one (e.g. many census blocks to one tract)
	- one-to-many (e.g. one water source serves many homes)
	- many-to-many 

