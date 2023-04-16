# Service Orientation in Internet of Things (IoT) Domain: Use Cases, Benefits, and Challenges

## Overview

In our previous Hot Topic Study Journal, we explored numerous use cases and their respective benefits and challenges in the vast and complex domain of the Internet of Things (IoT). However, for the purposes of this case study, we will not delve into as many cases but rather concentrate on the service providers themselves and how their offerings are harnessed in the IoT systems.

It is pertinent to note that the two most prominent cloud service providers globally, Amazon Web Services (AWS) and Microsoft Azure, are at the forefront of providing IoT-related services. To this end, we aim to compare the concentration and diversity of their respective product offerings in the IoT field particularly. Not only will we scrutinize the Infrastructure as a Service (IaaS), Platform as a Service (PaaS), and Software as a Service (SaaS) suites for most of the use cases, we will also examine how these different service levels are applied to satisfy the demands of developing IoT systems.

## Introduction

IoT (Internet of Things) refers to the connection of various physical devices and objects to the internet, enabling them to perform smart and automated functions through the use of sensors, software, and networking technologies. IoT systems can be used for monitoring, controlling, data collection, automation, and more, and can be applied to various fields such as industry, healthcare, home automation, transportation, environmental protection, etc.

### General Components

IoT systems typically consist of the following components:

1. **Physical devices**: including various sensors, actuators, controllers, etc., used to sense and control various physical parameters in the real world.

2. **Network communication**: used to connect various physical devices and the internet, including wired and wireless networks, Bluetooth, WiFi, etc.

3. **Data processing and storage**: used to process and store data collected from physical devices, including various databases, cloud computing platforms, etc.

4. **Applications and services**: used to provide various functions and services, such as monitoring, control, automation, prediction, diagnosis, etc., which can be interacted with by users through web interfaces, mobile applications, etc.

When we utilize the service-oriented approach in the development of IoT systems, we should include the following aspects:

1. **Design scalable service interfaces**: each component of an IoT system should be designed and implemented as a service, with clear interfaces and functions, to facilitate composition and reuse.

2. **Implement service components**: each service interface should be implemented as a concrete component, which can use different programming languages and frameworks, but should ensure compatibility and interoperability between services.

3. **Deploy service components**: service components should be deployed on different devices and servers, which can use containerization technology and cloud computing platforms for deployment and management.

4. **Integrate service components**: service components should be integrated, which can use message queues, REST APIs, event-driven mechanisms, etc., to achieve integration and coordination of the IoT system's overall functionality.

5. **Provide applications and services**: various applications and services should be provided based on service components, such as web interfaces, mobile applications, APIs, etc., to allow users to interact with the IoT system conveniently.

### Utilization of Cloud Services

Cloud service providers typically offer three levels of services, IaaS (Infrastructure as a Service), PaaS (Platform as a Service), and SaaS (Software as a Service), which can be used in various ways for developing IoT systems.

- **IaaS**: With IaaS, the cloud service provider offers virtualized computing resources such as servers, storage, and networking infrastructure to developers. In IoT systems, IaaS can be used to deploy and manage the backend infrastructure, including data processing, storage, and network communication. IaaS can also be used to provide edge computing capabilities, which can enable IoT devices to perform computation and data processing at the edge of the network, closer to the data source, rather than sending all data to the cloud.

- **PaaS**: PaaS provides developers with a platform to develop, run, and manage applications without the need to manage the underlying infrastructure. PaaS can be used in IoT systems to develop and deploy middleware, software frameworks, and application logic that enable IoT devices to interact with each other and with the cloud. PaaS can also be used to develop and deploy analytics and machine learning models that can process and analyze the data collected by IoT devices.

- **SaaS**: SaaS provides end-users with access to applications and services over the internet, without the need for installation and maintenance. SaaS can be used in IoT systems to provide end-users with applications and services such as dashboards, analytics tools, and remote management capabilities. SaaS can also be used to provide end-users with access to IoT data and insights in real-time.

