# EMODnet Physics Web Service

<table class="table">
<tbody>
<tr>
<th>Method<br>(click method name for description of return variables)</th>
<th>Description</th>
<th>

Parameters ([description](#parameters-description))

</th>
<th>Example</th>
</tr>
<tr>
<td>

[GetAllDataOwner](#getalldataowner)
</td>
<td>it gives the list and details of the data owners/contributors</td>
<td></td>
<td>

[XML](http://www.emodnet-physics.eu/Map/service/WSEmodnet2.aspx?q=GetAllDataOwner)  
[TXT](http://www.emodnet-physics.eu/Map/service/WSEmodnet2.aspx?q=GetAllDataOwner&Format=txt)
</td>
</tr>

<tr>
<td>

[GetAllLatestData60Days](#getalllatestdata60days)</td>
<td>it gives the latest data (60 days) for the specified platform</td>
<td>PlatformID
</td>
<td>

[XML](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllLatestData60Days&PlatformID=10000)  
[TXT](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllLatestData60Days&PlatformID=10000&Format=txt)</td>
</tr>
<tr>
<td>

[GetAllLatestDataCode](#getalllatestdatacode)</td>
<td>it gives the latest data (60 days) for the specified platform and parameter</td>
<td>PlatformID<br>
ParamCode</td>
<td>

[XML](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllLatestDataCode&PlatformID=10000&ParamCode=TEMP)  
[TXT](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllLatestDataCode&PlatformID=10000&ParamCode=TEMP&Format=txt)</td>

</tr>

<tr>

<td>

[GetAllLatestDataFromTo](#getalllatestdatafromto)</td>
<td>it gives the latest data (up to latest 60 days) for the specified platform within the specified time window</td>
<td>PlatformID<br>
StartDate<br>
EndDate</td>

<td>

[XML](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllLatestDataFromTo&PlatformID=10000&StartDate=24/09/2017&EndDate=08/11/2017)  
[TXT](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllLatestDataFromTo&PlatformID=10000&StartDate=24/09/2017&EndDate=08/11/2017&Format=txt)</td>

</tr>

<tr>

<td>

[GetAllLatestDataFromToCode](#getalllatestdatafromtocode)</td>
<td>it gives the latest data (up to latest 60 days) for the specified platform and parameter within the specified time window</td>
<td>PlatformID<br>
ParamCode<br>
StartDate<br>
EndDate</td>
<td>

[XML](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllLatestDataFromToCode&PlatformID=10000&ParamCode=TEMP&StartDate=24/09/2017&EndDate=08/11/2017)  
[TXT](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllLatestDataFromToCode&PlatformID=10000&ParamCode=TEMP&StartDate=24/09/2017&EndDate=08/11/2017&Format=txt)</td>

</tr>

<tr>

<td>

[GetAllLatestDataParameterGroup](#getalllatestdataparametergroup)</td>
<td>it gives the latest data for the specified platform and parameter</td>
<td>PlatformID<br>
ParameterGroupID
</td>

<td>

[XML](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllLatestDataParameterGroup&PlatformID=10000&ParameterGroupID=10)  
[TXT](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllLatestDataParameterGroup&PlatformID=10000&ParameterGroupID=10&Format=txt)</td>

</tr>

<tr>

<td>

[GetAllParameters](#getallparameters)</td>
<td>it gives the prameters description and codes</td>
<td></td>
<td>

[XML](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllParameters)  
[TXT](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllParameters&Format=txt)</td>

</tr>

<tr>

<td>

[GetAllParametersGroup](#getallparametersgroup)</td>
<td>it gives the parameters groups</td>
<td></td>
<td>

[XML](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllParametersGroup)  
[TXT](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllParametersGroup&Format=txt)</td>

</tr>

<tr>

<td>

[GetAllPlatforms](#getallplatforms)</td>
<td>it gives the platforms list and details</td>
<td></td>
<td>

[XML](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllPlatforms)  
[TXT](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllPlatforms&Format=txt)</td>

</tr>

<tr>

<td>

[GetPlatformId](#getplatformid)</td>
<td>it givest the platform details for the specified platform</td>
<td>PlatformID</td>

<td>

[XML](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetPlatformId&PlatformID=10746)  
[TXT](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetPlatformId&PlatformID=10746&Format=txt)</td>

</tr>

<tr>

<td>

[GetAllPlatformsBBoxCode](#getallplatformsbboxcode)</td>
<td>it gives the list of the platforms and details for the specified bounding box and parameter code</td>
<td>BBox<br>
ParamCode
</td>

<td>

[XML](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllPlatformsBBoxCode&BBox=-12,37,4,53&ParamCode=TEMP)  
[TXT](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllPlatformsBBoxCode&BBox=-12,37,4,53&ParamCode=TEMP&Format=txt)</td>

</tr>

<tr>

<tr>

<td>

[GetAllPlatformsDataOwner](#getallplatformsdataowner)</td>
<td>it gives the list of the platforms and details for the specified dataowner/contributor</td>
<td>DataOwnerCode</td>

<td>

[XML](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllPlatformsDataOwner&DataOwnerCode=ISPRA)  
[TXT](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllPlatformsDataOwner&DataOwnerCode=ISPRA&Format=txt)</td>

</tr>

<tr>

<td>

[GetAllPlatformsParameterGroup](#getallplatformsparametergroup)</td>
<td>it gives the list of the platforms and details for the specified parameter group</td>
<td>ParameterGroupID</td>

<td>

[XML](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllPlatformsParameterGroup&ParameterGroupID=10)  
[TXT](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllPlatformsParameterGroup&ParameterGroupID=10&Format=txt)</td>

</tr>

<tr>

<td>

[GetAllRoos](#getallroos)</td>
<td>it gives the ROOSs list and codes</td>
<td></td>
<td>

[XML](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllRoos)  
[TXT](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllRoos&Format=txt)</td>

</tr>

<tr>

<td>

[GetAllPlatformsRoos](#getallplatformsroos)</td>
<td>it gives the list of the platforms in the specified ROOS</td>
<td>RoosID</td>

<td>

[XML](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllPlatformsRoos&RoosID=7)  
[TXT](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetAllPlatformsRoos&RoosID=7&Format=txt)</td>

</tr>

<tr>

<td>

[GetPlatformMonthlyCDIAvailability](#getplatformmonthlycdiavailability)</td>
<td>it gives the list of avaialble monthly data files and the list of available CDIs for the specified platform</td>
<td>PlatformID</td>

<td>

[XML](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetPlatformMonthlyCDIAvailability&PlatformID=14500)  
[TXT](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetPlatformMonthlyCDIAvailability&PlatformID=14500&Format=txt)</td>

</tr>

<tr>

<td>

[GetPlatformMinMaxAVG](#getplatformminmaxavg)</td>
<td>it gives the parameters monthly average, monthly max and min for the specified platform</td>
<td>PlatformID</td>

<td>

[XML](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetPlatformMinMaxAVG&PlatformID=8551)  
[TXT](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetPlatformMinMaxAVG&PlatformID=8551&Format=txt)</td>

</tr>

<tr>

<td>

[GetMonthlyData](#getmonthlydata)</td>
<td></td>
<td>
usernameCMEMS<br>
passwordCMEMS<br>
PlatformID<br>
Parameter<br>
QC(optional)<br>
StartDate(optional)<br>
EndDate(optional)
</td>

<td>

[XML](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetMonthlyData&usernameCMEMS=user&passwordCMEMS=pass&PlatformID=8427&Parameter=TEMP&QC=1&StartDate=01/01/2017&EndDate=31/01/2017)  
[TXT](http://www.emodnet-physics.eu/Map/Service/WSEmodnet2.aspx?q=GetMonthlyData&usernameCMEMS=user&passwordCMEMS=pass&PlatformID=8427&Parameter=TEMP&QC=1&StartDate=01/01/2017&EndDate=31/01/2017&Format=txt)</td>

</tr>

</tbody>

</table>

# Parameters Description
parameters | description
---------------- | -----------
BBox | 
DataOwnerCode | 
ParamCode | 
Parameter | 
ParameterGroupID | 
PlatformID | 
QC | 
RoosID | 
StartDate, EndDate | 
usernameCMEMS, passwordCMEMS | 

# Method return variables


### GetAllDataOwner
return variables | description
---------------- | -----------
DataOwnerID | EMODnet Physics internal DataOwner ID
Code | DataOwner Acronym
Descr | DataOwner full name description
website | DataOwner website
country | DataOwner Country
EDMO | DataOwner EDMO code

### GetAllLatestData60Days
return variables | description
---------------- | -----------
LatestPlatformID | EMODnet Physics internal Platform ID
PlatformID | EMODnet Physics external Platform ID
Date | yyyy/mm/dd hh:mm:ss
Depth | measurement depth
ParamValue | ParameterCode 1 and value; ParameterCode 2 and value; … ; ParameterCode N and value;

### GetAllLatestDataCode
return variables | description
---------------- | -----------
atestPlatformID | EMODnet Physics internal Platform ID
PlatformID | EMODnet Physics external Platform ID
Date | yyyy/mm/dd hh:mm:ss
Depth | measurement depth
ParamValue | ParameterCode and value

### GetAllLatestDataFromTo
return variables | description
---------------- | -----------
LatestPlatformID | EMODnet Physics internal Platform ID
PlatformID | EMODnet Physics external Platform ID
Date | yyyy/mm/dd hh:mm:ss
Depth | measurement depth
ParamValue | ParameterCode 1 and value; ParameterCode 2 and value; … ; ParameterCode N and value;

### GetAllLatestDataFromToCode
return variables | description
---------------- | -----------
LatestPlatformID | EMODnet Physics internal Platform ID
PlatformID | EMODnet Physics external Platform ID
Date | yyyy/mm/dd hh:mm:ss
Depth | measurement depth
ParamValue | ParameterCode and value

### GetAllLatestDataParameterGroup
return variables | description
---------------- | -----------
LatestPlatformID | EMODnet Physics internal Platform ID
PlatformID | EMODnet Physics external Platform ID
Date | yyyy/mm/dd hh:mm:ss
Depth | measurement depth
ParamValue | ParameterCode and value

### GetAllParameters
return variables | description
---------------- | -----------
ParameterID | EMODnet Physics internal parameter ID
ParameterGroup | parameter description
Code | international code acronym
CFStandardName | standard parameter full name
Descr | parameter description
MeasurementUnit | measurement unit

### GetAllParametersGroup
return variables | description
---------------- | -----------
ParameterGroupID | EMODnet Physics internal parameter group ID
Descr | parameter group description

### GetAllPlatforms
return variables | description
---------------- | -----------
PlatformID | EMODnet Physics external Platform ID
PlatformType | Type of the platform
DataOwnerCode | data owner acronym
HistoricalPlatformCDI | is the platform connected to any SeaDataNet CDI?
PlatformCode | platform name
WMOPlatformCode | WMO code (if available)
MyOceanNumber | internal code to link to crosslink the platform and MYO products
Parameters | recorded parameters (international code acronym)
Latitude | Latitude
Longitude | Longitude
EDMO | EDMO code
LastDataMeasured | date of the last measurement
YearDataMeasured | list of the years when the platform worked
Provider | data owner acronym
InstitutionReference | data owner website
Contact | principal investigator - data curator emails
DataAssemblyCenter | data assembly full name

### GetPlatformId
return variables | description
---------------- | -----------
PlatformID | EMODnet Physics external Platform ID
PlatformType | Type of the platform
DataOwnerCode | data owner acronym
HistoricalPlatformCDI | is the platform connected to any SeaDataNet CDI?
PlatformCode | platform name
WMOPlatformCode | WMO code (if available)
MyOceanNumber | internal code to link to crosslink the platform and MYO products
Parameters | recorded parameters (international code acronym)
Latitude | Latitude
Longitude | Longitude
EDMO | EDMO code
LastDataMeasured | date of the last measurement
YearDataMeasured | list of the years when the platform worked

### GetAllPlatformsBBoxCode
return variables | description
---------------- | -----------
PlatformID | EMODnet Physics external Platform ID
PlatformType | Type of the platform
DataOwnerCode | data owner acronym
HistoricalPlatformCDI | is the platform connected to any SeaDataNet CDI?
PlatformCode | platform name
WMOPlatformCode | WMO code (if available)
MyOceanNumber | internal code to link to crosslink the platform and MYO products
Parameters | recorded parameters (international code acronym)
Latitude | Latitude
Longitude | Longitude
EDMO | EDMO code
LastDataMeasured | date of the last measurement
YearDataMeasured | list of the years when the platform worked
Institution | data owner acronym
InstitutionReference | data owner website
Contact | principal investigator - data curator emails
DataAssemblyCenter | data assembly full name

### GetAllPlatformsDataOwner
return variables | description
---------------- | -----------
PlatformID | EMODnet Physics external Platform ID
PlatformType | Type of the platform
DataOwnerCode | data owner code acronym
HistoricalPlatformCDI | is the platform connected to any SeaDataNet CDI?
PlatformCode | platform name
Parameters | recorded parameters (international code acronym)
Latitude | Latitude
Longitude | Longitude
EDMO | EDMO code
LastDataMeasured | date of the last measurement
YearDataMeasured | list of the years when the platform worked
Provider | data owner acronym
InstitutionReference | data owner website
Contact | principal investigator - data curator emails
DataAssemblyCenter | data assembly full name

### GetAllPlatformsParameterGroup
return variables | description
---------------- | -----------
PlatformID | EMODnet Physics external Platform ID
PlatformType | Type of the platform
DataOwnerCode | data owner code acronym
HistoricalPlatformCDI | is the platform connected to any SeaDataNet CDI?
PlatformCode | platform name
WMOPlatformCode | WMO code (if available)
MyOceanNumber | internal code to link to crosslink the platform and MYO products
Parameters | recorded parameters (international code acronym)
Latitude | Latitude
Longitude | Longitude
EDMO | EDMO code
LastDataMeasured | date of the last measurement
YearDataMeasured | list of the years when the platform worked
Institution | data owner acronym
InstitutionReference | data owner website
Contact | principal investigator - data curator emails
DataAssemblyCenter | data assembly full name

### GetAllRoos
return variables | description
---------------- | -----------
RoosID | EMODnet Physics internal ROOS ID
Code | ROOS acronym
Descr | ROOS full name

### GetAllPlatformsRoos
return variables | description
---------------- | -----------
PlatformID | EMODnet Physics external Platform ID
PlatformType | Type of the platform
DataOwnerCode | data owner acronym
HistoricalPlatformCDI | is the platform connected to any SeaDataNet CDI?
PlatformCode | platform name
WMOPlatformCode | WMO code (if available)
Parameters | recorded parameters (international code acronym)
Latitude | Latitude
Longitude | Longitude
EDMO | EDMO code
LastDataMeasured | date of the last measurement
YearDataMeasured | list of the years when the platform worked
Provider | data owner acronym
InstitutionReference | data owner website
Contact | principal investigator - data curator emails
DataAssemblyCenter | data assembly full name

### GetPlatformMonthlyCDIAvailability
return variables | description
---------------- | -----------
PlatformID | EMODnet Physics external Platform ID
PlatformType | Type of the platform
PlatformCode | platform name
EDMO | EDMO code
Parameters | recorded parameters (international code acronym)
Latitude | Latitude
Longitude | Longitude
LastDataMeasured | date of the last measurement
Provider | data owner acronym
CDISeriesID | list of available CDIs
MonthlyAvailability | list of year-month when the platform worked

### GetPlatformMinMaxAVG
return variables | description
---------------- | -----------
PlatformID | EMODnet Physics external Platform ID
Year | yyyy
Month | the month (1 -12)
Parameter | recorded parameters (international code acronym)
Min | the min recorded value for that month
Max | the max recorded value for that month
AVG | the avg recorded value for that month
Depth | depth of the measurement
QC | quality flag of data (0 no QC, 1 good, >3 not good/problems) - only QC = 1 are used
RoosID | EMODnet Physics internal ROOS ID
TotalRecordAVG | internal code
TotalRecord | internal code

### GetMonthlyData
return variables | description
---------------- | -----------
Date | yyyy/mm/dd hh:mm:ss
Depth | Depth
ParamQC | Parameter QC
ParamValue | Parameter Value
