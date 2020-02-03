# Introduction to Business Information Technlogy

# Business Technology Infrastucture core components
- Compute - compuatation power that needed to process tasks and handle application workload
- Network - how computing devices are interconnected with each other and talk. 
- Storage - all reliable and fault tolerant enterprise storage devices

## Compute

**Imagine you have 100 of clients(computers)**
Option 1:  go to each client to check compliance with corporate policies (not scaleable)

Option 2: set up a server than adminster all the clients centrally from the server. Initilize corporate policies and get a status update
on their complicance all in one place. You can manage users, permissions, their accounts, passwords, and other stuff from there, troubleshoot individual programs with clients as well. **Choose Server**

#### Server vs Client
- Servers has multiple powerful processors while clients has a single one
- Servers have more RAM
- Servers have faster hard drives
- Servers have more network cards( laptops usually have one wired and one wireless network card)
- Servers run a server operating system while client run client operating system
---

#### Operating Systems
**Client Operating Systems**
- Windows
- Mac OS X
- Ubuntu/Fedora

Entry level client operations system tasks:
- install operating system with correct setting, device drivers, configure the printer, install software
- troubleshoot slow performance, handling , power up and down, not being able to print, not being able to connect to server
- -test if problem is with client or a server side/networking problem
- maintence - scanning for malware, monitoring performance
- deploy operating system over a network for all clients (creating a standardized custom corporate image)(desktop admin)

**Server Operating Systems**
- Windows Server
- Mac OS X Server
- Red Hat Enterprise Server or SVSE Linux Enterprise Server
---
**Server Hardware Types**
- Tower Servers - cheapiest cost, most space used, worst power/cabling
- Rack Servers - (1 RU or rank unit)
- Blade Servers - expensive cost, less space used per unit, great power/cabling

## Server Types
1. Web servers - deliver web content over HTTP/HTTPS web servers can be public or private(intranet)
  - Client types in url into browsser ---> url get converted to IP address by DNS server--->computer connects to web server with IP address and requests for the website---> the web server fetches web pages, images,text, and video from it file syste, complies it and sends the website (HTTP response)
  - Microsoft server have internet information services (IIS) and Apache Tomcat

2. File servers -central location to store documents and files. File shares= N:// or T:// like at work that come automatically attached
  - create shares on server an map on to clients
  - server message block (SMB) or NFS or common internet file system (CIFS) protocol


3. Print servers - most new wired/wireless network based prints contain a print server built in (Document print queuing, spooling or prioritization)

4. DHCP server (dynamic host configuration protocol)- delievers IP addressing to clients and ensures there is no duplicate IP addresses in the network

5. DNS (Domain name server) -  translates fully qualified domain names into IP addresses in public and private network
  - pluralsight.com ----> 54.202.43.122

6. Proxy server/load balancer - handles external requests, caches content to improve performance, acts a a firewall

7. Email Server stores mailboxes, calendars, contact, spam filtering, and malware scan, support unified messages
  - POP3, IMAP, SMTP protocols
  - Exchange Server vs Zimbra

8. Authentication server - handles user auth and permissions(Active Directory)
  - Login to validate on server and you are given an authorization token, which states your level of access
  - Authentication server also verfies if the computer you use to access the network belons to the company. If not, you can not login
This is done by creating a domain enviroment, join clients to domain. Most od directory services operatoins happen over LDAP protocol
  - Microsost Active Directory, Open LDAP, Apache, or RedHat Directory Server
  
9. Syslog server - consolidated logs from multiple sources in a single location like router logs, firewall logs, webserver logs, etc...
  - routers may send messages about user logging on to console session, while web servers might log access denied events/attempts

10. Communication servers - IM, audio/video cals, virtual conferencing, auditing messages/calls, integrating PBX or PSTN
  - VOIP protocol
  - Lync server vs Jabber
  
  ## IT Service Managment
  - ICT infrastructure management
  - Service Desk
  - IT Infrastructure Library (ITIL)
  - Microsoft Operations Framework (MOF)
  - FitSM
  
  ## Data backups
 Data loss can translated to lost customers, lawsuits, tarnished reputations, and lost revenue, so protect data with regular backups.
 Also, perform regular mock data loss drill restoration to check that the data backup is working and is beneficially.
 
 Backup professionals have a responsibility to design a complete disaster recovery solution. A complete disaster recovery solution plan can encompass protecting a single file on a single customer to protecting a entire site level(in case of earthquakes, fires floods). Backups of entire sites are place in another site i.e. If you have a data center in NY back it up in Chicago.  

Examples are backup systems: 
- Storage media
- Backup tools
- Windows Backups

---
## When to build desktop apps
- App that can run standalone or offline
- no latency (since desktop app are local and are not very dependent on external networ, high exceution speed)
- when you need access local hardware like hard drive/ printer/ scanne/ graphics card(game)
- local operating system access

## When to build mobile apps instead of a modile enabled mobile website
- local resources from phone/tablet are need (camera access)
- Background tasks (for example: fitness app can run the bg to count calories while you use another mobile app)
- push notifications
- mobile apps can have local storage(for example: WhatsApp lets you res messge even if you are offline for a minute
- low resource consumption

## Job examples
- Server Admin
- Web or Database Admin
- Unified Messaging Admin
- Network Admin
- Storage Admin
- Web Developer
- Mobile Developer
- Software Developer
- PLM engineer = product life cycle managament 


1. RAM
  - memory hierachy (disks, RAM, Caches, Registers)
2. CPU
  - Instruction set Architecture
  - Instruction Level Parrkekusn(ILP)
3. Operating System
  - Virtual memory
  - Processes & Threads
  - static and shared libraries
4. Basic Networks/ The internet
5. How computers works PT1/PT2
6. The internet playlist
7.  internet sockets, IP, webframe, 
HTTP, web browsers, hosting
8. Interprocess communication
---
docker ps <br>
airflow-tutorial_webserver_1 <br>
docker exec -ti airflow-tutorial_webserver_1 bash <br>
**airfloow@ef5ea96c9c4**: ~$ airflow list-dags <br>
airflow initdb <br> 

docker exec -ti airflow-tutorial_webserver_1 bin/bash
ls
**airflow airflow.cfgg airflow-webserver.pid dags logs**
