# Network Infrastructure Memory

## Network Core
- **Router**: Ubiquiti UniFi UCG Max (DHCP server)
- **WAN**: 2x 1Gbps/50Mbps DOCSIS connections
- **Switches**:
  - 3x UniFi Flex 2.5G 8-port
  - 1x UniFi Flex 2.5G 4-port
  - 2x Mikrotik CRS305-1G-4S+IN
- **Access Points**: 3x UniFi U7

## Servers and Storage
All named devices connect via 10GB fiber and follow periodic table naming scheme.

### Lithium
- **Platform**: Synology DS1525+
- **RAM**: 32GB
- **Role**: NAS, Docker host, light virtual machines, backup Pi-hole DNS

### Sodium
- **CPU**: Intel Core i5-12500K
- **RAM**: 32GB
- **Storage**: 4TB NVMe
- **OS**: Linux Server
- **Role**: Primary Pi-hole DNS, Docker host, virtual machines

### Hydrogen
- **CPU**: Intel Core i9-12900K
- **RAM**: 48GB
- **GPU**: AMD Radeon RX 9070 XT 16GB
- **Storage**: 6TB NVMe
- **OS**: Fedora Linux or Windows 11
- **Role**: AI/ML workstation

### Sulfur
- **Platform**: Nvidia DGX Spark
- **RAM**: 128GB
- **Storage**: 4TB NVMe
- **Role**: Dedicated LLM inference server running vLLM and ComfyUI

### Carbon
- **Platform**: Lenovo ThinkPad X1 Carbon Gen 11

### Magnesium
- **Platform**: Apple M4 MacBook Pro 16"

### Xenon
- **Platform**: Microsoft Xbox Series X

## Network Segmentation
Dedicated VLANs for traffic isolation:
- Servers
- IoT
- Management
- Mobile
- Private
- Guest

## Naming Convention
Device naming follows periodic table elements.
