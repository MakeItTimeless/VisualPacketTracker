## Project Overview  
This project enables you to:  
- Capture network traffic using Wireshark (export as `.pcap` or `.pcapng`)  
- Parse the capture using Python (extract source IPs and metadata)  
- Geolocate each source IP using the GeoLiteCity database  
- Generate a KML/KMZ file that plots these IP locations on a map  
- Upload/view the resulting file on KMZView (https://kmzview.com/) to visually inspect where your packets are coming from and going to  



## Main Feature Highlight  
**Mapping network-traffic origins geographically** — using packet capture → IP extraction → geolocation → mapping workflow, you can _see_ the sources of traffic on a global map, which is valuable for cybersecurity analytics, incident response, teaching, and reporting.



## Repo Structure (suggested)

Here’s a **properly aligned** ready-to-copy repo structure for **VisualPacketTracker**:

```
VisualPacketTracker/
├── capture_files/
│   └── example_capture.pcap
├── data/
│   └── GeoLiteCity.mmdb
├── scripts/
│   ├── parse_pcap.py
│   ├── geolocate_ips.py
│   └── generate_kml.py
├── outputs/
│   ├── ip_list.json
│   ├── geo_ips.json
│   └── network_map.kmz
├── screenshots/
│   └── map_visualisation.png
├── README.md
└── requirements.txt
```

## Screenshot / Visualisation

**Here’s how the map visualisation looks in KMZView:**

#### Map View — Regional Focus  
<img width="1918" height="878" alt="map_visualization1.png" src="https://github.com/user-attachments/assets/2de2a4b0-d77b-4fce-908e-13cffda8a770" />



## **Key Tools & Components**

* KMZView  —  Web viewer for KML/KMZ map files (https://kmzview.com/)

* GeoLiteCity / GeoLite2  —  Free IP-geolocation database by MaxMind

* Wireshark  —  Packet capture tool to export network traffic files



## **Use Cases & Benefits**

* Visualise endpoints of a DDoS simulation or real-world network traffic for your “AI Evaluator” project

* Enhance VAPT or network-forensics reports with geographic maps of traffic sources

* Educational tool for teaching network forensics, packet capture workflows and geolocation mapping

* Incident-response support: quickly spot unexpected geographic origins of traffic
  

## **Future Enhancements**

* Real-time capture & live mapping instead of post-process only

* Heat-map overlays or clustering of IPs instead of individual markers

* Automated alerts for IPs in high-risk regions or flagged by threat-intel feeds

* Web dashboard or interactive viewer for user exploration

* Containerisation (Docker) & notebook (Jupyter) versions for classroom/deployment use

 ---
 
  Thank you for checking out VisualPacketTracker! Feel free to fork, contribute, and extend it.
If you embed this in your project repo, adjust any file-paths or command names to match your actual code structure.


