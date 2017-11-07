# SeaDataNet Climatology re-organized by EMODnet Physics

[Original data product](http://sdn.oceanbrowser.net/web-vis/?server=http://gher-diva.phys.ulg.ac.be/web-vis/Python/web/wms)

[EMODnet Physics product page](http://www.emodnet-physics.eu/Map/Products/V2/PRODUCTS.aspx?PRODTYPE=CL)

## WMS service url

##### Arctic Temperature WMS service url
http://thredds.emodnet-physics.eu/thredds/wms/SeaDataNet/Arctic/Temperature.19002014.4Danl.nc?
#####	Arctic Salinity WMS servcie url
http://thredds.emodnet-physics.eu/thredds/wms/SeaDataNet/Arctic/Salinity.19002014.4Danl.nc?
#####	Atlantic Temperature WMS service url
http://thredds.emodnet-physics.eu/thredds/wms/SeaDataNet/Atlantic/Temperature.19002013.4Danl.nc?
#####	Atlantic Salinity WMS servcie url
http://thredds.emodnet-physics.eu/thredds/wms/SeaDataNet/Atlantic/Salinity.19002013.4Danl.nc?
#####	Baltic Sea Temperature WMS service url
http://thredds.emodnet-physics.eu/thredds/wms/SeaDataNet/Baltic/Temperature.19002012.4Danl.nc?
#####	Baltic Sea Salinity WMS servcie url
http://thredds.emodnet-physics.eu/thredds/wms/SeaDataNet/Baltic/Salinity.19002012.4Danl.nc?
#####	Black Sea Temperature WMS service url
http://thredds.emodnet-physics.eu/thredds/wms/SeaDataNet/BlackSea/Temperature.4Danl.nc?
#####	Black Sea Salinity WMS servcie url
http://thredds.emodnet-physics.eu/thredds/wms/SeaDataNet/BlackSea/Salinity.4Danl.nc?
#####	Mediterranean Sea Temperature WMS service url
http://thredds.emodnet-physics.eu/thredds/wms/SeaDataNet/MediterraneanSea/Temperature.19002013.4Danl.nc?
#####	Mediterranean Sea Salinity WMS servcie url
http://thredds.emodnet-physics.eu/thredds/wms/SeaDataNet/MediterraneanSea/Salinity.19002013.4Danl.nc?
#####	North Sea Temperature WMS service url
http://thredds.emodnet-physics.eu/thredds/wms/SeaDataNet/NorthSea/Temperature.19752005.4Danl.nc?
#####	North Sea Salinity WMS servcie url
http://thredds.emodnet-physics.eu/thredds/wms/SeaDataNet/NorthSea/Salinity.19752005.4Danl.nc?
			
# LAYERS PARAMETER

  Parameters for Temperature layers

    LAYERS: 'Temperature_L2'

  Parameters for Salinity layers
    
    LAYERS: 'Salinity_L2'

# GENERAL PARAMETERS

Parameters for Temperature and Salinity layers
  
		ELEVATION:-0.0
		ABOVEMAXCOLOR: extend
		BELOWMINCOLOR: extend
		STYLES: boxfill/rainbow
		VERSION: 1.3.0

Parameters for Temperature layers

    COLORSCALERANGE: -10,30

Parameters for Salinity layers 
		
    COLORSCALERANGE: 0,40
		
# TIME PARAMETERS
	
	January 
		TIME: 1900-01-01T00:00:00.000Z
	February 
		TIME: 1900-02-01T00:00:00.000Z
	March 
		TIME: 1900-03-01T00:00:00.000Z
	April 
		TIME: 1900-04-01T00:00:00.000Z
	May
		TIME: 1900-05-01T00:00:00.000Z
	June
		TIME: 1900-06-01T00:00:00.000Z
	July
		TIME: 1900-07-01T00:00:00.000Z
	August 
		TIME: 1900-08-01T00:00:00.000Z
	September 
		TIME: 1900-09-01T00:00:00.000Z
	October
		TIME: 1900-10-01T00:00:00.000Z  (WARNING: not present in "North Sea" Temperature layer)
	November 
		TIME: 1900-11-01T00:00:00.000Z
	December 
		TIME: 1900-12-01T00:00:00.000Z

# OPENLAYERS EXAMPLE

Arctic Temperature for April
```javascript
var layer = new ol.layer.Tile({          
	source: new ol.source.TileWMS({
	url: 'http://thredds.emodnet-physics.eu/thredds/wms/SeaDataNet/Arctic/Salinity.19002014.4Danl.nc?',
	params: {
		'LAYERS': 'Temperature_L2', 
		'TILED': true,
		'ELEVATION': -0.0,
		'ABOVEMAXCOLOR': 'extend',
		'BELOWMINCOLOR': 'extend',
		'STYLES': 'boxfill/rainbow',
		'VERSION': '1.3.0',
		'COLORSCALERANGE': '-10,30',
		'TIME': '1900-04-01T00:00:00.000Z'
		}
	})
});
```

# LEAFLET EXAMPLE

Arctic Temperature for April
```javascript
var layer = L.tileLayer.wms(
	'http://thredds.emodnet-physics.eu/thredds/wms/SeaDataNet/Arctic/Salinity.19002014.4Danl.nc?', 
	{
		'LAYERS': 'Temperature_L2', 
		'TILED': true,
		'ELEVATION': -0.0,
		'ABOVEMAXCOLOR': 'extend',
		'BELOWMINCOLOR': 'extend',
		'STYLES': 'boxfill/rainbow',
		'VERSION': '1.3.0',
		'COLORSCALERANGE': '-10,30',
		'TIME': '1900-04-01T00:00:00.000Z'		
	});
```