Regarding the use of cloud services in IoT systems, while most of the system components can be deployed and managed on the cloud, some components may need to be deployed on the physical devices themselves, such as sensors, actuators, and controllers. In this case, cloud services can still be used to manage and monitor these devices, but some aspects of their functionality may need to be implemented on the physical device itself. Additionally, for some IoT systems, the physical devices may need to communicate directly with each other, without going through the cloud, to achieve real-time responsiveness and reliability.

## Use Cases

As was previously discussed, it is worth noting that the responsibility of developing the IoT system rests solely with the end-users, who leverage the services offered by service providers for the purpose of backend infrastructure and services. In this particular section, we shall delve into the intricate details of the development and deployment of several IoT systems, with a particular focus on how the services offered by service providers are harnessed and utilized during the development phase.

### AWS

- [AWS IoT Core](https://aws.amazon.com/iot-core/?nc2=type_a)

  AWS IoT Core makes it simple and secure to connect devices to the cloud without needing to manage servers. It supports multiple communication protocols, including MQTT and HTTPS, and provides secure device connections and data with mutual authentication and end-to-end encryption. It also allows for real-time filtering, transformation, and action on device data based on defined business rules.

The utilization of AWS web service architecture provides essential components required for developing IoT applications. Belkin International's use case highlights the advantages of AWS IoT services in building IoT systems. By utilizing AWS IoT architecture, Belkin International was able to transform its in-house IoT system for the Wemo product line, resulting in cost savings, better system performance, and improved user experience for the connected products.

The primary focus of the overhaul was the deployment of AWS IoT Core, a robust platform that provides critical support services for scaling and expanding IoT systems. Although the specific service infrastructures used in the system were not provided, AWS IoT Core was certainly deployed.

For program deployment, securing, connecting, and managing the Wemo network of devices using a platform as a service (**PaaS**), Belkin International selected FreeRTOS as its Operating System. FreeRTOS extends the functionality of the open-source FreeRTOS kernel, allowing for secure and dependable connectivity between devices and Cloud Services such as AWS IoT Core.

Belkin International leveraged AWS IoT Core as its Software as a Service (**SaaS**) to establish secure interconnection between connected devices and other devices or Cloud applications. The combination of AWS IoT Core and FreeRTOS creates a potent IoT system that enables Belkin International to reduce costs, improve performance, and provide an advanced user experience for both its next-generation IoT devices and the millions of Wemo devices already in customers' homes.

Now, let's summarize the **benefits** of AWS IoT services in the development of IoT systems and the **challenges** before using these services in Belkin International's systems.

**Previous Challenges**:

- **Infrastructure Management**: Organizations needed to maintain their own data centers and manage the hardware, network, and storage infrastructure themselves.

- **High Costs**: Setting up and maintaining an on-premises data center is a costly affair. Organizations need to invest heavily in hardware, software, and manpower to manage their infrastructure.

- **Scalability**: Scaling up or down the infrastructure based on the changing demands of the business is a significant challenge. On-premises infrastructure cannot match the scalability offered by cloud providers like AWS.

- **Security**: Securing the infrastructure against cyber threats and data breaches is a major concern. Organizations need to invest in security tools and personnel to protect their data and infrastructure.

**Benefits**:

- **Cost Savings**: AWS provides a pay-as-you-go model, which means organizations only pay for the resources they use. This helps organizations reduce their capital and operational expenditures significantly.

- **Scalability**: AWS provides an elastic infrastructure that can scale up or down based on the changing needs of the business. This helps organizations handle peak workloads efficiently without incurring any downtime.

- **Infrastructure Management**: AWS takes care of infrastructure management, including hardware, software, and network infrastructure. This helps organizations focus on their core business operations rather than worrying about infrastructure management.

- **Security**: AWS offers a wide range of security services and tools that help organizations secure their data and infrastructure against cyber threats and data breaches. AWS is compliant with several industry standards and regulations, making it a reliable platform for organizations that deal with sensitive data.

### Microsoft Azure

- [Azure IoT Home](https://azure.microsoft.com/en-us/resources/iot/)

  Microsoft Azure IoT is a platform that provides resources for planning and implementing IoT solutions. It offers guidance on improving energy efficiency, productivity, and security, as well as insights into launching and managing successful IoT projects. It also provides resources on training, certifications, documentation, and events related to cloud computing, machine learning, and other topics.

The Smart Home Automation domain faced several challenges in on-boarding millions of IoT devices, multiple platforms for various IoT-enabled products, and backend solution's data security, reliability, and availability. The Azure IoT Smart Home solution overcame these challenges efficiently, providing efficient bi-directional communication, effective data management system, cost-effective solution, common backend IoT platform, and the support of any kind of Smart Home device. The proposed solution comes up with IaaS, PaaS, and SaaS, and is an exceptional platform for intelligent energy management, intelligent decision-making, and significant cost reductions.

**Challenges**:

- Difficulty on-boarding millions of IoT devices to the existing platform
- Need for a unique, common IoT platform to handle various types of smart devices
- High costs associated with maintaining different platforms for different IoT enabled products
- Data security, solution availability, and reliability concerns in the backend solution

**Benefits**:

- Bi-directional communication between Smart Home devices and Cloud has been established using Azure IoT Hub and Web Apps.
- Robust data management system using Azure Table Storage and SQL based data ingestion to store, handle, process, and analyze energy consumption data from multiple connected Smart Home Devices and customer data.
- Energy management and scheduling provision through a web portal powered by Azure Web Apps Service.
- Cost-effective IoT solution eliminating hosting and administration charges, offered free with Energy Management products.
- Common backend IoT platform that supports any kind of Smart Home device that the client offers.
- The platform can easily on-board millions of Smart home devices and analyze billions of data records for efficient energy management and intelligent decision-making.

The usage of IaaS, PaaS, and SaaS in this solution is as follows:

- **IaaS** (Infrastructure as a Service):

  - Azure Virtual Machines (VMs) are an example of IaaS in this solution. The client developed a VM-based backend platform to handle and control connected devices.

- **PaaS** (Platform as a Service):

  - Azure IoT Hub is an example of PaaS in this solution. It was used to establish a two-way communication between cloud and IoT-based Smart Home devices, and to set up bi-directional communication.
  - Azure Web Apps Service is also an example of PaaS in this solution. It was used to provide energy management and scheduling provision through a web portal.

- **SaaS** (Software as a Service):
  - There is no explicit mention of SaaS in this solution. However, the client does offer Energy Management products like Smart Surge Protector and Smart Wall Plug as a service, which could be considered a form of SaaS.

## Conclusion

After analyzing the IoT services of both Amazon Web Services (AWS) and Microsoft Azure, we can conclude that both are major providers in this domain. These platforms offer Infrastructure as a Service (IaaS), Platform as a Service (PaaS), and Software as a Service (SaaS) suites. However, there are some differences between them.

AWS IoT core offers a simplified approach to connecting devices to the cloud by eliminating the need for server management; it supports multiple communication protocols, provides secure device connections and data, and offers cost-efficient solutions. Meanwhile, Microsoft Azure IoT provides resources for planning and implementing IoT solutions; it provides guidance on launching and managing successful projects, offers smart home automation solutions which facilitate effective communication, data management, and energy scheduling through a web portal.

Considering the above points, both providers have their unique strengths, and the choice of provider may vary based on the projects.

## References

- [AWS IoT - Belkin Rebuilds Wemo Operations on AWS IoT](https://aws.amazon.com/solutions/case-studies/belkin-case-study/?pg=ln&sec=c)
- [Azure IoT - Achieving More with Connected Products](https://azure.microsoft.com/en-us/resources/achieving-more-with-connected-products/)
