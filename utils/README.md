# PCAP processing and feature extraction using MMT

The [extract_features_pcap.py](extract_features_pcap.py) script automates the process of processing an input pcap file, generating reports using the [MMT-Probe](https://github.com/Montimage/mmt-probe) tool, aggregating the results, and extracting session-based features for network traffic analysis.

## Requirements

To run the script, you need the following dependencies:

- Python 3.8.10+
- MMT tools (using [prebuilt packages](mmt-packages)) 
- Python packages: `pandas`, `numpy`, `scipy` (see [requirements.txt](requirements.txt))

## Installation

Install all required Python packages for testing:

```bash
pip3 install -r utils/requirements.txt
```
Install mmt tools:

```bash
sudo dpkg -i mmt-packages/mmt-dpi_1.7.4_c5a4a6b_Linux_x86_64.deb 
sudo dpkg -i mmt-packages/mmt-security_1.2.14_d74aea4_Linux_x86_64.deb 
sudo dpkg -i mmt-packages/mmt-probe_1.5.5_6765397_Linux_x86_64_pcap.deb 
```

## Usage

```Bash
python extract_features_pcap.py <pcap_file> <is_malicious (True/False)>
```
