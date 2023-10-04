# Gateway Device Application (Connected Devices)

## Lab Module 05

Be sure to implement all the PIOT-GDA-* issues (requirements) listed at [PIOT-INF-05-001 - Lab Module 05](https://github.com/orgs/programming-the-iot/projects/1#column-10488421).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

**What does your implementation do?**

I am implementing the ability for the GDA to store and retrieve data locally on the device. This allows the GDA to keep a history of sensor data, system performance data, or any other relevant information, even when there is no internet connectivity. Later, you can use this stored data for analysis or decision-making. The GDA will have the capability to store and retrieve data locally, enhancing its ability to operate effectively in scenarios with limited or intermittent network connectivity.

**How does your implementation work?**

The local data persistence functionality provides the GDA with the capability to store incoming data locally on the device. This is particularly useful in scenarios with limited or intermittent network connectivity. The stored data can be retrieved and analyzed later, enabling the GDA to make decisions or perform analysis even when it's not connected to the internet. By implementing local data persistence, the GDA gains resilience and the ability to work effectively in situations where continuous internet connectivity may not be available.
### Code Repository and Branch

NOTE: Be sure to include the branch (e.g. https://github.com/programming-the-iot/python-components/tree/alpha001).

URL: https://github.com/lybamughees/piot-java-components/tree/labmodule05

### UML Design Diagram(s)

<img width="558" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/2d501353-1ee0-4a24-bbbe-ff53e647404d">


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
  
EOF.
