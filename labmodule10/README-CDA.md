# Constrained Device Application (Connected Devices)

## Lab Module 10

Be sure to implement all the PIOT-CDA-* issues (requirements) listed at [PIOT-INF-10-001 - Lab Module 10](https://github.com/orgs/programming-the-iot/projects/1#column-10488510).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

**What does your implementation do?**

The implementation focuses on the integration of Edge Tier applications, namely the CDA and GDA, in an IoT ecosystem using CoAP and MQTT protocols. A significant emphasis is placed on enhancing security by enabling TLS encryption for MQTT communication between the applications, ensuring the secure exchange of messages. The implementation provides detailed programming exercises for configuring TLS in the MQTT broker (Mosquitto) and modifying the MqttClientConnector class in both the CDA and GDA to support encrypted connections. It also addresses credential management and highlights the importance of secure practices in handling private keys. Overall, the implementation aims to establish a secure and robust communication framework within the Edge Tier of the IoT ecosystem.

**How does your implementation work?**

The implementation facilitates the integration of Edge Tier applications (CDA and GDA) in an IoT ecosystem using CoAP and MQTT protocols. A key emphasis is on security, with a focus on enabling TLS encryption for MQTT connections between CDA and GDA. The process involves configuring the Mosquitto broker to support TLS, loading credentials securely, and modifying the MqttClientConnector class in both applications. The modifications include SSL socket factory initialization and configuring the MQTT client connection for encryption. The implementation ensures secure communication between the applications, with the flexibility to adapt to different environments and cloud services.

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
