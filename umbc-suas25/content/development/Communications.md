---
menus:
    main:
        parent: Development
Title: Communications
---

The Gita XI 12 communicates with the ground station using the MAVLink (Micro Air Vehicle Link) protocol.

MAVLink is a lightweight, long ranged and open source communication protocol used in drones and unmanned vehicles. A unique advantage this protocol presents is its bi-directional communication capabilities. This allows the ground control station to send radio controls to manually pilot the aerial unit while receiving live time telemetry data such as air speed, altitude, pitch, distance travelled, GPS etc at the same time. The signal strength is constantly monitored by a heartbeat protocol, which is used to advertise the existence of a system on the MAVLink network, along with its system and component id, vehicle type, flight stack, component type, and flight mode (Mavlink np).

The Mavlink Long Range Signal (MAVLink LRS) is the radio system that allows communication through the MAVLink protocol over long distances (10km - 100km). The Mateksys Transmitter and Receiver modules used in the GITA XI 12 utilizes the LoRa (Long Range) hardware to achieve this range. MLRS supports full-duplex (bi-directional) connection. Therefore, even though the aerial and ground units are traditionally called receivers and transmitters consecutively, both essentially are transceivers.

Mavlink is used on this aircraft instead of other communication systems because it provides long range stable and bidirectional connection allowing both RC controls and telemetry communication to happen using the same equipment. Mavlink additionally provides more safety in case of accidental communication issues. For example, if the Ground Control System (GCS) connection is lost, the manual controls remain unaffected and the GCS is able to recover telemetry without restarting the flight controller. Usage of the specific hardware on the Gita XI 12 also allows wireless connection between the transmitter and the GCS, keeping navigation uncomplicated for the safety pilot.

![GCS_disconnected_but_plane_maneuverable](/development/GCS_disconnected_but_plane_maneuverable.png)
