# REACH-cruise-reports
A website reporting on data from the USF IMaRS FLARACEP (REACH) research cruises.

# Raw Data Inputs
Following a research cruise, raw data is uploaded into [this box.com folder](https://usf.app.box.com/folder/321222942799).
The directory structure is expected to match the pattern `IMaRS_Projects/FLRACEP V (REACH) project/DataManagement/{CRUISE_ID}/DataCollection/{DATA_TYPE}/`.

The following file patterns are expected for each `DATA_TYPE`:

* `FlowThrough`:
  * `{YEAR}_{MONTH}_{MARINE_TECH_ENTERED_STRING}_FT{UNKNOWN_IDENTIFIER}.hdr`
  * `{YEAR}_{MONTH}_{MARINE_TECH_ENTERED_STRING}_FT{UNKNOWN_IDENTIFIER}.hex`
  * `{YEAR}_{MONTH}_{MARINE_TECH_ENTERED_STRING}_FT{UNKNOWN_IDENTIFIER}.XMLCON`
* `EK80`:
  * `D{YEAR}{MONTH}{DAY}-T{HOUR}{MINUTE}{SECOND}.raw`
  * `D{YEAR}{MONTH}{DAY}-T{HOUR}{MINUTE}{SECOND}.idx`
* `SCS`:
  * `/Event Data/`
    * `C_{EVENT_ID}.elg`
    * `MetaDataSEnsorDescription_{EVENT_ID}.CSV`
    * `{MARINE_TECH_ENTERED_STRING}_Event File_{STATION_ID}_{EVENT_ID}.LOG`
    * `{MARINE_TECH_ENTERED_STRING}_Event File_{STATION_ID}_{EVENT_ID}.hdr`
    * `EventReportFile_{EVENT_ID}.txt`
    * `ButtonActivity_{EVENT_ID}.txt`
  * `{SENSOR_NAME}_{YEAR}{MONTH}{DAY}-{HOUR}{MINUTE}{SECOND}.{Raw | log | xml}` (raw, log, or xml depending on sensor)
* `CTD`:
  * `Processed/{STATION_ID}_processed.cnv`
  * `{STATION_ID}.mrk`
  * `{STATION_ID}.hex`
  * `{STATION_ID}.hdr`
  * `{STATION_ID}.XMLCON`
  * `{STATION_ID}.bl`
