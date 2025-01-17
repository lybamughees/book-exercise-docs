# Gateway Device Application (Connected Devices)

## Lab Module 10

Be sure to implement all the PIOT-GDA-* issues (requirements) listed at [PIOT-INF-10-001 - Lab Module 10](https://github.com/orgs/programming-the-iot/projects/1#column-10488510).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

**What does your implementation do?**

The implementation focuses on the integration of Edge Tier applications, namely the CDA and GDA, in an IoT ecosystem using CoAP and MQTT protocols. A significant emphasis is placed on enhancing security by enabling TLS encryption for MQTT communication between the applications, ensuring the secure exchange of messages. The implementation provides detailed programming exercises for configuring TLS in the MQTT broker (Mosquitto) and modifying the MqttClientConnector class in both the CDA and GDA to support encrypted connections. It also addresses credential management and highlights the importance of secure practices in handling private keys. Overall, the implementation aims to establish a secure and robust communication framework within the Edge Tier of the IoT ecosystem.

**How does your implementation work?**

The implementation facilitates the integration of Edge Tier applications (CDA and GDA) in an IoT ecosystem using CoAP and MQTT protocols. A key emphasis is on security, with a focus on enabling TLS encryption for MQTT connections between CDA and GDA. The process involves configuring the Mosquitto broker to support TLS, loading credentials securely, and modifying the MqttClientConnector class in both applications. The modifications include SSL socket factory initialization and configuring the MQTT client connection for encryption. The implementation ensures secure communication between the applications, with the flexibility to adapt to different environments and cloud services.


### Code Repository and Branch

NOTE: Be sure to include the branch (e.g. https://github.com/programming-the-iot/python-components/tree/alpha001).

URL: https://github.com/lybamughees/piot-java-components/tree/labmodule10

### UML Design Diagram(s)

NOTE: Include one or more UML designs representing your solution. It's expected each
diagram you provide will look similar to, but not the same as, its counterpart in the
book [Programming the IoT](https://learning.oreilly.com/library/view/programming-the-internet/9781492081401/).


### Unit Tests Executed

NOTE: TA's will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.


### Integration Tests Executed

NOTE: TA's will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- testConnectAndDisconnect

<img width="384" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/4ca4a189-8cc0-45f9-ad6d-0ccc2c31bb2f">

- testPublishQoS1()

  <img width="400" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/322a9468-8d1e-4b1d-b03e-52dbd72ea1cd">

- testPublishQoS2()

  <img width="386" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/55d85c6c-f720-47cc-91f1-6a448a04cc95">

- testPublishQoS0()

  <img width="439" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/afc3ccf5-6205-4394-ab29-e45b38e23420">

- MqttClientConnectorTest

  <img width="550" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/71513122-16a0-4e40-8573-e1a7890b1df1">

- testActuatorCommandResponseSubscription()

  <img width="342" alt="image" src="https://github.com/lybamughees/book-exercise-docs/assets/66569488/8e718938-4ade-4444-a12f-8ef1f517e043">

  


EOF.
