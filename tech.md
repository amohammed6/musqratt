---
title: MusQraTT Technology
feature_text: |
  ## MusQraTT
  An MQTT Broker in Rust on Composite OS
feature_image: "https://picsum.photos/1300/400?image=989"
---

## Composite OS
<p>
MusQraTT is built on the Composite kernel, a microkernel developed for secure and high-performance systems. Using Composite allows us to make key system optimizations that enable MusQraTT to be highly performant, and take advantage of years of research into OS design. Composite is being developed at the GW Embedded and Operating Systems Lab.
</p>

## Rust Programming Language

<p>
Using Rust programming languages has three main benefits that assist our Broker:
</p>

* <strong>Safer</strong> due to the Rust's compiler and type-system
* <strong>Faster</strong> due to it's lack of a garbage collector
* Allows for more <strong>concurrency</strong> to handle more clients

## MQTT-SN Rust Crate

<p>
We utilized a Rust Crate, known as <a href="https://crates.io/crates/mqtt-sn">"mqtt-sn"</a>. This crate provides the support and requirements for an MQTT-SN system. It included the packet specifications (packet id, topic subcription, etc) as well as the functionality for encoding, decoding, and parsing the packet. This made it possible for the packets, encoded in bytes, to be sent into a UDP socket.
</p>
