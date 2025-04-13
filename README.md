# Internet Fundamentals

---

## **1. What is the Internet?**

The Internet is a global network of interconnected computers and devices that communicate using a set of standardized protocols.

It enables users to access and share information across the world using technologies like the World Wide Web, email, file sharing, and more.

---

### Key Concepts of Internet

---

### **1. IP Address (Internet Protocol Address)**

**What it is:**  
A unique number assigned to every device connected to the internet.  
It’s like your home address, but for your computer or phone on the internet.

**Example:**  
- IPv4: `192.168.0.1`  
- IPv6: `2001:0db8:85a3:0000:0000:8a2e:0370:7334`

**Why it's important:**  
When you visit a website, your browser needs to know where to go.  
Websites also have IP addresses — the IP tells your browser exactly which computer (server) to talk to.

---

### **2. DNS (Domain Name System)**

**What it is:**  
A translator or phonebook for the internet.  
Converts human-friendly names (like `www.google.com`) into IP addresses (`142.250.190.36`).

**Why it matters:**  
You don’t need to memorize numbers.  
Without DNS, you’d have to remember IP addresses instead of website names!

---

### **3. Client and Server**

**What it is:**  
- **Client:** Your computer or phone (the device that asks for information).  
- **Server:** The powerful computer that stores websites or apps (the device that gives information).

**Real-world analogy:**  
You (client) go to a restaurant and order food.  
The kitchen (server) prepares and serves the food.

---

### **4. HTTP / HTTPS (HyperText Transfer Protocol)**

**What it is:**  
A set of rules used to transfer data over the internet.  
- `HTTP` = sends data  
- `HTTPS` = secure version (adds encryption)

**Why it matters:**  
When you open a website, your browser sends an HTTP request.  
The server responds with an HTTP response (the webpage you see).

**HTTPS protects:**  
- Passwords  
- Credit cards  
- Personal data  

Uses **SSL/TLS** encryption to make the connection secure.

---

### **5. Packets**

**What it is:**  
Data you send/receive over the internet is broken into tiny chunks called **packets**.

**Analogy:**  
Sending a long letter in small envelopes — the receiver puts the pieces back together.  
Even videos, images, and text are sent as packets.

---

### **6. Routers and Switches**

**What they are:**  
Devices that help direct traffic on the internet.

- **Routers:**  
  - Connect multiple networks  
  - Guide packets from one place to another

- **Switches:**  
  - Connect devices within a local network (like inside your home or office)

---

### **7. Undersea Cables and Satellites**

**What they are:**  
- Huge fiber-optic cables under oceans that connect countries  
- Satellites are used too, especially in remote places

**Why important:**  
They carry most of the world’s internet traffic.  
Without them, global websites wouldn't load!

---

### **8. Encryption**

**What it is:**  
A way to scramble data so that only the intended recipient can read it.

**Why it matters:**  
Protects your personal data — especially important for banking, emails, passwords.

---

### Note: Imagine You Want to Visit a Website

Let’s say you want to visit `www.google.com`. Here’s what happens step by step:

1. **You = The User**  
   You open your browser (like Chrome or Safari) and type `www.google.com`.

2. **Step 1: Ask for the Address (DNS)**  
   Your browser doesn’t know where Google lives, so it asks a special phonebook called DNS:  
   _"Hey, what is the address (IP address) of www.google.com?"_  
   DNS replies:  
   _"The address is 142.250.190.36"_

3. **Step 2: Go to the Address (Connect)**  
   Your browser sends a request to that address, like a car driving to Google’s house.

4. **Step 3: Request the Page**  
   Your browser knocks on the door:  
   _"Hey Google! Can you give me your homepage?"_

5. **Step 4: Google Sends the Page**  
   Google replies:  
   _"Sure! Here’s the homepage."_  
   (It sends HTML, images, buttons, etc.)

6. 🖥**Step 5: Your Browser Shows It**  
   Your browser puts all the pieces together and shows you the Google page on your screen.

---

## **2. What is HTTP?**

**HTTP** stands for **HyperText Transfer Protocol**.

It is the foundation of data communication on the World Wide Web.  
When you visit a website in your browser, your device and the website’s server use HTTP to communicate.

---

### 🍽️ Example: Think of it Like This

- **You = The Client (Browser)**  
- **Restaurant = The Server (Website)**

- You ask for a menu → Like browser requesting a page using HTTP  
- The waiter brings the food → Like website sending back the page  
- You enjoy your meal → You see the website!

---

### How HTTP Works Step-by-Step

1. You type `www.example.com` in your browser  
2. Browser sends an **HTTP request** to the server  
3. Server processes the request  
4. Server sends back an **HTTP response** (web content)  
5. Browser shows the page on your screen

