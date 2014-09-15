Strabos: an environment for structural geology data acquisition, storage, sharing and access
Field data work flow:
•	set up field project in office-- upload base maps, shape files existing points, get stuff in correct projections (list of supported projections), put in  basic metadata (who, what, why, access control).  
•	Allow shape files in view
•	Push configuration to Strabo mobile spot editor (as opposed to strabo desktop or strabo database)
•	basic map view allows display of multiple layers, using any georeferenced image (all have to be in same projection
•	Connects to GPS to display current location if GPS available (start using GPS on device; later look at bluetooth/wireless connection to GPS)

•	has drawing tool to put in points lines, polygon, multipoint. 
•	Select new and/or existing geometries and assign identity to link with a 'spot' observation
•	select existing feature(s) from loaded vector data to define spot--description or create relationships
•	This sends message to spot editor, open editor window (prepopulate with background information--who, what, link to geometry)
•	User selects kind of description (fault, bedding, fabric, fold...); this loads content model for description and spins up form interface
Editor capabilities: 
o	content model defines datatypes and vocabularies associated with properties. 
o	vocabulary appears in pick list
o	Can choose to restrict to vocabulary or allow user to add terms. 
o	Added terms appear in pick list
o	user can add properties dynamically; these are added to the content model (along with metadata--user provides definition of property, datatype, vocabulary name or link)
o	New properties appear in form
o	Links/relationships (create group) (version 2) … have control that lets user find/navigate to existing spot observations in the database (either the local cache if offline or 'home base' if online), select related items and assign a relationship type. 
o	Relationship type vocabulary available, user can add new relationships like new properties. A relationship definition might specify the source and target description types, which would make locating target items easier.
o	[version 2-- when operating with a GIS application like ArcMap or QGIS, relationships could be added by selecting spots on the map, or geometries in a dataset]

Desktop:
Project configuration workflow:
load images
project check/validation
images are in file system on server


Import existing data
Jason-- set up web app to map fields to neo4j
has to get vocabulary (unique values)
basic template for bsic data 
