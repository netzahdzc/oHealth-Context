# Physical Test

This section introduce a single schema to define an entity to define a physical test. It concentrates sensor data collected along a controlled test from a physical device carried/worn by a user while performing a supervised physical test.

## Example of use
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
        "type": "time-interval"
    },
    "omh:end_date_time": {
        "value": "2017-02-01T07:35:00Z-0800",
        "type": "time-interval"
    }
}
```

