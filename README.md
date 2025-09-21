# hash-id-helper

Hash-ID Helper
Hash-ID Helper is a Python-based utility that helps cybersecurity students and CTF players quickly
**identify hash types** and generate example cracking commands for **Hashcat** and **John the
Ripper**.
Features
- Detect common hash types (MD5, SHA1, SHA256, bcrypt, etc.)
- Suggest Hashcat `-m` mode IDs
- Suggest John the Ripper formats
- Save hashes to a clean file (`hashes_for_cracking.txt`)
- Beginner-friendly usage
Installation
git clone https://github.com/yourusername/hash-id-helper.git
cd hash-id-helper
pip install -r requirements.txt
Usage
Identify hashes from a file:
python3 hash_helper.py -i examples.txt
Identify a single hash from command line:
echo "5f4dcc3b5aa765d61d8327deb882cf99" | python3 hash_helper.py
Example Output
Hash: 5f4dcc3b5aa765d61d8327deb882cf99
Detected: MD5
hashcat mode: 0
Example hashcat command:
hashcat -m 0 hashes_for_cracking.txt /usr/share/wordlists/rockyou.txt
License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
