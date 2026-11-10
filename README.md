# Website Footprinting and Reconnaissance Project

## Project Overview
This project involved conducting a website footprinting and reconnaissance exercise using Kali Linux. The objective was to gather publicly accessible information about a target domain and identify its domain registration details, web technologies, IP address, HTTP response headers, Web Application Firewall (WAF), and DNS records.

**Target Domain:** `networkwalks.com`

**Operating System:** Kali Linux

## Objectives
- Identify domain registration information.
- Discover technologies used by the target website.
- Resolve the domain name to its IP address.
- Analyze HTTP response headers.
- Detect the Web Application Firewall protecting the website.
- Enumerate publicly accessible DNS records.

## Tools and Methodology

### Task 1: WHOIS – Domain Registration Lookup
**Command:**
```bash
whois networkwalks.com
```
**Purpose:**

Used WHOIS to retrieve domain registration information, including registrar details, registration dates, domain status, and name servers.

### Task 2: WhatWeb – Web Technology Fingerprinting
**Command:**
```bash
whatweb networkwalks.com
```
**Purpose:**

Used WhatWeb to identify technologies associated with the target website, such as web servers, content management systems, frameworks, and other technologies.

### Task 3: Nslookup – DNS Resolution
**Command:**
```bash
nslookup networkwalks.com
```
**Purpose:**

Used Nslookup to resolve the domain name into its corresponding IP address and retrieve DNS information.

### Task 4: cURL – HTTP Response Header Analysis
**Command:**
```bash
curl -I https://networkwalks.com
```
**Purpose:**

Retrieved HTTP response headers to examine server responses, status codes, server information, content types, and other available header information.

### Task 5: Wafw00f – Web Application Firewall Detection
**Command:**
```bash
wafw00f networkwalks.com
```
**Purpose:**

Used Wafw00f to identify whether a Web Application Firewall was protecting the target website.

**Finding:**
- Detected WAF: ModSecurity
- Provider: SpiderLabs
- Number of requests: 2

The scan identified ModSecurity as the Web Application Firewall associated with the target website.

### Task 6: DNSRecon – DNS Enumeration
**Command:**
```bash
dnsrecon -d networkwalks.com -t std
```
**Purpose:**

Used DNSRecon to enumerate publicly available DNS records and gather information about the target domain's DNS infrastructure.

## Skills Demonstrated
- Website footprinting
- Passive and active reconnaissance
- DNS enumeration
- Web technology fingerprinting
- HTTP header analysis
- Web Application Firewall identification
- Kali Linux command-line operations
- Cybersecurity information gathering

## Key Takeaways
This practical exercise improved my understanding of website reconnaissance and the importance of information gathering during the early stages of a penetration testing engagement.

I gained hands-on experience using different Kali Linux tools to investigate domain information, identify web technologies, analyze HTTP responses, and detect web security mechanisms.

## Screenshots and Evidence
Screenshots documenting each practical task are included in the `screenshots` folder.

## Disclaimer
This project was conducted for educational purposes. Reconnaissance activities should only be performed against systems and domains for which proper authorization has been obtained.

---
**Project Category:** Cybersecurity | Footprinting | Reconnaissance

**Environment:** Kali Linux
