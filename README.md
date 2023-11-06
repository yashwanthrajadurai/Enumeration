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

## Output:
![image](https://github.com/NAVEENKUMAR4325/Enumeration/assets/119479566/c56223c8-ceec-485b-b721-5b936f478d7b)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

## Output:

![image](https://github.com/NAVEENKUMAR4325/Enumeration/assets/119479566/69ef9360-ac75-4bca-be08-ad7308f53935)


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

## Output:

![image](https://github.com/NAVEENKUMAR4325/Enumeration/assets/119479566/10daa454-357c-43f1-856a-85adc624bf7e)



inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

## Output:

![image](https://github.com/NAVEENKUMAR4325/Enumeration/assets/119479566/abe9bd49-94f6-4a60-b495-73096e36c500)


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

## Output:

![image](https://github.com/NAVEENKUMAR4325/Enumeration/assets/119479566/70d7e016-1db1-440d-8b05-7ababe569b42)


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

## Output:

![image](https://github.com/NAVEENKUMAR4325/Enumeration/assets/119479566/2f709c2e-ef5d-4b12-afd1-ff69ca1d8f82)


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

## Output:

![image](https://github.com/NAVEENKUMAR4325/Enumeration/assets/119479566/a79df725-f505-4606-8e26-e32dab133c62)


 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![image](https://github.com/NAVEENKUMAR4325/Enumeration/assets/119479566/627b0094-4373-4420-979a-6056da309035)






##dnsenum
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

![image](https://github.com/NAVEENKUMAR4325/Enumeration/assets/119479566/de8bc164-f3c8-479b-a142-b66e26dc3d18)


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

![image](https://github.com/NAVEENKUMAR4325/Enumeration/assets/119479566/829aeb6f-dada-4e99-b539-460c3f7d9aa7)


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

![image](https://github.com/NAVEENKUMAR4325/Enumeration/assets/119479566/429e4a59-6c42-4335-bb5c-d660bb4e25ed)


select any username in the first column of the above file and check the same

![image](https://github.com/NAVEENKUMAR4325/Enumeration/assets/119479566/e2e32c11-2541-4083-9118-1051fb694118)



#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output

  ![image](https://github.com/NAVEENKUMAR4325/Enumeration/assets/119479566/496726e7-74bf-423c-b4af-21f5906d0731)

  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
![image](https://github.com/NAVEENKUMAR4325/Enumeration/assets/119479566/6a2bfb53-6c61-4f8f-a63e-756a09baf6af)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

