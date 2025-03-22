
# Network Traffic Logs

This repository contains a cleaned and labeled network traffic dataset derived from **Canadian Institute for Cybersecurity (University of New Brunswick)** logs, widely used in the cybersecurity community for intrusion detection and threat analysis.

The dataset includes metadata about network connections and has been annotated with labels to distinguish **benign** from **malicious** activity. It is suitable for building and evaluating network security models.



This CSV file includes connection-level features and labels. processed for use in machine learning and network behavior analysis.

### 🔢 Features

| Column Name        | Description                                              |
|--------------------|----------------------------------------------------------|
| `id.orig_p`        | Source port of the connection                            |
| `id.resp_p`        | Destination port of the connection                       |
| `proto`            | Protocol used (e.g., `tcp`, `udp`, `icmp`)               |
| `service`          | Application layer protocol detected (e.g., `http`, `dns`)|
| `duration`         | Duration of the connection in seconds                    |
| `orig_bytes`       | Bytes sent from originator to responder                  |
| `resp_bytes`       | Bytes sent from responder to originator                  |
| `conn_state`       | Connection state (e.g., `S0`, `SF`, `REJ`)               |
| `missed_bytes`     | Number of bytes missed during capture                    |
| `history`          | TCP flag history summarizing the connection              |
| `orig_pkts`        | Number of packets sent by originator                     |
| `orig_ip_bytes`    | Total IP-level bytes sent by originator                  |
| `resp_pkts`        | Number of packets sent by responder                      |
| `resp_ip_bytes`    | Total IP-level bytes sent by responder                   |
| `label`            | `Benign - 0` or `Malicious - 1` label indicating traffic class   |

## 📚 Use Cases

- Intrusion Detection System (IDS) development
- Network anomaly detection
- Traffic pattern classification
- Training supervised/unsupervised ML models
- Visualization and exploratory data analysis

## 🧪 Source and Authenticity

This dataset is based on real network traffic, captured and analyzed. The traffic has been manually or heuristically labeled to reflect known benign and malicious behaviors, making it appropriate for research in network security.

## 📌 Notes

- The dataset has been cleaned for missing values and is ready for ML pipelines.
- Some fields (e.g., `service`, `duration`, `bytes`) may contain `NaN` values due to limitations in protocol detection or short-lived flows.

## 📜 License

This dataset is provided for educational and research purposes. Please cite the original source if used in publications.

---

For questions or contributions, feel free to open an issue or submit a pull request.
