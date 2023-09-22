# Constrained Device Application (Connected Devices)

## Lab Module 02

Be sure to implement all the PIOT-CDA-* issues (requirements) listed at [PIOT-INF-02-001 - Lab Module 02](https://github.com/orgs/programming-the-iot/projects/1#column-9974938).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

This module serves to implement performance monitoring for our CDA at regular intervals, and log it using the system logger. It is built off of the architecture worked in the previous module.

How does your implementation work?

We have implemented a wrapper and multiple modules that serve to monitor specific performance data characteristics. For example, the SystemPerformanceManager module is responsible for all system performance data, in which it collects through the SystemCpuUtilTask and the SystemMemUtilTask modules. 

### Code Repository and Branch

URL: https://github.com/madlitch/python-components/tree/labmodule02

### UML Design Diagram(s)

![image](https://github.com/lybamughees/book-exercise-docs/assets/33076159/a3c84dda-d815-4673-a39c-b3bb2d34e0bf)


### Unit Tests Executed

NOTE: TA's will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- ConfigUtilTest
![CleanShot 2023-09-22 at 11 50 49@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/b09384ae-9fa9-4ec9-bcd1-85e7dd6bdfe8)

- SystemCpuUtilTaskTest
![CleanShot 2023-09-22 at 11 55 58@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/b3f4ee2b-bca4-4b05-9688-ef4440c30a59)

- SystemMemUtilTaskTest
![CleanShot 2023-09-22 at 11 56 35@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/396ffead-eec6-4ade-bfe8-af2b7c9296a7)


### Integration Tests Executed

NOTE: TA's will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- ConstrainedDeviceAppTest
![CleanShot 2023-09-22 at 11 49 35@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/ba75fc68-a028-4824-b079-5f01e3277e87)

- SystemPerformanceManagerTest (Excerpt)
![CleanShot 2023-09-22 at 11 54 23@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/022ca979-7c02-455a-baa4-ca4cdfc95a11)


EOF.
