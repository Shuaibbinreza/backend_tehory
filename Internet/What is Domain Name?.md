## 🌐 What is a Domain Name?

**Definition:**  
A domain name is a **human-readable address** used to access websites on the Internet (e.g., `mozilla.org`) instead of using hard-to-remember IP addresses (e.g., `192.0.2.172`).

---

## 🧩 Structure of a Domain Name

**Format:**  
`subdomain.secondary-level-domain.top-level-domain`

**Example:**  
`developer.mozilla.org`

- `org` → **TLD (Top-Level Domain)** – `.com`, `.org`, `.edu`, `.bd`
- `mozilla` → **SLD (Secondary Level Domain)** – your actual domain name
- `developer` → **Subdomain** – optional, used to organize content

---

## 🛒 Buying a Domain Name

- You **don’t own** a domain forever — you **rent** it yearly.
- Use a **domain registrar** (e.g., Namecheap, GoDaddy).
- You can **renew** to keep it.
- Example:
  - You want `afunkydomainname.org`.
  - You check using `whois afunkydomainname.org`.
  - If it's **NOT FOUND**, it’s available to register.

---

## 🧭 DNS (Domain Name System)

- DNS maps a **domain name** to its **IP address**.
- Process:
  1. You type `mozilla.org`.
  2. Browser checks local DNS cache.
  3. If not found, it queries a **DNS server**.
  4. The DNS server returns the matching IP.
  5. Browser uses that IP to load the site.

**Example:**  
Typing `google.com` → DNS finds IP → Browser connects to `142.250.64.110`.

---

## 🗂️ DNS Refreshing

- DNS info is stored temporarily (cached).
- If domain data changes (e.g., new IP), DNS servers update after a delay.
- These updates come from **authoritative name servers**.

---

## 🔎 Domain Availability Check

Use:
- Registrar websites (with search or "whois" tool)
- Terminal command:  
  ```bash
  whois mozilla.org
  ```

---

## 📝 Key Points

| Term         | Description                          | Example             |
|--------------|--------------------------------------|---------------------|
| Domain Name  | Human-readable address                | `example.com`       |
| TLD          | Top-level domain                      | `.org`, `.bd`       |
| SLD          | Main domain (before TLD)              | `example` in `example.com` |
| Subdomain    | Part before SLD, optional             | `blog.example.com`  |
| Registrar    | Company that manages domain names     | Namecheap, GoDaddy  |
| DNS Server   | Translates domain to IP               | `mozilla.org` → `192.0.2.172` |

---

## 🔗 Relationship Between Domain Name and URL

### ✅ **Domain Name**  
A **domain name** is the **main human-readable address** of a website — it identifies the location of a website on the Internet.

**Example:**  
`google.com`, `wikipedia.org`, `shuaib.dev`

### ✅ **URL (Uniform Resource Locator)**  
A **URL** is the **complete web address** used to access a specific resource (like a page, image, or file) on a website.

**Structure of a URL:**
```
protocol://subdomain.domain.tld/path?query=string#fragment
```

**Example URL:**
```
https://developer.mozilla.org/en-US/docs/Web/HTML
```

- **Protocol**: `https://`
- **Domain Name**: `developer.mozilla.org`
- **Path**: `/en-US/docs/Web/HTML`

---

## 🧠 In Simple Terms:

> A **domain name** is a part of a **URL**.

### 📌 Think of it like this:
- **Domain name = Home address** 🏠
- **URL = Full direction to a room in your house** 🛏️

---

## 💡 Scenario Example

Let’s say you’re looking for a recipe on a cooking website.

- 🔍 You go to:  
  `https://cookmaster.com`

This is the **domain name** → it's like entering the house.

- 🍲 You click on a recipe page:  
  `https://cookmaster.com/recipes/chicken-biryani`

This is the **URL** → it takes you to a specific room (recipe page) inside the house (website).

---

## ✅ Summary Table

| Component     | Example                             | Description                             |
|---------------|-------------------------------------|-----------------------------------------|
| Domain Name   | `cookmaster.com`                    | Base name of the website                |
| URL           | `https://cookmaster.com/recipes/chicken-biryani` | Full web address to a resource          |
| Relationship  | Domain name is **part of** the URL  | URL = Protocol + Domain + Path, etc.    |

---

