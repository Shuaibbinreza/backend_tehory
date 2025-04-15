
## 🌐 What is DNS?

**DNS (Domain Name System)** is like the **phonebook of the Internet**. It translates **human-readable domain names** (like `www.google.com`) into **machine-readable IP addresses** (like `142.250.186.100`) so browsers can load websites.

> 💡 Think of DNS as a translator between what humans type and what computers understand.

---

## ⚙️ How DNS Works (Step-by-Step)

Here’s what happens when you type `www.example.com` in your browser:

---

### **Step 1: DNS Query Initiation**
- You type `www.example.com` in your browser and hit Enter.
- Your computer checks its **local DNS cache** to see if it already knows the IP address.
- If not, it begins a **DNS query** to find out.

---

### **Step 2: Ask the Recursive Resolver**
- Your computer asks a **DNS Recursive Resolver** (usually provided by your ISP or a public DNS like Google `8.8.8.8`).
- The resolver’s job is to find the IP address on your behalf.

---

### **Step 3: Root DNS Server Lookup**
- If the resolver doesn't have the answer, it asks a **Root DNS Server**.
- Root servers don’t know exact IPs, but they know **which Top-Level Domain (TLD) server** to ask (e.g., `.com`, `.org`, etc.).

---

### **Step 4: TLD DNS Server Lookup**
- The resolver is redirected to the **TLD Server** (e.g., for `.com` domains).
- This server tells the resolver **where to find the authoritative DNS server** for `example.com`.

---

### **Step 5: Authoritative DNS Server**
- The **Authoritative DNS Server** stores the actual IP address of `www.example.com`.
- It responds with something like:  
  `www.example.com → 93.184.216.34`

---

### **Step 6: Return the Result**
- The resolver returns the IP address to your computer.
- Your browser connects to the server at `93.184.216.34` and loads the website.

---

### **Step 7: Caching**
- Your computer stores (caches) this info for next time so it doesn’t need to go through the whole process again.

---

## 📌 Example Scenario

Let’s say you type `www.wikipedia.org` into your browser:

1. Your system asks: “What’s the IP of `www.wikipedia.org`?”
2. The DNS resolver checks its cache. If not found:
3. It asks a **Root DNS Server**: “Where can I find `.org` domains?”
4. Root replies: “Ask the `.org` TLD server.”
5. The TLD server says: “Ask the authoritative server for `wikipedia.org`.”
6. The authoritative server replies:  
   `www.wikipedia.org = 208.80.154.224`
7. Your computer now knows the IP and opens Wikipedia.

---

## 🧠 Important DNS Jargon

| Term | Description |
|------|-------------|
| **DNS** | Domain Name System – maps domain names to IP addresses. |
| **IP Address** | A unique numerical label (e.g., `192.168.1.1`) identifying a device on the network. |
| **Domain Name** | A human-friendly address like `google.com`. |
| **DNS Query** | A request to resolve a domain name to an IP. |
| **Recursive Resolver** | The DNS server that does the lookup for your device. |
| **Root DNS Server** | The starting point that directs queries to TLD servers. |
| **TLD Server** | A server for top-level domains like `.com`, `.org`, `.net`. |
| **Authoritative DNS Server** | The server that holds the actual DNS records (final answer). |
| **DNS Record** | Data in DNS like A (address), CNAME (alias), MX (mail), etc. |
| **A Record** | Maps a domain to an IPv4 address. |
| **CNAME Record** | Maps a domain to another domain name. |
| **MX Record** | Defines mail servers for a domain. |
| **TTL (Time to Live)** | How long a DNS record is cached before refreshing. |
| **DNS Caching** | Temporarily storing DNS responses to speed up repeat visits. |

---

## 🎯 Summary

- DNS translates **domain names to IP addresses**.
- It works like a chain of lookup requests:  
  **Your device → Resolver → Root → TLD → Authoritative → Back to you**
- DNS makes it possible to visit websites using names, not numbers.

---

