# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com

<img width="1859" height="1011" alt="Screenshot 2026-02-05 223446" src="https://github.com/user-attachments/assets/f0d1e0e8-aacf-40a6-b172-c8a312de2d63" />

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

<img width="1749" height="1001" alt="Screenshot 2026-02-05 223606" src="https://github.com/user-attachments/assets/9ce5313e-ba4f-4ca0-8410-91a8481ab090" />

intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

<img width="1768" height="1025" alt="Screenshot 2026-02-05 223701" src="https://github.com/user-attachments/assets/00b64af6-23b7-457e-9ee5-71fbcddccf97" />

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

<img width="1733" height="1033" alt="Screenshot 2026-02-05 223811" src="https://github.com/user-attachments/assets/5540ce93-07d5-4811-9b5d-7511f3ac4d9f" />

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

<img width="1736" height="1026" alt="Screenshot 2026-02-05 223915" src="https://github.com/user-attachments/assets/82dd6006-9105-42b7-b11c-0d310140b5c8" />

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

<img width="1770" height="1030" alt="Screenshot 2026-02-05 224122" src="https://github.com/user-attachments/assets/af6fe259-b627-47ec-a436-4bd0ef027e72" />

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

 <img width="1756" height="1039" alt="Screenshot 2026-02-06 082116" src="https://github.com/user-attachments/assets/81eaaa57-86c7-4379-ae7e-c23f45a66297" />

## DNS Enumeration:

## DNS Recon:
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

<img width="1280" height="694" alt="1" src="https://github.com/user-attachments/assets/08ffb796-26df-4a3e-ba59-91742c50b625" />

## dnsenum:
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.
## Output:
<img width="1280" height="694" alt="2(1)" src="https://github.com/user-attachments/assets/326a77ee-a2bd-4940-b8bb-642b2f7e1035" />

<img width="1280" height="694" alt="2(2)" src="https://github.com/user-attachments/assets/c57b86de-aefb-4850-85a1-e0ecd1169b6d" />

## smtp-user-enum:
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

<img width="1280" height="694" alt="3" src="https://github.com/user-attachments/assets/598e1e72-6da7-469c-9f48-2116b715f4dd" />

In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same
## Output:

<img width="1280" height="694" alt="4" src="https://github.com/user-attachments/assets/8994b861-a6a8-422f-a028-221a573a98f3" />

## Telnet for smtp enumeration:
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
## Output:
   
<img width="1280" height="694" alt="5" src="https://github.com/user-attachments/assets/e44ec549-1564-46af-9057-eb51e9c5ee21" />

## nmap –script smtp-enum-users.nse <hostname>:

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## OUTPUT:

<img width="1280" height="694" alt="6" src="https://github.com/user-attachments/assets/a120aff1-2462-46cb-ba0f-3e0b1c893044" />

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

