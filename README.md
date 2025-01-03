# Extended Vehicle Energy Dataset (eVED)

This repository publishes an extended version of the Vehicle Energy Dataset ([VED](https://github.com/gsoh/VED)), which is a large-scale dataset for vehicle energy consumption analysis. Compared with its original version, the extended VED (eVED) dataset is enhanced with accurate vehicle trip GPS coordinates, serving as a reliable basis to associate the VED trip records with external information e.g., road speed limit and intersections, from accessible map services to accumulate attributes that is relevant and essential in analyzing vehicle energy consumption. In particularly, we calibrate all the GPS trace records in the original VED dataset, upon which we associated the VED data with new attributes extracted from the Quantum Geographic Information System (QGIS), the Overpass API, the Open Street Map API, and Google Maps API. The associated attributes include 12,609,170 records of road elevation, 12,203,044 of speed limit, 12,281,719 of speed limit with direction (in case the road is bi-directional), 584,551 of intersections, 429,638 of bus stop, 312,196 of crossings, 195,856 of traffic signals, 29,397 of stop signs, 5,848 of turning loops, 4,053 of railway crossings (level crossing), 3,554 of turning circles, and 2,938 of motorway junctions. With the accurate GPS coordinates and enriched features of the vehicle trip record, the obtained eVED dataset can provide a precise and abundant medium to feed a learning engine, especially a deep learning engine that is more demanding on data sufficiency and richness. Moreover, our software work that extracts and associates vehicle trip trajectories with mentioned attributes can be reused as a toolkit to generate further vehicle trip datasets for specific user cases, with more attributes opening avenues to deep insights into vehicle behaviors and traffic dynamics analyses. We anticipate that the eVED dataset and our data enrichment software can serve both the academic and industrial automotive section as apparatus in developing future technologies.


# Files

Before digging into the dataset, we recommend that users look into the raw [VED](https://github.com/gsoh/VED) dataset to gain the view of when, where, and how the data is recorded, and how the data is structured in the format of csv files. We use the same structure of data in csv files in our extended version.

# Access to the data

Due to the quota limit of github, we store the eVED dataset along with code which is used to generate the eVED data on Bitbucket which is accessible to download via: git clone https://Datarepo@bitbucket.org/datarepo/eved-dataset.git

You can view the data and code via the [link](https://bitbucket.org/datarepo/eved-dataset/src/main/).
