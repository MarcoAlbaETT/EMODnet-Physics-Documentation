
# EMODnet Physics Marine Mammals Product based on MEOP-CTD database

MEOP-CTD database have been used in EMODnet Physics to create route for each deployement for the parameters 'Sea temperature' and 'Practical Salinity'

Both products can be displayed on a web map application at the following address:

Sea temperature

[http://www.emodnet-physics.eu/map/Products/V2/PRODUCTS.aspx?PRODTYPE=RT&type=MM&param=TEMP](http://www.emodnet-physics.eu/map/Products/V2/PRODUCTS.aspx?PRODTYPE=RT&type=MM&param=TEMP)

Practical Salinity

[http://www.emodnet-physics.eu/map/Products/V2/PRODUCTS.aspx?PRODTYPE=RT&type=MM&param=PSAL](http://www.emodnet-physics.eu/map/Products/V2/PRODUCTS.aspx?PRODTYPE=RT&type=MM&param=PSAL)

The products supports two dimensions:

-   **Time dimension**  
    the data are included in the interval from
    2004-01-27T08:26:00.000Z to 2016-02-22T07:10:00.000Z and can be
    accessed with specific time or time interval. WMS TIME parameter is
    based on [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601)

-   **Elevation dimension**  
    the data use the value 'depth' as an elevation dimension with
    value from 0 to 9 with the following meanings:

> Table 1 -- Depth descriptions

  **Depth value** |  **Meanings**
  ----------------- |----------------------
  **0**|             near surface
  **1**|             near surface to 50 m
  **2**|             50 m to 100 m
  **3**|             100 m to 250 m
  **4**|             250 m to 500 m
  **5**|             500 m to 1000 m
  **6**|             1000 m to 1500 m
  **7**|             1500 m to 2000 m
  **8**|             2000 m to 2500 m
  **9**|             more than 2500 m

The products data are stored with the following structure:
>Table 2 -- Data structure

  Property | Type | Description
  -------- | ---- | -----------
  platformid | BigDecimal | Unique identifier of the platform in EMODnet
  date        |    Timestamp  |  Datetime of the observation
  isodate      |   String     |  Datetime of the observation in [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601) format
  depth        |   Double     |  Depth of the observation (Table 1)
  value       |    Double     |  Value of the parameter
  code         |   String     |  Code of the parameter ("TEMP" = Sea Temperature; "PSAL" = Practical Salinity)
  routetype    |   String     |  Fixed value "mm"
  qc            |  BigDecimal |  Quality Flag (Table 3)
  wkb_geometry |  LineString |  Geometry field (WKT Linestring)
  species      |   String     |  Specie of the platform (see Table 4 and Table 5 for methods to retrieve the list of available species, table 6 for the list of available species)

> Table 3 -- QC description

  QC | Description
  ---| -----------
  0        |No QC tests have been performed
  1        |Observation good
  2        |Observation probably good (implies some uncertainty)
  3        |Observation thought to be bad but may be recoverable
  4        |Observation thought to be bad and irrecoverable

>Table 4 -- WFS request to retrieve the list of species for the parameter "Sea Temperature"

Data format | link
----------- | ----
  CSV   | [http://geoserver.emodnet-physics.eu/geoserver/emodnet/ows?service=WFS&version=1.0.0&request=GetFeature&typeName=emodnet:sql\_mm\_temp\_0d\_species&outputFormat=csv](http://geoserver.emodnet-physics.eu/geoserver/emodnet/ows?service=WFS&version=1.0.0&request=GetFeature&typeName=emodnet:sql_mm_temp_0d_species&outputFormat=csv)
    XML|    [http://geoserver.emodnet-physics.eu/geoserver/emodnet/ows?service=WFS&version=1.0.0&request=GetFeature&typeName=emodnet:sql\_mm\_temp\_0d\_species&outputFormat=text%2Fxml%3B%20subtype%3Dgml%2F2.1.2](http://geoserver.emodnet-physics.eu/geoserver/emodnet/ows?service=WFS&version=1.0.0&request=GetFeature&typeName=emodnet:sql_mm_temp_0d_species&outputFormat=text%2Fxml%3B%20subtype%3Dgml%2F2.1.2)
  JSON|   [http://geoserver.emodnet-physics.eu/geoserver/emodnet/ows?service=WFS&version=1.0.0&request=GetFeature&typeName=emodnet:sql\_mm\_temp\_0d\_species&outputFormat=application%2Fjson](http://geoserver.emodnet-physics.eu/geoserver/emodnet/ows?service=WFS&version=1.0.0&request=GetFeature&typeName=emodnet:sql_mm_temp_0d_species&outputFormat=application%2Fjson)


>Table 5 - WFS request to retrieve the list of species for the parameter "Practical Salinity"

Data format | link
----------- | ----
  CSV   | [http://geoserver.emodnet-physics.eu/geoserver/emodnet/ows?service=WFS&version=1.0.0&request=GetFeature&typeName=emodnet:sql\_mm\_psal\_0d\_species&outputFormat=csv](http://geoserver.emodnet-physics.eu/geoserver/emodnet/ows?service=WFS&version=1.0.0&request=GetFeature&typeName=emodnet:sql_mm_psal_0d_species&outputFormat=csv)  
  XML  |  [http://geoserver.emodnet-physics.eu/geoserver/emodnet/ows?service=WFS&version=1.0.0&request=GetFeature&typeName=emodnet:sql\_mm\_psal\_0d\_species&outputFormat=text%2Fxml%3B%20subtype%3Dgml%2F2.1.2](http://geoserver.emodnet-physics.eu/geoserver/emodnet/ows?service=WFS&version=1.0.0&request=GetFeature&typeName=emodnet:sql_mm_psal_0d_species&outputFormat=text%2Fxml%3B%20subtype%3Dgml%2F2.1.2)
  JSON  | [http://geoserver.emodnet-physics.eu/geoserver/emodnet/ows?service=WFS&version=1.0.0&request=GetFeature&typeName=emodnet:sql\_mm\_psal\_0d\_species&outputFormat=application%2Fjson](http://geoserver.emodnet-physics.eu/geoserver/emodnet/ows?service=WFS&version=1.0.0&request=GetFeature&typeName=emodnet:sql_mm_psal_0d_species&outputFormat=application%2Fjson)

>Table 6 - list of available species

Species|
-------|
Southern ellie|
Green turtle|
Crabeater seal|
Hooded seal|
Harp seal|
Ringed seal|
Grey seal|
Weddell seal|
Northern ellie|


The products data are accessible with standard OGC WMS and WFS services on the [EMODnet Geoserver](http://geoserver.emodnet-physics.eu/geoserver/) server:

**WMS GetCapabilities**

Sea Temperature

[http://geoserver.emodnet-physics.eu/geoserver/emodnet/route\_mm\_temp\_0d/wms?service=WMS&version=1.1.0&request=GetCapabilities&namespace=emodnet](http://geoserver.emodnet-physics.eu/geoserver/emodnet/route_mm_temp_0d/wms?service=WMS&version=1.1.0&request=GetCapabilities&namespace=emodnet)

Practical Salinity 

[http://geoserver.emodnet-physics.eu/geoserver/emodnet/route\_mm\_psal\_0d/wms?service=WMS&version=1.1.0&request=GetCapabilities&namespace=emodnet](http://geoserver.emodnet-physics.eu/geoserver/emodnet/route_mm_psal_0d/wms?service=WMS&version=1.1.0&request=GetCapabilities&namespace=emodnet)

**WFS GetCapabilities**

Sea Temperature

[http://geoserver.emodnet-physics.eu/geoserver/emodnet/sql\_mm\_temp\_0d\_species/wms?service=WFS&version=1.1.0&request=GetCapabilities](http://geoserver.emodnet-physics.eu/geoserver/emodnet/sql_mm_temp_0d_species/wms?service=WFS&version=1.1.0&request=GetCapabilities)

Practical Salinity 

[http://geoserver.emodnet-physics.eu/geoserver/emodnet/sql\_mm\_psal\_0d\_species/wms?service=WFS&version=1.1.0&request=GetCapabilities](http://geoserver.emodnet-physics.eu/geoserver/emodnet/sql_mm_psal_0d_species/wms?service=WFS&version=1.1.0&request=GetCapabilities)

### Access to data: WMS LeafletJS example

This code load the WMS layer for Temperature parameter with the default
value of elevation (zero), all QC value and the most recent date
available:
```javascript
wmsOptions={
    layers: "emodnet:route_mm_temp_0d",
    style: "line",
    format:"image/png",
    transparent: "true"
};
var wmsLayer = L.tileLayer.wms("http://geoserver.emodnet-physics.eu/geoserver/emodnet/route_mm_temp_0d/wms?", wmsOptions).addTo(map);
```

To furter refine the visualization, three other options are available
(this options can be used also for WFS request):

1.  **elevation**: this option can be used to specifiy the depth of the
    routes to show and his value is in the format min/max (based on
    table 1) .
    Example:

    * To show only route near surface use the value "0/0"  
    * To show route between 100m and 1000m use the value "3/5"

2.  **time**: this option can be used to show routes between a start and end date and his value is in the format startdate/enddate; all date
    are in [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601) format. The list of available date are returned by the WMS GetCapabilities request.\
    Example:

    * To show routes for the year 2010 use the value "2010-01-01T00:00:00.000Z/2010-12-31T23:59:59.999Z"

3.  **cql\_filter**: this option can be used to specify the QC and/or the species of the routes to show.\
    Example:

    * to show only routes with QC equal to 1 use the value "qc=1"

    * to show only route with QC equal to 1 or 2 use the value "qc=1 or qc=2"

    * to show only route for the \"Weddell seal\" species use the value "species='Weddell seal'"

    * to show only routes for the \"Weddell seal\" species with QC equal to 1 use the value "qc=1 and species='Weddell seal'"

This code show the routes for Temperature parameter for the first 6
months of the 2010, with depth between near surface and 100m, the QC
equal to 1 and only for the the Southern Ellie species:

```javascript
wmsOptions={
	layers: "emodnet:route_mm_temp_0d",
	style: "line",
	format:"image/png",
	transparent: "true",
	elevation: "0/2",
	time:"2010-01-01T00:00:00.000Z/2010-06-30T23:59:59.999Z",
	cql_filter:"qc=1 and species='Southern ellie'"
};
var wmsLayer = L.tileLayer.wms("http://geoserver.emodnet-physics.eu/geoserver/emodnet/route_mm_temp_0d/wms?", wmsOptions).addTo(map);
```

