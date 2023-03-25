---
title: MusQraTT Technology
feature_text: |
  ## MusQraTT
  An MQTT Broker in Rust on Composite OS
feature_image: "https://picsum.photos/1300/400?image=989"
---

## Composite OS

## Rust Programming Language

<p>
Using Rust programming languages has three main benefits that assist our Broker:
</p>

* <strong>Safer</strong> due to the Rust's compiler and type-system
* <strong>Faster</strong> due to it's lack of a garbage collector
* Allows for more <strong>concurrency</strong> to handle more clients

## MQTT-SN Rust Crate

<p>
We utilized a Rust Crate, known as ["mqtt-sn"](https://crates.io/crates/mqtt-sn). This crate provides the support and requirements for an MQTT-SN system. It included the packet specifications (packet id, topic subcription, etc) as well as the functionality for encoding, decoding, and parsing the packet. This made it possible for the packets, encoded in bytes, to be sent into a UDP socket.
</p>