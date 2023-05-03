---
title: MusQraTT Results
feature_text: |
  ## MusQraTT
  An MQTT Broker in Rust on Composite OS
feature_image: "https://picsum.photos/1300/400?image=989"
---

<figure>
  <img src="https://github.com/amohammed6/musqratt/raw/main/docs/latencyImage.png" alt="Latency Image" style="width:80%">
  <figcaption>This graph displays the average transmission latency performance as the number of publishers and subscribers increases in a system. Musquitto and it's MQTT-SN gateway perform exponentially slower as more clients connect, while our MusQraTT broker remains with consisten low transmission latency.</figcaption>
</figure>

<p>
Click here to view the code behind our project: <a href = "https://github.com/amohammed6/composite_mqtt">GitHub Link</a>
</p>

### Performance Videos
<p>
In a smart city, an intersection may have a number of collision detection sensors that communicate with self-driving vehicles. If a car were to suddenly enter the intersection, the sensor should be able to communicate to surrounding vehicles quickly enough to notify them not to proceed.
</p>

<p>
We've created a mock scenario like this with two vehicles entering an intersection, one unexpectedly. Watch what happens when the "STOP" message is sent using the industry standard Musquitto versus our MQTT-SN broker MusQraTT.
</p>

#### Mosquitto + Gateway 
<br>
<video src="https://github.com/amohammed6/musqratt/raw/main/docs/mosquitto.mov" controls="controls" style="max-width: 400px;">
</video>

#### MusQraTT
<br>
<video src="https://github.com/amohammed6/musqratt/raw/main/docs/musqratt.mov" controls="controls" style="max-width: 400px;">
</video>