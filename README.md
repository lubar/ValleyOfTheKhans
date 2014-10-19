ValleyOfTheKhans
================

Crowdsourcing data gathered as part of an expedition to Mongolia in search of the legend of Genghis Khan.

This data supports the PLOS-One publication by Lin, Lanckriet, Huynh and Barrington [2014] titled "Crowdsourcing the Unknown". The paper describes a crowdsourcing initiative, http://exploration.nationalgeographic.com/, where more than 10,000 online explorers contributed to a massive, online, distributed search of thousands of satellite images. Using a simple web interface, the public "crowd" marked any clues in the images that could help explorers in a remote part of Mongolia identify locations of archaelogical significance, including graves, tombs, deer stones and khirigsuurs.

3 data files are published here, each in CSV format:

1) **Master** - a description of the 32 DigitalGlobe satellite images that were used in this work.
- id
- upper_left_E
- upper_left_N
- lower_left_E
- lower_left_N
- upper_right_E
- upper_right_N
- lower_right_E
- lower_right_N
- width
- height
- url

2) **Tile** - Master images were chopped into 84,183 small tiles for individuals to view on the crowdsourcing site. 
- id
- upper_left_E
- upper_left_N
- lower_left_E
- lower_left_N
- upper_right_E
- upper_right_N
- lower_right_E
- lower_right_N
- width
- height
- url
- master_id
- zoom
- bad_tile

3) **View** - 974,116 records of which users viewed which tiles and when
- id
- timestamp
- user_id
- tile_id

4) **Annotation** - 2,617,633 locations where users identified a feature of interest in the Tiles
- id
- timestamp
- tile_id
- user_id
- E
- N
- type_id
- comment

5) **AnnotationType** - users searched for 5 features: roads, rivers, modern buildings, archaeological sties and "other"
- id
- name
- color
- simple
