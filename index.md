---
title: About Section
feature_text: |
  ## MusQraTT
  An MQTT-SN Broker in Rust on Composite OS
feature_image: "https://picsum.photos/1300/400?image=989"
---

<p>
  MQTT-SN is a publisher-subscriber communication protocol designed primarily for Internet of Things (IoT) and cyber-physical systems. These can vary from smart home hubs and smart refrigerators to smart vehicles in smart cities, sensor networks, and even has some aerospace implications.
</p>

<p>
  Today, computational workloads for these cyber-physical systems and IoT devices are becoming increasingly sensitive to latency, a time measurement of delay for network communications. For mission critical applications, this could be a difference in avoiding a collision for autonomous vehicles or precise motion control for industrial equipment. 
</p>

<p>
  The current industry standard for MQTT/MQTT-SN is Mosquitto. Some larger technology companies also have their own implementations for their smart devices, such as Amazon AWS and Microsoft Azure. These are provide support for C, Java, and Javascript programming languages. However, those runtimes are too memory intensive and not suitable for real-time systems. In addition, the future of these IoT and cyber-physical systems is moving towards the Edge of the network; Mosquitto, Microsoft, and Amazon do not provide Edge support <em>and</em> have higher transmission latencies. 
</p>

<p>
  Our project is <strong>MusQraTT</strong>, a MQTT-SN broker built in Rust ported to CompositeOS. By building the Broker in Rust, we ensure the guaranteed memory safety from the language, and Rust has a reduced runtime. CompositeOS, a research operating system built at GW, provides segmented memory and resources, allowing for our broker to handle more clients.
</p>

### Features

* <em>performance metrics</em>
* Support for UDP clients
* Increases speed by handling client requests with threading
* Can handle over 65k clients