# Physical Test

This section introduce a single schema to define an entity to define a physical test. It concentrates sensor data collected along a controlled test from a physical device carried/worn by a user while performing a supervised physical test.

## Example of use
```
{
    "id": "smarthphone-1",
    "type": "PhysicalTest",
    "test": {
        "value": "Timed Up and Go"
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
        "value": { 
                0.0635477304458618,0.00490868091583252,0.0516815185546875,2016-09-08T10:51:41.341Z-0500
                0.0342383980751038,0.0448725819587708,-0.0150432586669922 2016-09-08T10:51:41.395Z-0500
                0.0336517691612244,0.0183262079954147,0.0110836029052734,2016-09-08T10:51:41.460Z-0500
                0.0376898050308228,0.0156682282686234,0.0296926498413086,2016-09-08T10:51:41.517Z-0500
                0.0559502840042114,0.0154750347137451,0.0503759384155273,2016-09-08T10:51:41.559Z-0500
                0.0620525479316711,0.0435315370559692,0.0377740859985352,2016-09-08T10:51:41.600Z-0500
                0.0869676470756531,0.0758075714111328,0.0395002365112305,2016-09-08T10:51:41.649Z-0500
                0.0620377659797668,0.0276693403720856,0.00120067596435547 2016-09-08T10:51:41.706Z-0500
            },
        "type": "sensor-data"
        },
    "timeInterval": {
        "duration": {
            "value": 20,
            "unit": "sec"
        },
        "start_date_time": "2017-02-01T07:35:00Z-800"
    }
}
```

