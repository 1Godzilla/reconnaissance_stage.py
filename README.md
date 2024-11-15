
# Reconnaissance Stage Tool

This Python script is designed to assist with the **Reconnaissance Stage** of cybersecurity. It automates information gathering about a target domain or IP address, providing critical details such as WHOIS information, DNS records, subdomains, IP geolocation, and open ports. The tool is built to support ethical hacking and penetration testing practices.

## Features

- **WHOIS Lookup**: Retrieve registration details about the target domain.
- **DNS Enumeration**: Gather DNS records like A, MX, and NS.
- **Subdomain Enumeration**: Discover subdomains of the target domain.
- **IP Geolocation**: Determine the geographical location of a target IP address.
- **Port Scanning**: Identify open TCP ports on the target.
- **HTTP Headers Inspection**: View the headers of a target web server.

## Requirements

- Python 3.x
- Libraries:
  - `socket`
  - `requests`
  - `dnspython`
  - `ipwhois`
  - `python-whois`

Install all dependencies using:
```bash
pip install -r requirements.txt

Usage

	1.	Clone this repository or copy the script to your machine:

git clone https://github.com/username/reconnaissance-tool.git
cd reconnaissance-tool


	2.	Run the script using Python:

python reconnaissance.py


	3.	Enter the required target details when prompted:
	•	Domain: Enter the domain name to analyze (e.g., example.com).
	•	IP Address: Provide the IP address for geolocation and port scanning.

Example Input and Output

Input:

Enter the target domain: example.com
Enter the target IP address: 93.184.216.34

Output:

--- WHOIS Information ---
Domain: example.com
Registrar: Example Registrar
Creation Date: 1995-08-13
Expiration Date: 2024-08-13

--- DNS Records ---
A Record: 93.184.216.34
MX Record: mail.example.com
NS Record: ns1.example.com, ns2.example.com

--- Subdomains ---
Found subdomains: blog.example.com, shop.example.com

--- Geolocation ---
Country: United States
Region: California
City: Los Angeles

--- Open Ports ---
Port 80 (HTTP) is open.
Port 443 (HTTPS) is open.

--- HTTP Headers ---
Server: Apache
Content-Type: text/html

Project Structure

reconnaissance/
│
├── reconnaissance.py     # Main script for reconnaissance
├── requirements.txt      # List of required Python libraries
└── README.md             # Documentation file

Limitations

	•	Focuses on TCP port scanning; does not include UDP scanning.
	•	Relies on third-party libraries for accuracy; data may vary based on API responses.

Future Enhancements

	•	Add banner grabbing to extract service details from open ports.
	•	Include OSINT integration for deeper reconnaissance (e.g., Shodan API).
	•	Support multi-threaded scanning for faster results.
	•	Generate HTML or PDF reports of the findings.

Legal Disclaimer

This tool is intended for educational purposes only. Ensure you have proper authorization before scanning any systems. Unauthorized use of this tool may violate local, state, or federal laws.

License

This project is licensed under the MIT License - see the LICENSE file for details.

Author

Ani Chigozie Destiny
Cybersecurity Enthusiast & Developer

Feel free to contribute to this project or report any issues for improvements.

### Notes:
- Replace `LICENSE` with the actual license file if you include one.
- Update the GitHub repository URL in the cloning section.
- Modify the features or output examples based on your script's actual capabilities.