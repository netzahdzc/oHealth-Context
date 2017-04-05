# PhysicalTest

## Description

Sensor data collected along a physical test in the scope of health. This model has been developed based on [Open mHealth](http://www.openmhealth.org/). 

## Data Model

A JSON Schema corresponding to this data model can be found [here](https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/PhysicalTest/physical-test-1.x.json).

+ `id` : Entity's unique identifier which must follow a specific format (i.e., \<DEVICE UNIQUE ID\>-\<SENSOR\>-\<TEST NUMBER\>; without blank spaces in between and using capital letters).
   + Mandatory.

+ `type` : Entity type. It must be equal to `PhysicalTest`.
   + Mandatory.

+ `test` : Name of physical test.
   + Attribute type: [test-type](https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/dataType/test-type-1.x.json).
   + Mandatory.

+ `refDevice` : Reference to the device(s) used to monitor this test.
   + Attribute type: List of Reference to entity(ies) of type [Device](https://github.com/netzahdzc/dataModels/blob/master/Device/Device/doc/spec.md)
   + Mandatory.
```
+ `data` : Represents a set of sensor data collected by a mobile device used by a user while performing a supervised physical test.
   + Attribute type: [sensor-data](https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/dataType/sensor-data-1.x.json).
   + Attribute metadata:
      + `format` : This schema defines data format used along the gathering process.
         + Attribute type: [data-format](https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/dataType/data-format-1.x.json)
         + Allowed values: (`csv`, `tsv`).
      + `device` : This schema defines a set of diverse devices used to obtain information in the scope of mobile sensing.
         + Attribute type: [device-type](https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/dataType/device-type-1.x.json).
         + Allowed values: (`Smartphone`, `Smartwatch`).
      + `model` : Device model.
         + Attribute type: Text.
      + `brand` : Device brand defined from respective manufacture.
         + Attribute type: Text.
      + `software` : Software version defined from installed program that is gathering sensor data from respective device.
         + Attribute type: Text.
      + `library` : Sofware version or description to further identify the library used by the main software to collect sensor data.
         + Attribute type: Text.
   + Mandatory.

+ `sensor` : Defines sensors devices used to obtain information from mobile devices (i.e., Accelerometer, Orientation).
   + Attribute type: [sensor-type](https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/dataType/sensor-type-1.x.json).
   + Attribute metadata:
      + `speed` : Represents the speed of the sensors devices used to collect data (e.g., hz).
         + Attribute type: [sensor-speed](https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/dataType/sensor-speed-1.x.json).
         + Allowed values: (`hz`).
   + Mandatory.
```
+ `omh:end_date_time` : Time the test starts.
   + Attribute type: [omh:date-time](http://www.openmhealth.org/schema/omh/date-time-1.0.json).
   + Mandatory.

+ `omh:start_date_time` : Time the test ends.
   + Attribute type: [omh:date-time](http://www.openmhealth.org/schema/omh/date-time-1.0.json).
   + Mandatory.


    
## Examples of use

```
{  
   "id": "test-ffffffffff9cbbf4465f0ef30033c587-acc-7118",
   "type": "PhysicalTest",
   "test": {  
      "value": "Timed Up and Go",
      "type": "test-type"
   },
   "refDevice": {
      "id": "device-ffffffffff9cbbf4465f0ef30033c587-acc-7118",
      "type": "Device",
      "category": ["smartphone"],
      "controlledProperty": ["accelerometer","orientation"],
      "osVersion": "Android 4.0",
      "softwareVersion": "MA-Test 1.6",
      "hardwareVersion": "GP-P9872",
      "firmwareVersion": "SM-A310F",
      "refDeviceModel": {
         "id": "model-ffffffffff9cbbf4465f0ef30033c587-acc-7118",
          "type": "DeviceModel",
          "function": ["sensing"],
          "energyLimitationClass": "E1",
          "brandName": "Xioami",
          "modelName": "MI 5",
          "manufacturerName": "Samsung",
      },
      "value": {"acceleration" : "-69.895,72.0493,4.90137,2017-01-18T20:45:43.765Z-0800 -69.844,72.0726,4.85817,2017-01-18T20:45:43.799Z-0800...", "orientation" : "-69.895,72.0493,4.90137,2017-01-18T20:45:43.765Z-0800 -69.844,72.0726,4.85817,2017-01-18T20:45:43.799Z-0800..." },
      "configuration": {
         "data": {  
            "format": {
               "value": "csv",
               "type": "data-format"
         }
       },
         "sensor": {  
            "speed": {
               "value": "60",
               "type": "hz"
            }
         }
      },
      "dateCreated": "2017-04-05"
   },
   "omh:end_date_time": {
      "value": "2017-01-18T20:45:58.447Z-0800",
      "type": "omh:date-time"
   },
   "omh:start_date_time": {
      "value": "2017-01-18T20:45:42.697Z-0800",
      "type": "omh:date-time"
   }
}
```
    
## Use it with a real service

T.B.D.

## Open Issues

T.B.A.