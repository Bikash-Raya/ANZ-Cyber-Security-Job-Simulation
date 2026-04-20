# 🕵️ Network Traffic Investigation Task (PCAP Analysis)

---

## 📌 Background Information

Suspicious network activity has been detected coming from a user on the ANZ network.  

A laptop has been flagged by security systems due to unusual internet traffic. An investigation is required to determine what the user accessed and downloaded.  

Your task is to examine the user’s network activity and identify:
- Images viewed  
- Files accessed or downloaded  

You have been provided with a packet capture file (PCAP) containing all recent network activity. The file may contain multiple artifacts, and you are expected to identify and report as many as possible.  

You must provide a report of all findings and document the processes and steps followed during the investigation.  

You will need to use **Wireshark** and a **Hex editor** to fully investigate the network traffic and analyze the PCAP file.

## 🧰 Tools Required

| Tool | Purpose |
|------|--------|
| Wireshark | Packet capture analysis |
| Hex Editor | File inspection and validation |
| PCAP File | Primary evidence source |

---


## 👤 My Findings and Answer.

The final answers and findings for this task are documented in the following file:

👉 [Task 2 - Answers.pdf](Task%202%20-%20Answers.pdf)

## 🔍 Methodology / What I Did

To complete this investigation, I analyzed the provided PCAP file using Wireshark and a Hex editor to reconstruct user network activity and extract evidence of accessed files and images.

### 🧰 Step 1: Loading the PCAP File
- Opened the PCAP file in Wireshark
- Reviewed overall traffic patterns and protocols
- Identified key traffic types (HTTP, DNS, TCP)

---

### 🔎 Step 2: Traffic Filtering
- Applied filters such as `http`, `dns`, and `tcp.stream`
- Isolated relevant web browsing sessions
- Focused on HTTP GET requests for file downloads

---

### 🌐 Step 3: Session Analysis
- Followed TCP streams to reconstruct full sessions
- Identified user requests and server responses
- Located files and media transferred over HTTP

---

### 📁 Step 4: File Extraction
- Used Wireshark “Export Objects (HTTP)” feature
- Extracted images and downloaded files from traffic
- Saved recovered artifacts for further analysis

---

### 🧩 Step 5: Hex Editor Analysis
- Opened extracted raw data in a Hex editor
- Identified file signatures (e.g., JPEG, PDF, ZIP)
- Reconstructed files by copying data between header and footer signatures
- Saved files in correct formats for validation

---

### 📊 Step 6: Validation of Findings
- Verified extracted files by opening them normally
- Cross-checked TCP streams with recovered artifacts
- Confirmed that extracted data matched network traffic evidence
