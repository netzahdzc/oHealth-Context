# Schema library (v 1.0)

This schema represents a mechanism to package sensor data collected from mobile devices worn by a user while performing one of either physical test (i.e., Timed Up and Go, 30-Second Chair Stand, 4-Stage Balance Test).

## General use
* [PHYSICAL TEST](oHealth-Context/schemas/physical-test.1.x.json)
* [TEST TYPE](oHealth-Context/schemas/test-type.1.x.json)
* [SENSOR TYPE](oHealth-Context/schemas/sensor-type.1.x.json)
* [SENSOR SPEED](oHealth-Context/schemas/sensor-speed.1.x.json)
* [SENSOR DATA](oHealth-Context/schemas/sensor-data.1.x.json)
* [TIME INTERVAL](oHealth-Context/schemas/time-interval.1.x.json)

## Specific purpose (Physical test)
### Test: Timed Up and Go 
Below we present the schemas that correspond to the variables of interest required for each physical test. 
* [Step count](oHealth-Context/schemas/step-count.1.x.json)
* [Walk speed](oHealth-Context/schemas/walk-speed.1.x.json)
* [Distance between steps](oHealth-Context/schemas/step-distance1.x.json)
* [Distance unit value](oHealth-Context/schemas/distance-unit.1.x.json)
* [Time between steps](oHealth-Context/schemas/latency.1.x.json)

### Test: 30-Second Chair Stand Test
* [Number of repetitions](oHealth-Context/schemas/repetitions.1.x.json)
* [Time between repetitions](oHealth-Context/schemas/latency.1.x.json)

### Test: 4-Stage Balance Test
* [Interval of time that last the test] (oHealth-Context/schemas/duration-unit-value.1.x.json)
* [Balance index](oHealth-Context/schemas/balance-index.1.x.json)

