# caic-data
Repository for CAIC (Colorado Avalanche Information Center) GIS data.
This data is scraped from their website.  http://avalanche.state.co.us/

### About
All data is in EPSG:3857 for quick use in web mapping applications.

Files are in GeoJSON format for Git version control purposes.

## Data Layers

#### caic_accidents
Contains all avalanche accidents from 2009-Present.  Accidents going back to 1993 can be added by hand.

| Field Name | Details |
|------------|---------|
| acc_id    | The CAIC accident id.  You can use this to look up accident details with GET on their PHP pages. |
| acc_date | The date of the accident. |
| acc_travel | The mode of travel that the victims were using. |
| acc_activi | The backcountry/recreational activity being performed during the accident. |
| acc_locati | A brief description of the avalanche site. |
| acc_no_cau | The number of people caught in the avalanche. |
| acc_no_bur | The number of people partially or fully buried by the avalanche. |
| acc_no_kil | The number of people killed by the avalanche. |
| acc_type | Usually "inv" (investigation), but sometimes "rep" (report). |
| acc_lat | Latitude. |
| acc_lon | Longitude. |

#### caic_zones
The zones that the CAIC uses to issue forecasts and warnings.

| Field Name | Details |
|------------|---------|
| Zone | The name of the zone, e.g. "Vail & Summit County" |
| caic_id | The id given to the zone by CAIC. |

#### caic_observations
Contains all field observations from 2010  to 11/20/2015.

| Field Name | Details |
|------------|---------|
|obs_id | The CAIC observation id.  You can use this to look up observation details with GET on their PHP pages. |
| obs_date | The date of the observation. |
| obs_bc_landmark | The backcountry 'landmark' -- recognizable or notable features near the observation. |
| obs_caught_avi |  |
| obs_obsfm |  |
| obs_rand |  |
| obs_see_avi |  |
| obs_trigger_avi |  |
| obs_wx_precip_rate | The precipitation rate at the time of the observation. |
