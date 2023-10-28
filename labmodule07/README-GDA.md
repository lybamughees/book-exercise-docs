# Gateway Device Application (Connected Devices)

## Lab Module 07

Be sure to implement all the PIOT-GDA-* issues (requirements) listed at [PIOT-INF-07-001 - Lab Module 07](https://github.com/orgs/programming-the-iot/projects/1#column-10488499).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 


My implementation focuses on building MQTT client connection logic within the Gateway Device Application (GDA). This GDA will eventually serve as the bridge between Constrained Device Applications (CDA) and remote cloud services, using MQTT for communication.


How does your implementation work?

My implementation involves integrating MQTT (Message Queuing Telemetry Transport) into the Gateway Device Application (GDA) for handling communication with Constrained Device Applications (CDAs) and potentially remote cloud services. Overall, my implementation enables my GDA to communicate with CDAs and remote cloud services using MQTT. It follows the MQTT publish-subscribe pattern, where messages are published to topics and subscribed to by interested clients. The MqttClientConnector component plays a crucial role in establishing and managing these MQTT connections. This integration allows for reliable, two-way communication in the context of the Internet of Things (IoT).

### Code Repository and Branch

NOTE: Be sure to include the branch (e.g. https://github.com/programming-the-iot/python-components/tree/alpha001).

URL: https://github.com/lybamughees/piot-java-components/tree/labmodule07

### UML Design Diagram(s)

NOTE: Include one or more UML designs representing your solution. It's expected each
diagram you provide will look similar to, but not the same as, its counterpart in the
book [Programming the IoT](https://learning.oreilly.com/library/view/programming-the-internet/9781492081401/).


### Unit Tests Executed

NOTE: TA's will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- 
- 
- 

### Integration Tests Executed

NOTE: TA's will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- 
- 
- 

EOF.
