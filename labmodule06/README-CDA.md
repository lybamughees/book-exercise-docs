# Constrained Device Application (Connected Devices)

## Lab Module 06

Be sure to implement all the PIOT-CDA-* issues (requirements) listed at [PIOT-INF-06-001 - Lab Module 06](https://github.com/orgs/programming-the-iot/projects/1#column-10488434).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

The implementation builds pub/sub communications capability into the CDA using MQTT, which allows it to publish messages to an MQTT broker and receive updates based on its topic-level subscriptions.

How does your implementation work?

- Updates CDA with MQTT client
- Client connects to MQTT broker
- Uses topic-level subscriptions for updates
- Adds MQTT client abstraction layer to CDA

### Code Repository and Branch

NOTE: Be sure to include the branch (e.g. https://github.com/programming-the-iot/python-components/tree/alpha001).

URL: https://github.com/madlitch/python-components/tree/default

### UML Design Diagram(s)

NOTE: Include one or more UML designs representing your solution. It's expected each
diagram you provide will look similar to, but not the same as, its counterpart in the
book [Programming the IoT](https://learning.oreilly.com/library/view/programming-the-internet/9781492081401/).

![CleanShot 2023-10-27 at 12 21 30@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/cdb3e62f-5876-4bf8-959d-9216de5ed2d1)


### Unit Tests Executed

NOTE: TA's will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

N/A

### Integration Tests Executed

NOTE: TA's will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- MqttClientConnectorTest
![CleanShot 2023-10-27 at 11 15 42@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/4777a8ba-1211-4f57-8134-74b37449b941)
![CleanShot 2023-10-27 at 11 15 48@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/dfbd27c9-8eba-478b-ab1a-06f54b861922)

- testConnectandDisconnect
![CleanShot 2023-10-27 at 11 46 22@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/519f2088-5737-49a2-8ee9-a976c105038c)

- testConnectAndCDAManagementStatusPubSub
![CleanShot 2023-10-27 at 11 49 58@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/03f1e577-fb19-4dda-a708-fa77b2775abd)

- testActuatorCmdPubSub
![CleanShot 2023-10-27 at 11 56 08@2x](https://github.com/lybamughees/book-exercise-docs/assets/33076159/94efa17e-1e67-4ed8-bb45-1f89ab65520b)

EOF.
