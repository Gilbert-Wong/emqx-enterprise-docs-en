
.. _mqtt:

=============
MQTT Protocol
=============

------------------------------------------------------
MQTT - Light Weight Pub/Sub Messaging Protocol for IoT
------------------------------------------------------

Introduction
------------

MQTT stands for "MQ Telemetry Transport". It was invented by Dr Andy Stanford-Clark of IBM and Arlen Nipper of Arcom in 1999 when they were connecting geographically dispersed devices on an unreliable network infrastructure. The protocol is designed with goals like "simple to implement", "Quality of Service"  and "Lightweight and bandwidth efficient". These goals still characterize the MQTT protocol today.

In the abstract of MQTT standard the MQTT protocol is described as follow: 

    "MQTT is a Client Server publish/subscribe messaging transport protocol. It is light weight, open, simple, and designed so as to be easy to implement. These characteristics make it ideal for use in many situations, including constrained environments such as for communication in Machine to Machine (M2M) and Internet of Things (IoT) contexts where a small code footprint is required and/or network bandwidth is at a premium."


MQTT Web site: http://mqtt.org

MQTT V3.1.1 standard: http://docs.oasis-open.org/mqtt/mqtt/v3.1.1/os/mqtt-v3.1.1-os.html

Features
--------

1. Open messaging transport protocol, easy to implement.

2. Use of publish/subscribe message pattern, which supports many-to-many communication.

3. Based on TCP/IP network connection.

4. 1 byte Fixed header, 2bytes KeepAlive packet. Compact packet structure.

5. Support QoS, reliable transmission. 

Use Cases
------------

MQTT protocol is widely used in Internet of Things, Mobile Internet, smart hardware, automobile, energy and other industry. 

1. IoT M2M communication, IoT big data collection 

2. Mobile message push, Web message push

3. Mobile instant messenger

4. Smart hardware, smart home, smart phone

5. Automobile communication, electric vehicle charging station/pole

6. Smart city, telemedicine, distance education

7. Energy industry
   
.. _mqtt_vs_xmpp:

------------------
MQTT v.s. XMPP
------------------

MQTT is designed to be light weight and easy to use. It is suitable for the mobile Internet and the Internet of Things. While XMPP is a product of the PC era. 

1. MQTT uses a one-byte fixed header and two-byte KeepAlive packet, its packet is small at size and simple to en/decode. While XMPP is encapsulated in XML, it is large in size and complicated in interaction.

2. MQTT uses topic for routing, it is more flexible than XMPP's peer to peer routing based on JID.

3. MQTT protocol doesn't define a payload format, thus it carries different higher level protocol with ease. While the XMPP uses XML for payload, it must encapsulate binary in Base64 format.   

4. MQTT supports message acknowledgement and QoS mechanism, which is absent in XMPP, thus MQTT is more reliable. 


   
   
.. _mqtt_client_libraries:

---------------------
MQTT Client Library 
---------------------

emqtt Client Library 
--------------------

emqtt project: https://github.com/emqtt

+--------------------+---------------------------------+
| `emqttc`_          | Erlang MQTT Client Library      |
+--------------------+---------------------------------+
| `CocoaMQTT`_       | Swift MQTT Client Library       |
+--------------------+---------------------------------+
| `QMQTT`_           | QT Framework MQTT Client Library|
+--------------------+---------------------------------+

Eclipse Paho Client Library
----------------------------

Paho's Website: http://www.eclipse.org/paho/

mqtt.org Client Library
------------------------

mqtt.org: https://github.com/mqtt/mqtt.github.io/wiki/libraries

.. _emqttc: https://github.com/emqtt/emqttc
.. _CocoaMQTT: https://github.com/emqtt/CocoaMQTT
.. _QMQTT: https://github.com/emqtt/qmqtt

