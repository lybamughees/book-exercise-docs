# Constrained Device Application (Connected Devices)

## Lab Module 09

Be sure to implement all the PIOT-CDA-* issues (requirements) listed at [PIOT-INF-09-001 - Lab Module 09](https://github.com/orgs/programming-the-iot/projects/1#column-10488503).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

**What does your implementation do?**

In this implementation, I've examined a Java class named CoapClientConnector. The class serves as a CoAP (Constrained Application Protocol) client connector, providing functionality to send various CoAP requests (GET, POST, PUT, DELETE) to a specified server and handle the corresponding responses. It also supports CoAP discovery requests to retrieve information about available resources on the server. One notable feature is the ability to observe resources, allowing the client to receive updates when the observed resource changes. The implementation utilizes the Californium CoAP library providing a flexible and modifiable shell for CoAP communication. The class structure includes methods for initializing the client, sending different types of requests, handling responses, and managing resource observation. Additionally, the class incorporates logging and exception handling to improve robustness.

**How does your implementation work?**

In my implementation, the `CoapClientConnector` class is designed to establish and manage CoAP communication with a specified server. Upon instantiation, the class initializes its parameters such as the server's host, port, and protocol based on configuration data. The `initClient` method sets up the CoAP client connection with the configured server address. The class offers methods to send CoAP requests for resource discovery, retrieval (GET), creation (POST), update (PUT), and deletion (DELETE). It dynamically adjusts the CoAP communication mode based on whether Confirmable (CON) or Non-confirmable (NON) messages are enabled. The implementation includes a mechanism to observe resources, enabling the client to receive updates when the observed resource changes. This is facilitated by a CoAP observer relation and a custom handler (`SensorDataObserverHandler`) that processes received responses, logging them and potentially notifying a data message listener. Overall, the implementation is modular, logging is used for informative purposes and potential debugging.

### Code Repository and Branch

NOTE: Be sure to include the branch (e.g. https://github.com/programming-the-iot/python-components/tree/alpha001).

URL: https://github.com/lybamughees/piot-java-components/tree/labmodule09

### UML Design Diagram(s)
<img width="713" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/3eb17629-53a6-4fcb-904b-630bbe1fbd27">

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

- CoapServerGatewayTest

  <img width="1091" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/ca20b663-3f51-4868-8580-abc4c6de46d6">
  <img width="1075" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/d8257dca-164d-450b-8396-b60441e7688c">

- testConnectAndDiscover
  
 <img width="759" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/9ff8c5ca-0828-418f-a398-15a162815393">

- testObserve

 <img width="730" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/4afd6112-a3d3-4e1b-8029-b06c3a312da7">


- testGetRequestCon

<img width="722" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/11ca897a-983a-46fb-bbdd-4494385085a4">

- testGetRequestNon

<img width="733" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/e3f3fc6a-5f24-429f-86fe-ee417fa5738e">

- testPutRequestNon

  <img width="731" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/2dad108a-141f-4159-ad49-d3f71ee69a19">


- testPostRequestCon

  <img width="725" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/48d289ff-b1d1-4538-87d5-5a2c410e734b">

- testPostRequestNon

  <img width="724" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/13e41c9e-3567-4a79-a921-807b04bd55c8">

- testPutRequestCon

  <img width="732" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/8efb8e7d-39c6-41d9-abbc-6618adbdfa54">


- testDeleteRequestCon

  <img width="731" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/11bd2393-244a-4ac8-baf1-c8e3041fb4dc">

- testDeleteRequestNon

  <img width="735" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/c7457681-870d-475e-9c97-496e8ce63e5f">







EOF.
