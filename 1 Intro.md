# Before we get started...
## How the web works
- Web Pages - Basic Components (HTML, CSS, JS)
- Websites - Interconnected Pages
- Web App - Website relying on dynamic, user-generated data

## **URL and Web Addresses**
- Uniform Resource Locator 
	- https://www.google.com
- _http://__ - Hypertext Transfer Protocol
	- Set of rules that defines how information is exchanged between a client (like a web browser) and a web server
        - It specifies the format of the messages that are sent between them
        - Has two main methods attached to it: GET and POST
            - We'll be using and learning more about them in later workshops!
- _www_ - World Wide Web   
    - subdomain to indicate that the web server/ page is in the World Wide Web
        - Optional in modern browsers
        - Historically used to distinguish websites from other types of internet services like FTP (File Transfer Protocol) or Gopher servers (Search it up if you're curious!)
- _google_ - Web server or site maintainer  
    - The ones responsible for hosting the content
- _com_ - Commercial site
    - The top-level domain, indicates the type or purpose of the website
    - .com is originally for commercial entities, but it became the most used and recognized domain extension; used by individuals, businesses, and organizations alike
	    - Other top-level domains: .org, .net, .edu


---

# Client-Server Architecture
A fundamental design pattern where processes are divided between the client and server components
- For efficient communication and resource management
- Basically, divide the tasks to specialized components so they get done faster
![[Pasted image 20231106232658.png]]
### **Presentation Tier**
- Clients presenting info from the servers
- Devices showing apps, websites, etc.
### **Application Tier**
- Contains application servers
- Processing and managing app logic
    - Validation, computing
    - Getting stuff from the database and doing computations
### **Data Tier**
- Contains database Server
- Responsible for storing, retrieving, and managing data
- Security implementations are necessary

When making a website, you will have to touch on all 3 layers!


---

# The Big 3...
Every webpage lives and breathes by 3 main components

## **HTML**
- Structure and Content
- The bones of the webpage    
- Doesn't look good, but that's what CSS is for
## **CSS**
- Aesthetics
- The skin and unique features of the webpage
    - 2 websites can have the exact same HTML yet look wildly different because of CSS
## **JS**
- JavaScript
- The logic or mind of the webpage
- Makes the webpage move and interact with other stuff (data, other webpages, databases, etc.)