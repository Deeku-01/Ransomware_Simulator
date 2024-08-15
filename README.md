# moSeR

# Your Friendly Ransomware Simulator

## Overview

**moSeR** is a Python-based tool designed to simulate the behavior of various ransomware families. This simulator replicates the encryption mechanisms, key management, and exfiltration techniques of 20 different ransomware variants, providing a comprehensive environment for studying and understanding these types of cyber threats.

## Features

- **20 Ransomware Variants**: Accurately simulates the encryption and key exfiltration techniques of 20 different ransomware families.
- **Multiple Encryption Techniques**: Supports encryption algorithms such as AES, ChaCha20, and RSA, tailored to specific ransomware types.
- **Configurable Simulation**: Easily customize and choose between full or partial file encryption based on the ransomware variant.
- **Private Key Exfiltration**: Simulates exfiltration of the private key via email, including different exfiltration methods for different ransomware families.
- **Modular Design**: The simulator is structured to allow easy addition or modification of ransomware variants and their corresponding behaviors.

## Ransomware Variants Simulated

1. **WannaCry** - Implements encryption using ChaCha20 with RSA for key encryption.
2. **Petya** - Simulates master boot record encryption with RSA key management.
3. **Locky** - AES encryption with unique key per file, using RSA to encrypt the AES keys.
4. **Cerber** - Custom AES-256 encryption with key exfiltration.
5. **TeslaCrypt** - AES encryption with RSA key encryption.
6. **CryptoLocker** - RSA-2048 for file encryption.
7. **NotPetya** - MBR encryption along with file encryption using AES.
8. **Sodinokibi (REvil)** - ChaCha20-Poly1305 with RSA for key encryption.
9. **Maze** - RSA-2048 for encryption and data exfiltration techniques.
10. **Ryuk** - AES-256 with RSA encryption for the AES keys.
11. **Dharma** - AES-256 encryption with RSA key encryption.
12. **Conti** - Multi-threaded encryption using AES with RSA.
13. **Egregor** - Combines RSA and AES for file encryption.
14. **Avaddon** - AES-256 with RSA encryption and exfiltration.
15. **Black Basta** - Exfiltration-focused with multiple obfuscation techniques.
16. **Play** - Partial encryption with RSA and AES.
17. **SunCrypt** - Hybrid RSA and AES-256 encryption.
18. **Thanos** - Customizable ransomware with RSA-4096 and AES.
19. **Snake (Ekans)** - Targeted attacks using AES with RSA key management.
20. **Clop** - RSA-1024 encryption with public and private key exfiltration.

## Installation

### Prerequisites

- Python 3.8+
- Pip (Python package manager)
- Dependencies listed in `requirements.txt` in Ransim Folder

### Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/Ransomware_Simulator.git
   cd Ransomware_Simulator/Ransim

2. Installing Dependencies
     ```bash
     pip install -r requirements.txt

3.Run the simulator:
  ```bash
  python script.py

Usage
Main Script
The main script (script.py) allows you to simulate different ransomware variants. You will be prompted to select a ransomware variant and the encryption type (if applicable). The script will then simulate the encryption process.

Description Module
The simulator includes a module (descript.py) that handles the Description of Encrypted files.

Key Exfiltration Module
This module can send the private key to a remote server or an email address based on your selection.

Configuration
The ransomware behaviors are configurable via a ransomware_config.json file, where you can specify details like the encryption type and file extensions used by each ransomware variant.

Important Notes
Educational Purposes Only: This simulator is intended solely for educational and research purposes. The use of this tool in any unauthorized or malicious manner is strictly prohibited.
No Real Encryption: While the simulator mimics the behavior of ransomware, it does not perform actual encryption on sensitive files.

Contribution
Contributions are welcome! If you have suggestions for new features or ransomware variants to include, feel free to fork the repository and submit a pull request.
