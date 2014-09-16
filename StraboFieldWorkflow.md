# Strabos: an environment for structural geology data acquisition, storage, sharing and access #
## Field data work flow: ##
•	set up field project in office-- upload base maps, shape files existing points, get stuff in correct projections (list of supported projections), put in  basic metadata (who, what, why, access control).  
•	Allow shape files in view  
•	Push configuration to Strabo mobile spot editor (as opposed to strabo desktop or strabo database)  
•	basic map view allows display of multiple layers, using any georeferenced image (all have to be in same projection; have to figure out how to have GPS 
•	Connects to GPS to display current location if GPS available (start using GPS on device; later look at bluetooth/wireless connection to GPS)  

•	has drawing tools to put in points lines, polygon, multipoint, different tool for each geometry type; for portryala start with dots lines, polys, all same symbol. 
•  select existing feature(s) from loaded vector data to define spot--description or create relationships
display options; -- labeling spots.. strike dip stick for orientation measure; fall back -- sketch symbol as graphic; have 36 symbols for different strikes. color scheme

•	Can select new and/or existing geometries and  link with a 'spot' observation or assign to group defined base on arbitrary criteria.     
•	This sends message to spot editor, open editor window (prepopulate with background information--who, what, link to geometry)
•	User selects kind of description (fault, bedding, fabric, fold...); this loads content model for description and spins up form interface
•	attach picture, add sketch (use device camera to start).  
•	Sketch tool.... 
vadd spots in picture or sketch (use same image interface) 
•	save button to commit notes
•	push data to home base
•	see description of exiting spot
•	select and edit description of existing spot


###Editor capabilities: ###
-- Content model defines datatypes and vocabularies associated with properties.  
-- Vocabulary appears in pick list  
-- Can choose to restrict to vocabulary or allow user to add terms.   
--	Added terms appear in pick list  
--	user can add properties dynamically; these are added to the content model (along with metadata--user provides definition of property, datatype, vocabulary name or link)  
--	New properties appear in form  
--	Links/relationships (create group) (version 2) … have control that lets user find/navigate to existing spot observations in the database (either the local cache if offline or 'home base' if online), select related items and assign a relationship type.   
--	Relationship type vocabulary available, user can add new relationships like new properties. A relationship definition might specify the source and target description types, which would make locating target items easier.  
--	[version 2-- when operating with a GIS application like ArcMap or QGIS, relationships could be added by selecting spots on the map, or geometries in a dataset]  

Do in Desktop (network connected browser application):

- Project configuration workflow:
- load images
- project check/validation
- images are in file system on server


Import existing data
Jason-- set up web app to map fields to neo4j
has to get vocabulary (unique values)
basic template for bsic data 
