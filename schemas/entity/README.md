# Health issues tracking data models

These data models allow to perform health data tracking. They have been designed with a view to enabling trivial interoperability between FIWARE NGSI version 2 and oMobile-Health. As a result, property names have not been normalized to the camelCasesyntax, they remain as currently specified by [Open mHealth](http://www.openmhealth.org/). That is the rationale behind naming entity types with omh prefix. However, a few properties are added, so that FIWARE NGSI version 2 implementations can properly store respective data.

oHealth-Context data model defines the following entity:

## Physical Test

This section introduce a single schema to define an entity to define a physical test. It concentrates sensor data collected along a controlled test from a physical device carried/worn by a user while performing a supervised physical test.

### Data model
* ```id:``` Entity's unique identifier which must follow a specific format (i.e., `<`DEVICE UNIQUE ID`>`-`<`TEST NUMBER`>`; without blank spaces in between and using capital letters).
* ```type:``` It must be PhisicalTest.
* ```test:``` Physical test to measure risk of fall (i.e., Timed Up and Go, 30 second sit to stand test, Four Step Square Test).
* ```sensor:``` Defines sensors devices used to obtain information from mobile devices (i.e., Accelerometer, Orientation).
* ```speed:``` Represents the speed of the sensors devices used to collect data (e.g., hz). 
* ```data:``` Represents a set of sensor data collected by a mobile device used by a user while performing a supervised physical test.

### Example of use
```
{
    "id": "smarthphone-2",
    "type": "PhysicalTest",
    "test": {
        "value": "Timed Up and Go",
        "type": "test-type"
        },
    "sensor": {
        "value": "Accelerometer",
        "type": "sensor-type"
        },
    "speed": {
        "value": "hz",
        "type": "sensor-speed"
        },
    "data": {
        "value": "0.0635477304458618,0.00490868091583252,0.0516815185546875,2016-09-08T10:51:41.341Z-0500",
        "type": "sensor-data"
        },
    "omh:start_date_time": {
        "value": "2017-02-01T07:35:00Z-0800",
        "type": "omh:time-interval"
    },
    "omh:end_date_time": {
        "value": "2017-02-01T07:35:00Z-0800",
        "type": "omh:time-interval"
    }
}
```