---

### 🛠️ Common HTTP Methods

- `GET` : Requests data from a server  
- `POST` : Sends data to a server  
- `PUT` : Updates data on a server  
- `DELETE` : Deletes data from a server  
- `PATCH` : Partially updates data

---

## **3. What is HTTPS?**

**HTTPS** stands for **HyperText Transfer Protocol Secure**.  
It’s the secure version of HTTP.

---

### Simple Explanation

Imagine:  
You’re sending a private letter (like a password or credit card) to a website.

- With **HTTP**, anyone can read the letter  
- With **HTTPS**, the letter is locked in a safe only the website can open

That’s **encryption** — it keeps your data safe.

---

### **3.1 What Makes HTTPS Secure?**

HTTPS adds security using three things:

1. **Encryption**   
   - Scrambles data so no one else can read it

2. **Authentication**   
   - Proves the website is real (using SSL certificates)

3. **Data Integrity** 
   - Makes sure the data isn’t changed in transit

---

### **3.2 What is SSL/TLS?**

Websites use **SSL certificates** (or TLS) to make HTTPS work.

- **SSL = Secure Sockets Layer**  
- **TLS = Transport Layer Security** (newer and better)

**What it does:**  
- Proves the website is real  
- Starts encryption between browser and server

Technically:  
`HTTPS = HTTP + SSL/TLS`

---

### **3.3 How to Know a Site Uses HTTPS?**

Look in your browser’s address bar:

Lock icon 🔒  
URL starts with `https://`

**Examples:**
- `https://www.google.com` (Secure)
- `http://example.com` (Not secure)

---

### Real Life Example

Visit: `https://www.amazon.com`  
Enter your credit card.

**Result:**  
Your data is encrypted. Only Amazon can read it.  
No Wi-Fi provider, ISP, or hacker can steal it.

---

## **4. What is a Domain Name?**

A **domain name** is the human-friendly address you type in your browser.

**Examples:**  
- `www.google.com`  
- `youtube.com`  
- `facebook.com`

---

### Simple Analogy

- **Real World:**  
  A house has a street address (`123 Main St`)

- **Internet World:**  
  A website has an IP address (`142.250.190.68`)  
  But instead, we use a domain name like `google.com`

---

### **4.1 How Domain Names Work**

1. You type `www.google.com`  
2. Browser asks DNS for its IP  
3. DNS replies with something like `142.250.190.68`  
4. Browser connects to that IP and loads the site

Domain names make it easy for humans to browse without memorizing numbers.

---

### **4.2 Parts of a Domain Name**

Take `www.example.com`:

- `www` : Subdomain  
- `example` : Main domain  
- `.com` : Top-Level Domain (TLD)

---

## **5. What is DNS?**

**DNS** stands for **Domain Name System**.  
It’s like the **phonebook** of the internet.

It translates domain names (like `google.com`) into IP addresses (`142.250.190.78`).

---

### Real Life Analogy

You want to call “John”, but you only know his name.

- You look up “John” in your contacts  
- Phone finds his number  
- You call him!

Same with DNS:

- You type `facebook.com`  
- DNS finds the IP  
- Browser connects to it

---

### **5.1 DNS Steps**

1. You type `example.com`  
2. Computer asks resolver: “What’s the IP?”  
3. Resolver queries:  
   - Root Server  
   - TLD Server  
   - Authoritative Server  
4. DNS returns IP like `93.184.216.34`  
5. Browser opens the website

---

## **6. What is a Web Browser?**

A **web browser** is an application (Chrome, Firefox, Safari, Edge) that lets you view and interact with websites.

You type `www.google.com` → browser loads Google’s homepage → you interact.

---

### Main Job of a Browser

- Accept web address (e.g., `https://example.com`)  
- Get website files from the internet (HTML, CSS, JS)  
- Understand those files  
- Display the website nicely

---

### **6.1 How Does a Browser Work? (Step-by-Step)**

Example: You type `www.wikipedia.org`

1. **DNS Lookup**  
   - Browser says: “Where is `wikipedia.org`?”  
   - DNS gives IP: `208.80.154.224`

2. **Make HTTP/HTTPS Request**  
   - Browser asks: “Give me the homepage!”

3. **Server Response**  
   - HTML (structure)  
   - CSS (styles)  
   - JS (interactivity)  
   - Images, fonts, etc.

4. **Render Page**  
   - Parse HTML → Build DOM  
   - Apply CSS  
   - Run JS  
   - Paint screen → You see the page

---

### **6.2 What Happens When You Press Enter in the Browser?**

- DNS lookup for domain  
- Send HTTPS request to server  
- Server replies with HTML  
- Browser fetches CSS, JS, images  
- Renders and displays the page
