# DarknetTraficClassification
Developed classification model to differentiate between benign network traffic and Darknet-related activity. Conducted statistical and network analyses to identify key features crucial for classification. Built and fine-tuned a machine learning model based on selected features, ensuring accurate identification of Darknet traffic.

# Column and dataset description

DARKNET

Most of us are familiar with the Internet and the World
Wide Web (WWW, or web). We regularly access both using web
browsers or other networked applications to share information
publicly, guided by search engine indexing of the Domain Name
System (DNS) over globally bridged Internet Protocol (IP) networks.
This publicly accessible and indexed address space is known as
the surface web or clearnet. In contrast, the WWW address space
which is not indexed by search engines but still publicly accessible
is known as the deep web. Private networks within the deep web
or networks comprised of unallocated address space are known as
darknets and collectively termed the dark web.



'Flow ID' : Unique identifier for flow

'Src IP':  Ip source

'Src Port': Port source 

'Dst IP': Ip destination

'Dst Port': Port destination

'Protocol': protocol 6 - TCP (Transmission Control Protocol).
17 - UDP (User Datagram Protocol).
0 - ICMP (Internet Control Message Protocol).

'Timestamp': Time and hour 

'Flow Duration': Time of the complete flow

'Total Fwd Packet': Total number of packets sent in the forward direction (from source to destination).

'Total Bwd packets': Total number of packets sent in the backward direction (from destination to source).

'Total Length of Fwd Packet': Total length of all packets sent in the forward direction.

'Total Length of Bwd Packet': Total length of all packets sent in the backward direction.

'Fwd Packet Length Max': Maximum length of packets sent in the forward direction.

'Fwd Packet Length Min': Minimum length of packets sent in the forward direction.

'Fwd Packet Length Mean': Mean length of packets sent in the forward direction.

'Fwd Packet Length Std': Standard deviation of packet length sent in the forward direction.

'Bwd Packet Length Max': Maximum length of packets sent in the backward direction.

'Bwd Packet Length Min': Minimum length of packets sent in the backward direction.

'Bwd Packet Length Mean': Mean length of packets sent in the backward direction.

'Bwd Packet Length Std': Standard deviation of packet length sent in the backward direction.

'Flow Bytes/s': Amount of bytes transferred per second in the network flow.

'Flow Packets/s': Number of packets transferred per second in the network flow.

IAT, which stands for "Inter-Arrival Time", refers to the time lapse between the arrival of two successive events within a sequence of events. In the context of networks or network traffic, it applies to the time duration between the arrival of successive packets in a communication sequence.

'Flow IAT Mean': Mean value of the inter-arrival time of flows (average time between two flows) in the observed network traffic.

'Flow IAT Std': Standard deviation of the inter-arrival time of flows in the observed network traffic.

'Flow IAT Max': Maximum inter-arrival time of flows in the observed network traffic.

'Flow IAT Min': Minimum inter-arrival time of flows in the observed network traffic.

'Fwd IAT Total': Total time between two forward packets sent.

'Fwd IAT Mean': Mean value of the time between two forward packets sent.

'Fwd IAT Std': Standard deviation of the time between two forward packets sent.

'Fwd IAT Max': Maximum time between two forward packets sent.

'Fwd IAT Min': Minimum time between two forward packets sent.

'Bwd IAT Total': Total time between two backward packets sent.

'Bwd IAT Mean': Mean value of the time between two backward packets sent.

'Bwd IAT Std': Standard deviation of the time between two backward packets sent.

'Bwd IAT Max': Maximum time between two backward packets sent.

'Bwd IAT Min': Minimum time between two backward packets sent.

'Fwd PSH Flags': Number of forward packets with the PSH (Push) flag activated. Indicates that data should be pushed to the application layer.

'Bwd PSH Flags': Number of backward packets with the PSH (Push) flag activated.

'Fwd URG Flags': Number of forward packets with the URG (Urgent) flag activated. Indicates urgent data in the packet.

'Bwd URG Flags': Number of backward packets with the URG (Urgent) flag activated.

'Fwd Header Length': Total length of headers for forward packets.

'Bwd Header Length': Total length of headers for backward packets.

'Fwd Packets/s': Rate of forward packets per second.

'Bwd Packets/s': Rate of backward packets per second.

'Packet Length Min': Minimum length of packets.

'Packet Length Max': Maximum length of packets.

'Packet Length Mean': Mean length of packets.

'Packet Length Std': Standard deviation of packet length.

'Packet Length Variance': Variance of packet length.

