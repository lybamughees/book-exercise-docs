# Constrained Device Application (Connected Devices)

## Lab Module 05

Be sure to implement all the PIOT-CDA-* issues (requirements) listed at [PIOT-INF-05-001 - Lab Module 05](https://github.com/orgs/programming-the-iot/projects/1#column-10488421).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

The implementation describes how to convert data objects, such as ActuatorData, SensorData, and SystemPerformanceData, to and from JSON format using a DataUtil class. The ActuatorDataToJson function converts an ActuatorData object to a JSON string, while the jsonToActuatorData function reverses the process by converting a JSON string back to an ActuatorData object. These functions ensure that data can be easily exchanged between components in an IoT system by converting it to a common JSON format. Similar conversion functions can be implemented for other data types, allowing for seamless data communication within the system.

How does your implementation work?

The implementation enables the conversion of custom data objects, such as ActuatorData, SensorData, and SystemPerformanceData, to JSON format and vice versa. When converting to JSON, the system uses a private function to create a JSON representation of the data object's attributes and values, ensuring compatibility through a custom JSON encoder. When converting from JSON, the system parses the JSON input, extracts key-value pairs, and constructs a new data object instance, updating its attributes with values from the JSON data. This functionality streamlines data exchange in an IoT ecosystem, promoting seamless communication and interoperability among various components.
### Code Repository and Branch

NOTE: Be sure to include the branch (e.g. https://github.com/programming-the-iot/python-components/tree/alpha001).

URL: https://github.com/madlitch/python-components/tree/labmodule05

### UML Design Diagram(s)

NOTE: Include one or more UML designs representing your solution. It's expected each
diagram you provide will look similar to, but not the same as, its counterpart in the
book [Programming the IoT](https://learning.oreilly.com/library/view/programming-the-internet/9781492081401/).

<img width="759" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/2d928006-8928-483f-8321-080e46dfe2e3">


### Unit Tests Executed

NOTE: TA's will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- DataUtilTest
![CleanShot 2023-10-06 at 20 13 39@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/13e26c85-7a4e-4327-8f95-d3d22d47cbdc)
- ActuatorDataTest
  ![CleanShot 2023-09-29 at 16 34 19@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/b1d1a46c-2190-40ca-ac72-1154d8b74a78)

- SensorDataTest
![CleanShot 2023-09-29 at 16 34 49@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/038beb01-9db3-4a85-9a2a-e7305c96fa76)

- SystemPerformanceDataTest
![CleanShot 2023-09-29 at 16 35 17@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/58b04452-493d-440b-a19e-97581390f9b4)

- HumiditySensorSimTaskTest
![CleanShot 2023-09-29 at 16 46 04@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/b36f17cb-3d22-4e49-8869-65edae277b9d)

- PressureSensorSimTaskTest
![CleanShot 2023-09-29 at 16 48 19@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/2d280d2f-3634-4086-90cf-d0bc652b0c58)

- TemperatureSensorSimTaskTest
![CleanShot 2023-09-29 at 16 48 41@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/6ec5b873-399d-414f-bd9b-38465017fc23)

- HumidifierActuatorSimTaskTest
![CleanShot 2023-09-29 at 17 00 06@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/3b4a8117-92dd-4844-bf3d-bf8ca6b47885)

- HvacActuatorSimTask
![CleanShot 2023-09-29 at 17 00 54@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/ed554f9e-a38b-460c-903c-d33312ef7629)


### Integration Tests Executed

NOTE: TA's will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- SystemPerformanceManagerTest
![CleanShot 2023-10-06 at 20 15 57@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/ecb2ab92-d32e-466a-ad58-3be273b1d2a6)
- SensorAdapterManagerTest
![CleanShot 2023-09-29 at 17 08 47@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/51ce99de-317e-4da9-816a-8adbbb7ecd02)

- ActuatorAdapterManagerTest
![CleanShot 2023-09-29 at 17 11 22@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/b16a619d-55fe-4e46-80fb-bd49ef5478dc)

- DeviceDataManagerNoCommsTest
![CleanShot 2023-09-29 at 17 24 32@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/e204ddc9-9563-429b-af75-5f4b8ca39952)

- ConstrainedDeviceAppTest
![CleanShot 2023-09-29 at 17 26 25@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/48a22b91-4acb-4608-aa0a-5a67d19d1b7f)

-DataIntegrationTest
![image](https://github.com/lybamughees/book-exercise-docs/assets/66569488/35b1e099-7577-4930-b04c-452227381431)




EOF.
