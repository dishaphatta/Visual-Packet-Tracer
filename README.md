# Visual-Packet-Tracer

This project visualizes Wireshark-captured network traffic on Google Maps by processing IP addresses with Python, mapping them to locations, and generating a KML file for import.

Features:
- Capture network traffic with Wireshark.
- Extract and map source and destination IP addresses to geographic locations using the GeoLiteCity database.
- Generate KML files for visualization on Google Maps.
- Customizable line styles for better map visualization.

Requirements:
Software:-
Python 3.x (Download Python)
Wireshark (Download Wireshark)

Python Libraries:
Install the required libraries using pip in VS Code:
pip install dpkt socket pygeoip

Database:
Download the GeoLiteCity database and place it in the project’s root directory.

**How to Use**

Capture Network Traffic:

- Open Wireshark and select an active network interface (e.g., Ethernet or Wi-Fi).
- Start capturing packets.
- Stop the capture after a suitable duration.
- Save the captured packets as a .pcap file in the project folder (e.g., wire.pcap).
- Set Up the Project

Place the GeoLiteCity.dat file and wire.pcap file in the root directory.

Execute the script main.py:
$ python main.py

The script generates a .kml file containing the network traffic visualization data.

Import into Google Maps:

- Go to Google My Maps.
- Create a new map.
- Import the generated .kml file.
- Visualize your network traffic on the map.


