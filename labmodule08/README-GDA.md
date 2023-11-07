# Gateway Device Application (Connected Devices)

## Lab Module 08

Be sure to implement all the PIOT-GDA-* issues (requirements) listed at [PIOT-INF-08-001 - Lab Module 08](https://github.com/orgs/programming-the-iot/projects/1#column-10488501).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

In my implementation, I've developed a CoAP (Constrained Application Protocol) server as part of my Gateway Device Application (GDA) within my IoT system. This CoAP server enables my gateway device to interact with other devices within the IoT ecosystem by using the CoAP protocol. I've integrated resource management into the server, allowing me to represent different IoT resources, like sensors and actuators, through unique URL-like paths. For each type of resource, I've defined resource handlers that dictate how the server should respond to various CoAP request methods. The server effectively manages CoAP messaging formats, which are optimized for efficient communication between devices in resource-constrained environments. Additionally, I've ensured error handling, testing, and integration to guarantee that the CoAP server operates seamlessly, facilitating communication between my GDA and other devices through CoAP. This implementation plays a pivotal role in supporting data exchange and command execution in my IoT architecture alongside other communication protocols like MQTT.

How does your implementation work?

My implementation works by integrating a CoAP (Constrained Application Protocol) server into my Gateway Device Application (GDA) within my Internet of Things (IoT) system. This CoAP server serves as a pivotal link, enabling my gateway device to engage with other devices across the IoT network using the CoAP protocol. Within the server, I've set up resource handlers that define how the server should respond to different CoAP request methods like GET, PUT, POST, and DELETE. These resource handlers manage specific resources, such as sensors and actuators, represented by unique URL-like paths. This setup empowers my GDA to efficiently retrieve sensor data and dispatch actuator commands. The CoAP server efficiently handles the binary message format used for communication in resource-constrained environments. Moreover, I've implemented robust error handling, comprehensive testing, and seamless integration to ensure the server operates flawlessly. As a result, it facilitates smooth data exchange and command execution between my GDA and other devices, complementing the functionality of other communication protocols like MQTT within my IoT architecture.

### Code Repository and Branch

NOTE: Be sure to include the branch (e.g. https://github.com/programming-the-iot/python-components/tree/alpha001).

URL: 

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