'FIN Flag Count': Number of packets with the FIN (Finish) flag.

'SYN Flag Count': Number of packets with the SYN (Synchronize) flag.

'RST Flag Count': Number of packets with the RST (Reset) flag.

'PSH Flag Count': Number of packets with the PSH (Push) flag.

'ACK Flag Count': Number of packets with the ACK (Acknowledgment) flag.

'URG Flag Count': Number of packets with the URG (Urgent) flag.

'CWE Flag Count': Number of packets with the CWE (Congestion Window Reduced) flag.

'ECE Flag Count': Number of packets with the ECE (Explicit Congestion Notification Echo) flag.

'Down/Up Ratio': Downlink (incoming) to uplink (outgoing) ratio.

'Average Packet Size': Mean packet size.

'Fwd Segment Size Avg': Average size of forward segments.

'Bwd Segment Size Avg': Average size of backward segments.

In the context of data transmission and communication networks, the term "bulk" refers to a set or group of elements that are handled or transmitted together as a single entity. In terms of network packets, a "bulk" refers to a set of packets or segments that are sent or processed as a group, rather than handled individually. This grouping can be useful for efficiency in data transmission and to reduce the overhead associated with processing and transmitting individual elements.

'Fwd Bytes/Bulk Avg': Average number of bytes in a bulk of forward packets.

'Fwd Packet/Bulk Avg': Average number of packets in a bulk of forward packets.

'Fwd Bulk Rate Avg': Average rate of bulk forward packets.

'Bwd Bytes/Bulk Avg': Average number of bytes in a bulk of backward packets.

'Bwd Packet/Bulk Avg': Average number of packets in a bulk of backward packets.

'Bwd Bulk Rate Avg': Average rate of bulk backward packets.

A "subflow" is a part or subdivision of a larger flow that shares the same characteristics as the main flow, but is differentiated by a particular characteristic.For example, a bidirectional TCP flow between two devices could be divided into subflows to represent traffic in a specific direction (e.g., subflow of data packets sent and subflow of data packets received).

The key difference between a flow and a subflow lies in their scope and level of detail. While a flow represents a general sequence of data between two points in the network, subflows divide that sequence into more specific segments based on certain characteristics, such as direction, packet type, time, among others. Subflows allow a more detailed and specific analysis within a general flow.

'Subflow Fwd Packets': Number of forward subflow packets.

'Subflow Fwd Bytes': Number of forward subflow bytes.

'Subflow Bwd Packets': Number of backward subflow packets.

'Subflow Bwd Bytes': Number of backward subflow bytes.

'FWD Init Win Bytes': Initial window size for forward flow.

'Bwd Init Win Bytes': Initial window size for backward flow.

'Fwd Act Data Pkts': Number of active forward data packets.

'Fwd Seg Size Min': Minimum forward segment size.

'Active Mean': Mean of active time.

'Active Std': Standard deviation of active time.

'Active Max': Maximum active time.

'Active Min': Minimum active time.

In the context of computer networks, the term "idle" refers to the state of inactivity or lack of activity on a network device or network connection.

When a network device is idle, it means that it is not involved in transmitting or receiving data at that specific time.

'Idle Mean': Mean of idle time.

'Idle Std': Standard deviation of idle time.

'Idle Max': Maximum idle time.

'Idle Min': Minimum idle time.



References	

https://www.kaggle.com/code/happygerypangestu/darknet-traffic-classification-k-nearest-neighbor

Tajadura Cubillo, D. (2022). Aplicación de técnicas de Deep Learning en un Sistema de Detección de Intrusos con tráfico de red relacionado con la Dark Web. Universitat Politècnica de València. http://hdl.handle.net/10251/185219

Rust-Nguyen, N., Sharma, S., & Stamp, M. (2023). Darknet traffic classification and adversarial attacks using machine learning. Computers & Security, 127, 103098. https://doi.org/10.1016/j.cose.2023.103098.

Arash Habibi Lashkari, Gurdip Kaur, and Abir Rahali. 2021. DIDarknet: A Contemporary Approach to Detect and Characterize the Darknet Traffic using Deep Image Learning. In Proceedings of the 2020 10th International Conference on Communication and Network Security (ICCNS '20). Association for Computing Machinery, New York, NY, USA, 1–13. https://doi.org/10.1145/3442520.3442521

Almomani, A. Darknet traffic analysis, and classification system based on modified stacking ensemble learning algorithms. Inf Syst E-Bus Manage (2023). https://doi.org/10.1007/s10257-023-00626-2
