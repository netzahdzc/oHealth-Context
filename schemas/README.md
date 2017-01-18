# Schema library (v 1.0)

This schema represents a mechanism to package sensor data collected from mobile devices worn by a user while performing one of either physical test (i.e., Timed Up and Go, 30-Second Chair Stand, 4-Stage Balance Test).

## General use
* [PHYSICAL TEST](https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/entity/physical-test-1.x.json)
* [TEST TYPE](https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/dataType/test-type-1.x.json)
* [SENSOR TYPE](https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/dataType/sensor-type-1.x.json)
* [SENSOR SPEED](https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/dataType/sensor-speed-1.x.json)
* [SENSOR DATA](https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/dataType/sensor-data-1.x.json)
* [TIME INTERVAL](https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/dataType/time-interval-1.x.json)

## Specific purpose (Physical test)
### Test: Timed Up and Go 
Below we present the schemas that correspond to the variables of interest required for each physical test. 
* [Step count](https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/dataType/step-count-1.x.json)
* [Walk speed](https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/dataType/walk-speed-1.x.json)
* [Distance between steps](https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/dataType/step-distance-1.x.json)
* [Distance unit value](https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/dataType/distance-unit-1.x.json)
* [Time between steps](https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/dataType/latency-1.x.json)

### Test: 30-Second Chair Stand Test
* [Number of repetitions](https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/dataType/repetitions-1.x.json)
* [Time between repetitions](https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/dataType/latency-1.x.json)

### Test: 4-Stage Balance Test
* [Interval of time that last the test] (https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/duration-unit-value-1.x.json)
* [Balance index](https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/dataType/balance-index-1.x.json)

Please refer to the [specification section](./spec.md) for detailed information.
