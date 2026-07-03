# Part 1 – Introduction to Footprinting

## Objective

I want to learn about the basics of footprinting and how to gather information about a target.
I need to understand what is the difference between active reconnaissance. 
I also want to learn how to get information about a target from publicly available sources.

---

# What is Footprinting?

Footprinting is when you collect information about a target organization or system before you test its security. It is the step in ethical hacking. 
This helps the person doing the testing understand the targets environment. 
Footprinting is like gathering clues about the target.

---

# Types of Footprinting

### Passive Footprinting

You collect information without talking to the target

Examples:

- I use Google Search to find information

- I check WHOIS to see who owns a domain

- I look at Social Media to see what people are saying

- I read Public Documents to learn more

- I check DNS Records to see what is connected

---

### Active Footprinting

You collect information by talking to the target

Examples:

- I use DNS Queries to ask for information

- I use Ping to see if the target is alive

- I use Port Scanning to see what ports are open

- I use Banner Grabbing to see what software is running

---

## 1. Verify Internet Connectivity

### Scenario

Before I start looking for information I need to make sure my system is connected to the internet.

### Command

```bash

ping -c 4 google.com

```

### Description

This command sends four messages to Google to see if I can get a response. If I get a response then I know I have internet access. Footprinting needs internet access to work.

### Screenshot

![Alt text](screenshots/ping-google.png)

---

## 2. Perform a Basic DNS Lookup

### Scenario

I want to find the IP address of a domain name.

### Command

```bash

host openaai

```

### Description

This command shows me the IP addresses that are connected to the domain name. This is important for footprinting because it helps me understand the targets network.

### Screenshot

![Alt text](screenshots/host-openai.png)

---

## 3. Query DNS Information

### Scenario

I want to get information about a domains DNS records.

### Command

```bash

dig google.com

```

### Description

This command asks the DNS server for information about the target domain. It shows me the DNS records, which's useful for footprinting. Footprinting is about collecting information like this.

### Screenshot

![ text](screenshots/dig-google.png)

---

## Key Concepts Learned

- What Footprinting is and why it is important

- Why Footprinting is the first step in ethical hacking

- The difference between Passive and Active Footprinting

- Why looking for information is crucial

- How to check if I have internet access

- How to find the IP address of a domain name

- How to get basic DNS information

---

# Conclusion

In this part, I learned:

- The purpose of Footprinting.
- Passive vs Active Footprinting.
- How to verify internet connectivity using `ping`.
- How to resolve domain names using `host`.
- How to retrieve DNS information using `dig`.






