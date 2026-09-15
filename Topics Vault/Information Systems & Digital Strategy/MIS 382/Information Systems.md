---
topic: "Information Systems & Digital Strategy"
related-topics: [Supply Chain & Operations]
source-class: "MIS 382"
source-semester: "Fall 2027"
tags:
  - topic/infosys
  - topic/ops
  - class/MIS-382
---

## 1. Management Information Systems

**Definitions**

- System: a regularly interacting or interdependent group of items forming a unified whole
- Systems Analysis and Design: a structured approach to developing and improving systems
- Management Information Systems: a business function dealing with planning, development, management, and use of IT tools to help people perform information processing and management tasks
- MIS coordinates three organizational resources: people, information, and information technology

**The Three Key Resources of MIS**

- People: the organization's most important resource and its reason for existing
- Information: classified by usefulness and value, and classified by quality
- Information Technology: hardware (input and output devices, storage, computing, telecom, connecting) and software (application vs system)

**How People, Info, and Tech Interact**

- Information systems enable people to interact with information using technology
- Systems development: can we make something that works
- Systems analysis: how does it work, and how well
- Systems design: can we make it work better

**Classifying Information by Usefulness and Value**

- Data: raw facts, text, graphics, sound, etc.
- Data plus meaning and context becomes Information
- Information plus usefulness in decision making becomes Intelligence
- Intelligence plus practice and time becomes Knowledge
- Knowledge plus action becomes Wisdom

**Classifying Information by Quality**

- Form: is the data in a usable format, is it free of errors and noise
- Accessibility: where is the data located, how freely can you use it, do you have access when needed
- Relevance: does it describe the right things (time frame), does it describe them the right way (granularity)
- Validity: how credible is the source (example: cia.gov vs a random unofficial site)

---

## 2. Hardware and Software

**Computer Chips and Semiconductors**

- Semiconductor: a substance like silicon dioxide used in most computer chips, capable of both enabling and inhibiting the flow of electricity

**Moore's Law**

- Original (1965): the number of transistors on a computer chip doubles roughly every two years
- Modern interpretation: for the same money, in about eighteen months you can buy chips that are twice as fast or store twice as much
- Discussion point: does Moore's Law apply outside semiconductors, is it dead, how has Apple revived it

**Software Types**

- System Software: runs in the background underneath other programs
    - BIOS: base level commands controlling a hardware device, loads the OS
    - Embedded Systems: special purpose software built into physical products, often on firmware
    - Operating System: controls the hardware and sets standards for developing and running applications
    - Utilities: programs like antivirus or disk optimization tools
- Application Software: performs specific tasks for users
    - Desktop software: installed on a personal computer, usually single user
    - Enterprise software: serves multiple users across an organization
    - Apps: smaller software built for a specific platform

**Enterprise Software Categories**

- Supply Chain Management (SCM)
- Customer Relationship Management (CRM)
- Enterprise Resource Planning (ERP)

**Supply Chain Management**

- Just in time production and delivery (examples: GM, Target)
- Risk of too many items: inventory cost, obsolescence
- Risk of too few items: assembly line shutdowns, retail stock outs
- Information partnerships (example: Staples and UPS)

**Customer Relationship Management**

- Manages and tracks interactions with customers across channels
- Converts customer information into insight (needs, wants, behaviors)
- Integrates customer facing processes: sales force automation, customer service and support, marketing campaign management and analysis

**Enterprise Resource Planning**

- A suite of integrated software for managing essentially everything in the business
- Unified interface
- Centralized data
- Modular design

**IT Infrastructure and Networks**

- IT infrastructure: physical and virtual resources, systems, and technologies supporting delivery of IT services, including hardware, software, and networking
- Network: two or more computers sharing information, software, peripherals, and or processing power, the fundamental base of any IT environment

**Network Types**

- Decentralized: little sharing, everyone has their own resources
- Centralized: everything lives in one place (example: early mainframes)
- Distributed: information, devices, and processing power shared across a network, computers in different locations can communicate

**Servers and Clients**

- Server (hardware): a computer configured to support requests from other computers (examples: Dell, IBM, HP)
- Server (software): a program that fulfills requests (example: Apache web server)
- Client: a computer or program that makes requests from a server
- Client/Server System: a distributed network where one or more computers act as servers to client computers
- Multitiered System: a generalization of client/server where different computers have different roles or ranks

**APIs and Web Services**

- API: programming hooks or guidelines published by firms telling other programs how to get a service to perform a task, such as sending or receiving data (example: Amazon APIs letting developers place orders programmatically)
- Web Services: software systems that support interoperable machine to machine interaction over a network
- Data interchange formats like EDI, XML, and JSON help exchange data between applications

**Cloud Computing**

- Delivery of resources (application software, processing power, storage, backup, development tools) as services over the internet
- Virtualization: software letting one computer or cluster act as several computers, each running its own OS and software, this underpins cloud computing
- Advantages: lower capital expenditures, immediate access to a broad range of software, real time scalability, reduced maintenance costs

---

## 3. Telecommunications

**The Internet as Infrastructure**

- The internet functions like a wire connecting devices
- Discussion point: is your computer connected directly to the internet, and why might high frequency trading firms care about the path in between

**The World Wide Web**

- The internet is the wire, the World Wide Web is the globally linked system of pages and content on servers, accessed by browsers, all connected to that wire
- The internet is a network of networked devices allowing any computer to request and receive files from any other connected computer
- Communication between devices answers three questions: what are you looking for, where is it, how do we get there

**Protocols**

- A protocol like HTTP or FTP defines the format of data and rules for exchange, similar to grammar and vocabulary in a spoken language
- Protocols are independent of hardware and software
- Over 95 percent of the web now supports SSL encryption, the S in HTTPS

**URLs**

- The URL answers "what are you looking for"
- Each part of the URL carries information about the target file (protocol, host, domain, directory, file name)

**IP Addresses and DNS**

- The IP address answers "where is it," every device connected to the internet has one
- IP addresses are assigned whenever and wherever you access the internet
- DNS (Domain Name Service) answers "how do we get there," working like a collection of phone books called nameservers that match domain names to IP addresses

**TCP and IP**

- TCP (Transmission Control Protocol): slices data into packets at the source, labels them with source and destination addresses, and reassembles them at the destination
- IP (Internet Protocol): routes packets across the internet, wrapping them with routing information
- A router connects networks and exchanges data between them, every computer connects to a router and routers connect to each other
- UDP: a faster but lower quality alternative to TCP, useful when speed matters more than reliability

**Backbone and Last Mile**

- Internet Backbone: high speed fiber optic cables carrying data over long distances
- Bandwidth: network transmission speed, usually measured in bits per second
- Last Mile: the technologies connecting end users to the internet (cable, DSL, fiber, wireless, satellite), usually the slowest part of the network

**Net Neutrality**

- The principle that all internet traffic should be treated equally, with no discrimination by ISPs based on user, content, site, platform, application, equipment, or communication mode
- Discussion point: arguments for and against net neutrality

---

## Related Notes

- [[Porter 5 forces - MIS 382]]
- [[Apple Supply Chain in class - SCOM 465]]

