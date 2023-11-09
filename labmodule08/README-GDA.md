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

URL: https://github.com/lybamughees/piot-java-components/tree/labmodule08

### UML Design Diagram(s)

<img width="554" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/64dbb32d-04e3-4528-97da-b5ca570bce34">


NOTE: Include one or more UML designs representing your solution. It's expected each
diagram you provide will look similar to, but not the same as, its counterpart in the
book [Programming the IoT](https://learning.oreilly.com/library/view/programming-the-internet/9781492081401/).


### Unit Tests Executed

NOTE: TA's will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- ConfigUtilTest
  
<img width="733" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/c26452dd-3805-4c6e-9299-6921c87e2503">

- SystemMemUtilTaskTest
  
  <img width="670" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/73d05108-a319-40d2-82dd-57885cbe47f1">
  
- SystemCpuUtilTaskTest
  
  <img width="704" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/a4d46d1f-4cd8-4383-986c-6d96903ac534">
  
- ActuatorDataTest
  
  <img width="585" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/faf101b0-31d9-4834-9a0d-3a7e71bc2edc">
  
- BaseIotDataTest
  
  <img width="598" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/1194d551-81b4-4117-9e48-d66a8a3ec309">
  
- DataUtilTest
  
  <img width="579" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/c1a69781-03ff-456c-9ff1-5e3ee2b244d9">
  
- SensorDataTest
  
  <img width="722" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/52b92023-fc39-4ba9-ab53-3657361f245a">
  
- SystemPerformanceDataTest
  
  <img width="718" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/cb50cf32-5005-4bc2-818b-10241836f9e4">

### Integration Tests Executed
  
NOTE: TA's will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- GatewayDeviceAppTest
  
  <img width="584" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/ce865771-39e1-43b7-9d21-f50539a05307">
  
- SystemPerformanceManagerTest
  
  <img width="602" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/c84dd343-725e-4f8e-bd18-4a63879c44d8">
  
- DeviceDataManagerNoCommsTest
  
  <img width="509" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/44bc4118-26b4-4bf4-8b7f-f15e93d881b6">
  
- DataIntegrationTest
  
  ![image](https://github.com/lybamughees/book-exercise-docs/assets/66569488/b6c2b0f1-0795-4da1-ba99-5208ccadb259)

- MqttClientConnectorTest
  


  <img width="661" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/b0548501-ebf2-4f5a-b68f-bbad633d990d">
<img width="675" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/70d17685-032d-4ce2-a2a7-50de16bc3c9d">
<img width="623" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/ad20954c-540e-4ec7-9139-edace5e215ca">
EOF.
