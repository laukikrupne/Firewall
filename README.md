# Firewall

A Firewall is a software program or a piece of hardware that helps to screen out hackers, viruses, and worms that try to reach your computer over the internet. A software firewall is a program that is installed on your pc. A hardware firewall is a device placed in between your network and untrusted internet. If more than a computer is connected to your network, then it is necessary to protect your network from the untrusted internet via a firewall. But it is also necessary to protect each computer with a software firewall so that if one computer gets infected from the viruses then other computers remain free from the viruses. Windows computers (OS 7 and higher) have a built-in firewall that is on by default. The basic task of a firewall is to regulate the flow of traffic in between computer networks of different trust levels.  For example, the Internet is the zone of no trust, and your home network is a zone of high trust. All incoming messages are passed through the firewall. The firewall checks whether these messages satisfy the security criteria. If they satisfy they are passed through the firewall. Otherwise, they are blocked by the firewall. A similar thing happens with the outgoing messages. If you turn your firewall off, then all the messages will pass through the firewall freely. As a result, hackers can easily hack your computer and obtain your sensitive data. So never shut your firewall off.

### How does a Firewall work?
Internet is an unrusted network of connected computers. In a web browser, we enter the name of the website. This request is forwarded to the website. Within seconds we get a reply from that computer on the internet that stores the content of the requested website. As a result, a website is displayed on the pc screen. But sometimes hackers get access to the Internet connection and then they try to steal your information but the firewall protects you from online hackers.

Firewalls use one or a combination of the following three methods to control traffic flowing in and out of the network:
- Packet Filtering
- Stateful inspection
- Proxy service

##### Packet Filtering
The firewall maintains a list of allowed and not allowed computers. Consider Bob and Sam the name of two servers present on the internet. Bob stores the content of the website (example.com) while Sam is the hacker’s computer and its name is written in the not allowed section of the list. Now John types the address of Bob’s computer (example.com) this request is forwarded to the internet. Bob stores the content of the requested website so it generates the reply. But hackers computer too sends a reply. Since Sam's name is written in the not allowed section of the list so whatever Sam had sent will be blocked by the firewall, but the content of the Bob will be forwarded to John’s pc. This method of protection is called packet filtering and the list is called access list.

##### Stateful inspection
The firewall also notes which website you are currently using. The firewall maintains the conversation list containing the name of your computer and the website that you are currently visiting. Consider hacker has hacked the computer and he has started sending some unwanted data with the data of the streaming video but your firewall knows you have accessed data from the youtube only. This method of protection is called Stateful Inspection.

##### Proxy service
John and Cena are the names of the computer connected to the internet via the third computer name Orlo. John requests (example.com) and Orlo receives the request and passes the request towards the internet. The computer thinks instead of John, Orlo is requesting for (example.com) i.e Orlo has hidden John from the attackers on the internet. Hence Orlo can hide the john with the help of Proxy firewalls.

### Types of Firewalls
- Packet Filtering Firewall
- Application/Proxy Firewall
- Hybrid Firewall

##### Packet Filtering Firewall
Suppose we are downloading the file of 200MB from the internet, but we will not receive the entire 200MB data at once but we will receive small packets say 5MB every second( A typical packet contains 1000 to 1500 bytes). This 5MB of every packet has the sender’s and receiver’s address. The Packet Filtering Firewall checks the sender’s and receiver’s data inside every packet. Hence called Packet Filtering Firewall.
> Limitations
The hacker can send malicious data inside payload of the packet so the Packet Filtering Firewall will not be able to detect it.

##### Application/Proxy Firewall
An application proxy firewall acts as an intermediate gateway attempting to look not only at the packet headers but also at the data inside the packets entering or leaving the network to be protected. Proxy Firewall hides the details of the client’s data from the internet.
>Limitations
Much slower than Packet Filtering Firewall.

##### Hybrid Firewall
Hybrid Firewall is the combination of Packet-Filtering firewall and Application/Proxy firewall. The Packet Filtering Firewall stays behind the Application Firewall in series.

### Choosing a Firewall

| Firewall Architecture | High Risk | Medium Risk | Low Risk |
| ------ | ------ |------ |------ |
| Packet Filtering |0|1|4|
| Application Gateway |3|4|2|
| Hybrid Gateway |4|3|2|
- 0 - unacceptable
- 1 - minimal security
- 2 - acceptable
- 3- effective
- 4 -recommended

### Limitations of Firewall
- How to verifies the incoming data?
  Hacker's can use fake data packets with trusted ip address.
- Intrusion Attack :-
  Hacker can easily baypass the firewall from inside to allow attack.
- Direct Internet Traffic :-
  When we add exception in firewall then hacker tries to send malicious data with the help of exception.
