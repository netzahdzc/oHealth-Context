# Health issues tracking data models

These data models allow to perform health data tracking. They have been designed with a view to enabling trivial interoperability between FIWARE NGSI version 2 and oMobile-Health. As a result, property names have not been normalized to the camelCasesyntax, they remain as currently specified by [Open mHealth](http://www.openmhealth.org/). That is the rationale behind naming entity types with omh prefix. However, a few properties are added, so that FIWARE NGSI version 2 implementations can properly store respective data.

oHealth-Context data model defines the following entity:

## Entities

This section introduce a number of schema to define an entitis. For instance the **physical test** concentrates sensor data collected along a controlled test from a physical device carried/worn by a user while performing a supervised physical test.

| Attribute| Description                                                                                                                              |
|---------------|------------------------------------------------------------------------------------------------------------------------------------------|
| id            | Entity's unique identifier which must follow a specific format (i.e., \<DEVICE UNIQUE ID\>-\<SENSOR\>-\<TEST NUMBER\>; without blank spaces in between and using capital letters). |
| type          | It must be PhisicalTest.                                                                                                                 |
| test          | Physical test to measure risk of fall (i.e., Timed Up and Go, 30 second sit to stand test, Four Step Square Test).                       |
| sensor        | Defines sensors devices used to obtain information from mobile devices (i.e., Accelerometer, Orientation).                               |
| speed         | Represents the speed of the sensors devices used to collect data (e.g., hz).                                                             |
| data          | Represents a set of sensor data collected by a mobile device used by a user while performing a supervised physical test.                 |

### Example of use
```
{  
   "id":"ffffffffff9cbbf4465f0ef30033c587-acc-7118",
   "type":"PhysicalTest",
   "test":{  
      "value":"Timed Up and Go",
      "type":"test-type",
      "metadata":{  
         "variant":{  
            "value":"NA",
            "type":"test-option"
         }
      }
   },
   "data":{  
      "value":"-69.895,72.0493,4.90137,2017-01-18T20:45:43.765Z-0800 -69.844,72.0726,4.85817,2017-01-18T20:45:43.799Z-0800 -69.8184,72.0956,4.84979,2017-01-18T20:45:43.859Z-0800 -69.7982,72.1125,4.83087,2017-01-18T20:45:43.892Z-0800 -69.7344,72.1441,4.77256,2017-01-18T20:45:43.930Z-0800 -69.6329,72.1785,4.6916,2017-01-18T20:45:43.957Z-0800 -69.5742,72.1842,4.63849,2017-01-18T20:45:43.984Z-0800 -69.5733,72.215,4.64865,2017-01-18T20:45:44.078Z-0800 -69.5594,72.2631,4.64678,2017-01-18T20:45:44.196Z-0800 -69.5009,72.2957,4.59217,2017-01-18T20:45:44.236Z-0800...",
      "type":"sensor-data",
      "metadata":{  
         "format":{  
            "value":"csv",
            "type":"format"
         },
         "device":{  
            "value":"Smartphone",
            "type":"device-type"
         },
         "model":{  
            "value":"MI 5",
            "type":"Smartphone"
         },
         "brand":{  
            "value":"Xioami",
            "type":"Smartphone"
         },
         "software":{  
            "value":"vN1.0_vC6",
            "type":"Version"
         },
         "library":{  
            "value":"23",
            "type":"Android API"
         }
      }
   },
   "sensor":{  
      "value":"Accelerometer",
      "type":"sensor-type",
      "metadata":{  
         "speed":{  
            "value":"60",
            "type":"hz"
         }
      }
   },
   "omh:end_date_time":{  
      "value":"2017-01-18T20:45:58.447Z-0800",
      "type":"omh:time-interval"
   },
   "omh:start_date_time":{  
      "value":"2017-01-18T20:45:42.697Z-0800",
      "type":"omh:time-interval"
   }
}
```
