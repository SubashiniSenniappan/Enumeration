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
Following searches for all the sites that is in the domain google.com

![Screenshot 2024-04-16 182456](https://github.com/Lakshmipriya2005/Enumeration/assets/115525361/a0eff083-9691-4fde-b6c3-90e652e7b459)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain google.com

![Screenshot 2024-04-16 182643](https://github.com/Lakshmipriya2005/Enumeration/assets/115525361/b0d15ff3-b6e0-485b-b967-1c93909aea82)



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![Screenshot 2024-04-16 183008](https://github.com/Lakshmipriya2005/Enumeration/assets/115525361/ecc999f7-1b8a-4aa0-9a82-d067cd5c2123)



inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

![Screenshot 2024-04-16 183537](https://github.com/Lakshmipriya2005/Enumeration/assets/115525361/b0f8ea5f-ebe2-4b29-b7f9-8c8c96f56aea)


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

![Screenshot 2024-04-16 183801](https://github.com/Lakshmipriya2005/Enumeration/assets/115525361/1f3a45e9-92ab-4c33-a793-cf210b65a3f5)


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![Screenshot 2024-04-16 183916](https://github.com/Lakshmipriya2005/Enumeration/assets/115525361/ea6bd286-72e3-43eb-8d67-4f14108f54e1)


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

![Screenshot 2024-04-16 190328](https://github.com/Lakshmipriya2005/Enumeration/assets/115525361/7e6c530a-e1ed-473f-bc51-128eb72a034e)


 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:


![img 1](https://github.com/Lakshmipriya2005/Enumeration/assets/115525361/51311995-da55-4458-9a5b-81fa7f46e76c)





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

##output

![img 3](https://github.com/Lakshmipriya2005/Enumeration/assets/115525361/d7e6b77a-332e-4236-9a3a-297ca88e539d)



##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output

 ![img 4](https://github.com/Lakshmipriya2005/Enumeration/assets/115525361/3b842162-4bf6-45cc-9721-59b95139576f)

  
  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

![img 4](https://github.com/Lakshmipriya2005/Enumeration/assets/115525361/f662ce4e-0093-46a8-ad1b-4cb3ddfacbad)



## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

