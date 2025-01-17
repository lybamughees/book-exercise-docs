# Gateway Device Application (Connected Devices)

## Lab Module 02

Be sure to implement all the PIOT-GDA-* issues (requirements) listed at [PIOT-INF-02-001 - Lab Module 02](https://github.com/orgs/programming-the-iot/projects/1#column-9974938).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

**What does your implementation do?**

The implementation is of a Gateway Device Application (GDA) for an IoT system. The GDA is part of the IoT Edge Tier and is responsible for collecting system performance data and potentially other telemetry from IoT devices. The GDA collects system performance telemetry, including metrics like CPU and memory utilization. It may also collect additional telemetry data related to network utilization and disk utilization. While the CDA (Constrained Device Application) generates its specific system performance telemetry and sensor-specific telemetry, the GDA processes data from the CDA and sends both its own telemetry and the CDA's telemetry to the cloud for further processing. The GDA uses Java's concurrency library to manage tasks that collect telemetry data at regular intervals. The implementation includes unit tests for various components to ensure they work as expected. The implementation uses logging to record information about the application's initialization, start, stop, and telemetry data. Overall, the GDA is a central component in an IoT system, responsible for collecting and managing system performance data and potentially other telemetry, which can be later processed and sent to the cloud for further analysis.


**How does your implementation work?**

The GDA's entry point is the `GatewayDeviceApp` class. During initialization, the GDA reads configuration settings, including the polling rate for collecting telemetry data, from a configuration file. The `SystemPerformanceManager` is responsible for managing the collection of system performance data. It creates instances of `SystemCpuUtilTask` and `SystemMemUtilTask`, which are responsible for collecting CPU and memory utilization data. The manager sets up a scheduled task using Java's concurrency library (`ScheduledExecutorService`) to run at regular intervals (defined by the polling rate). At each interval, the scheduled task calls the `handleTelemetry()` method in the manager. The `SystemCpuUtilTask` and `SystemMemUtilTask` classes are responsible for collecting CPU and memory utilization data, respectively. They use platform-specific APIs or libraries to retrieve system performance metrics. The collected data is then logged, and the telemetry values are made available to the manager. The `handleTelemetry()` method in the `SystemPerformanceManager` is called at regular intervals. It retrieves telemetry data from the `SystemCpuUtilTask` and `SystemMemUtilTask`. The telemetry data, including CPU and memory utilization values, is logged for monitoring purposes. The GDA application logs various messages, including initialization, start, and stop events, as well as telemetry data. When the GDA application is stopped, it shuts down the `ScheduledExecutorService`, which stops the scheduled telemetry collection task.


### Code Repository and Branch

NOTE: Be sure to include the branch (e.g. https://github.com/programming-the-iot/python-components/tree/alpha001).

URL: https://github.com/lybamughees/piot-java-components/tree/labmodule02

### UML Design Diagram(s)

NOTE: Include one or more UML designs representing your solution. It's expected each
diagram you provide will look similar to, but not the same as, its counterpart in the
book [Programming the IoT](https://learning.oreilly.com/library/view/programming-the-internet/9781492081401/).

<img width="666" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/c15ada76-f403-4f9c-a1d8-b205e3ecd347">

### Unit Tests Executed

NOTE: TA's will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- ConfigUtilTest
- <img width="645" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/0ef62500-e512-4928-b528-56280b449d70">

  - SystemMemUtilTaskTest
  - <img width="645" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/3bc1e4b7-47a2-4a36-86e1-045f6eb01588">

- SystemCpuUtilTaskTest
- <img width="651" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/e0d0d727-bd7c-43a5-bec2-e21f6732422d">

### Integration Tests Executed

NOTE: TA's will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- SystemPerformanceManagerTest
- <img width="635" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/98f58ba7-2dce-4a63-8a7d-1e4e251a00c2">

- GatewayDeviceAppTest
- <img width="624" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/2dd8b834-0c21-4248-bb6c-43b11ad5f6a1">

EOF.
