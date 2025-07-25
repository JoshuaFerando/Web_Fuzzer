# Web_Fuzzer


## Description

A multi-threaded Python-based CLI tool to perform web fuzzing by brute-forcing a wordlist and checking for live directories via HTTP GET requests.

---


## 🚀 Features

- 🧵 Multi-threaded for fast performance.
- 📄 Wordlist-based brute force.
- ✅ Identifies live subdomains with HTTP 200 status code.
- 🖥️ Beautiful ASCII banner for branding.
- 📦 Simple and lightweight – only requires `requests`.

  ## 📁 File Structure

- `WebFuzzer.py` – Main script for website fuzzing.
- `small.txt` – (You need to provide) A wordlist containing directories names to test.

---

## ⚙️ Requirements

- Python 3.x

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/JoshuaFerando/Web_Fuzzer
   cd Web_Fuzzer
   ```


2. Install the required module using:
   ```bash
   pip install -r requirements.txt
   ```


---

## 🛠️ Usage
1. **Prepare your wordlist** (e.g., `small.txt`) – one directory per line.
2. **Edit script variables** in `WebFuzzer.py`:
   ```python
   url = "https://www.google.com"
   wordlist_path = "small.txt"
   total_threads = 72
   ```
3. **Run the tool**:
   ```bash
   python3 WebFuzzer.py
   ```

## 📝 Example Output

   ```bash



██╗    ██╗███████╗██████╗     ███████╗██╗   ██╗███████╗███████╗
██║    ██║██╔════╝██╔══██╗    ██╔════╝██║   ██║╚══███╔╝╚══███╔╝
██║ █╗ ██║█████╗  ██████╔╝    █████╗  ██║   ██║  ███╔╝   ███╔╝ 
██║███╗██║██╔══╝  ██╔══██╗    ██╔══╝  ██║   ██║ ███╔╝   ███╔╝  
╚███╔███╔╝███████╗██████╔╝    ██║     ╚██████╔╝███████╗███████╗
 ╚══╝╚══╝ ╚══════╝╚═════╝     ╚═╝      ╚═════╝ ╚══════╝╚══════╝
                                                               

        CLI Brute-Force Web Fuzzer
        
***********************************
Target URL: https://www.google.com
Wordlist Used: small.txt
Total Directories To check: 959
*********************************** 


The Various Directories found are...

https://www.google.com/crs
https://www.google.com/publisher
https://www.google.com/search
https://www.google.com/sw
https://www.google.com/research
https://www.google.com/groups
   
   ...
   ...
   ```

---


## 🔧 Configuration Tips

- If you encounter `ConnectionResetError`, reduce the `total_threads` value.
- Make sure your target URL does not block too many requests in a short span (may trigger rate-limiting or firewall rules).

---



## Disclaimer

This script is intended for educational and ethical penetration testing purposes only. Unauthorized usage against systems you do not own or have explicit permission to test is illegal.

## Contribution

Pull requests are welcome! Feel free to improve the script by optimizing performance or adding new features.

## Author

Joshua Fernando



