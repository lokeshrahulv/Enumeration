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
## OUTPUT:
![239592969-75019822-2a90-47e2-93cf-5c0d8ce50f3d](https://github.com/lokeshrahulv/Enumeration/assets/118423842/39766180-84a3-4d0d-aef5-7025de30bdc7)
filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
## OUTPUT:
![239593233-aca98252-be96-42cb-8291-95388802523f](https://github.com/lokeshrahulv/Enumeration/assets/118423842/aaae97b0-a53c-4907-8fbd-25f20c0508c0)
intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
## OUTPUT:
![239594061-79c3aa8a-24c1-46dc-b2fa-5d45cf440bb5](https://github.com/lokeshrahulv/Enumeration/assets/118423842/1b30a409-d636-4a3d-b513-4827f47f4871)
inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
## OUTPUT:
![239594379-5df0d26a-9a8d-41b1-806b-39ee0b516fd5](https://github.com/lokeshrahulv/Enumeration/assets/118423842/3eef73cc-006e-46bb-bc97-682421c835d9)
intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
## OUTPUT:
![239594611-76cec9fc-3756-4e59-8ab7-62ef225e49f6](https://github.com/lokeshrahulv/Enumeration/assets/118423842/1145b73e-46bb-471b-94bd-ef036613692e)
link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
## OUTPUT:
![239594767-48385782-16fa-4b11-bb77-410f4b69d328](https://github.com/lokeshrahulv/Enumeration/assets/118423842/2cdd0b71-854c-4f7e-a3a6-953a0fb813c9)
cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
## OUTPUT:
![239594985-fed106bd-ef84-4eba-9f20-42f0578caf07](https://github.com/lokeshrahulv/Enumeration/assets/118423842/40c8e1d9-fb3c-4461-abe2-174d168d3ad2)
#DNS Enumeration
##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![240358807-404a97fc-30d3-4dbf-bd44-e87e8a6a7c4d](https://github.com/lokeshrahulv/Enumeration/assets/118423842/44d96a43-66bd-477d-a04d-41e84c5043cb)
![240358918-cccb27a8-2711-492a-bda9-5fa261c0f27c](https://github.com/lokeshrahulv/Enumeration/assets/118423842/abb68801-cbbc-4046-94b3-42a98c0dc6bd)

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
## OUTPUT:
![240359135-2c7f0da3-b169-4390-a802-e7da5842a787](https://github.com/lokeshrahulv/Enumeration/assets/118423842/c76e3206-347c-47a3-a39f-028f2c65d591)
##smtp-user-enum Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![240359294-36268e62-becc-4a52-971d-0db0460b9673](https://github.com/lokeshrahulv/Enumeration/assets/118423842/51e334f0-2ee0-4c36-95ec-ca6d551d7257)
In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
select any username in the first column of the above file and check the same
![240359449-213e9b42-33e5-41d4-a2bc-ec3e7c03bd72](https://github.com/lokeshrahulv/Enumeration/assets/118423842/d64c07ae-c0bd-428b-9475-ff7fc29b784c)
#Telnet for smtp enumeration Telnet allows to connect to remote host based on the port no. For smtp port no is 25 telnet 25 to connect and issue appropriate commands
![240359680-6c49d93b-c710-4e51-87af-d6cb5a453918](https://github.com/lokeshrahulv/Enumeration/assets/118423842/0de80821-5625-46a0-aa36-d97999af192c)
## nmap –script smtp-enum-users.nse
The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.
![240359786-5a15bf55-ccc2-4c84-81bc-a7975acc0265](https://github.com/lokeshrahulv/Enumeration/assets/118423842/0c0d353a-0617-4f46-bdf4-ab061d7286b9)
## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

