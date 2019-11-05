## LibreCAN: Automated CAN Message Translator

In this project, we developed LibreCAN, a system to automatically translate most CAN messages with minimal effort. The protocol is designed to save security researchers the time and effort they spend manually reverse-engineering the CAN messaging format of each vehicle they study. This makes it easier to determine how new attacks can be used against a number of makes and models at once and design necessary defenses.

Vehicle security attacks to date have all shared one very important feature – they all ultimately require write access to the CAN bus. But in order to do that, one has to know the message format of the CAN bus to inject meaningful data. All makes and models of vehicles have different message formats that are proprietary to the car manufacturer which hopes to prevent cybersecurity attacks on vehicles by not disclosing translation tables for CAN data. In order to cause targeted and intentional changes in vehicle behavior, malicious CAN injection attacks require knowledge of these translation tables.

### Abstract

Modern Connected and Autonomous Vehicles (CAVs) are equipped
with an increasing number of Electronic Control Units (ECUs),
many of which produce large amounts of data. Data is exchanged
between ECUs via an in-vehicle network, with the Controller Area
Network (CAN) bus being the de facto standard in contemporary
vehicles. Furthermore, CAVs have not only physical interfaces but
also increased data connectivity to the Internet via their Telematic
Control Units (TCUs), enabling remote access via mobile devices. It
is also possible to tap into, and read/write data from/to the CAN
bus, as data transmitted on the CAN bus is not encrypted. This
naturally generates concerns about automotive cybersecurity. One
commonality among most vehicular security attacks reported to
date is that they ultimately require write access to the CAN bus.

In order to cause targeted and intentional changes in vehicle behavior, 
malicious CAN injection attacks require knowledge of the
CAN message format. However, since this format is proprietary
to OEMs and can differ even among different models of a single
make of vehicle, one must manually reverse-engineer the CAN
message format of each vehicle they target — a time-consuming
and tedious process that does not scale. To mitigate this difficulty,
we develop LibreCAN, which can translate most CAN messages
with minimal effort. Our extensive evaluation on multiple vehicles
demonstrates LibreCAN’s efficiency in terms of accuracy, coverage,
required manual effort and scalability to any vehicle.
