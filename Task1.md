# Nmap Scan Report

**Scan initiated:** Wed Sep 24 01:52:03 2025  
**Command used:**  
```bash
/usr/lib/nmap/nmap -sS -oN Output.txt 192.168.1.1/24
```

---

## Host: 192.168.1.1
- **Status:** Host is up (0.0027s latency).  
- **Not shown:** 989 closed TCP ports (reset).  

| Port    | State     | Service         |
|---------|-----------|-----------------|
| 21/tcp  | filtered  | ftp             |
| 22/tcp  | filtered  | ssh             |
| 23/tcp  | open      | telnet          |
| 53/tcp  | open      | domain (DNS)    |
| 80/tcp  | open      | http            |
| 139/tcp | filtered  | netbios-ssn     |
| 443/tcp | filtered  | https           |
| 445/tcp | filtered  | microsoft-ds    |
| 3517/tcp| filtered  | 802-11-iapp     |
| 8082/tcp| filtered  | blackice-alerts |
| 8888/tcp| filtered  | sun-answerbook  |

**MAC Address:** `F4:27:56:3A:6D:57 (Dasan Network Solutions)`

---

## Host: 192.168.1.33
- **Status:** Host is up (0.00030s latency).  
- **Not shown:** 997 filtered TCP ports (no-response).  

| Port    | State | Service        |
|---------|-------|----------------|
| 135/tcp | open  | msrpc          |
| 139/tcp | open  | netbios-ssn    |
| 445/tcp | open  | microsoft-ds   |

**MAC Address:** `F8:54:F6:20:99:59 (AzureWave Technology)`

---

## Host: 192.168.1.34
- **Status:** Host is up (0.0051s latency).  
- **All scanned ports:** ignored states.  
- **Not shown:** 1000 closed TCP ports (reset).  

**MAC Address:** `EC:30:B3:28:2E:C6 (Xiaomi Communications)`

---

## Host: 192.168.1.35
- **Status:** Host is up (0.0066s latency).  
- **All scanned ports:** ignored states.  
- **Not shown:** 1000 closed TCP ports (reset).  

**MAC Address:** `72:6F:6C:F7:A1:75 (Unknown)`

---

## Host: 192.168.1.37
- **Status:** Host is up (0.0000050s latency).  
- **All scanned ports:** ignored states.  
- **Not shown:** 1000 closed TCP ports (reset).  

---

# Scan Summary
**Finished:** Wed Sep 24 01:52:25 2025  
**Scanned:** 256 IP addresses  
**Hosts up:** 5  
**Duration:** 22.21 seconds  

---

## Common Services

| Host IP      | Ports         | Services                           |
|--------------|--------------|-------------------------------------|
| 192.168.1.1  | 23, 53, 80   | Telnet, DNS, HTTP                  |
| 192.168.1.33 | 135, 139, 445| MSRPC, NetBIOS-SSN, Microsoft-DS   |

---

## Potential Security Risks

- **Telnet (23/tcp):** Transmits passwords in plaintext.  
- **HTTP (80/tcp):** Exploitable if web server software is outdated or misconfigured.  
- **DNS (53/tcp):** Open DNS may be abused for amplification attacks or cache poisoning.  
- **MSRPC (135/tcp):** Target for remote code execution or Windows exploits.  
- **NetBIOS (139/tcp) & Microsoft-DS (445/tcp):** File sharing vulnerabilities, ransomware, credential theft.  
