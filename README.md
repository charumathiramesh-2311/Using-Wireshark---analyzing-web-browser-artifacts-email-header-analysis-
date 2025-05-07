# Using-Wireshark---analyzing-web-browser-artifacts-email-header-analysis
## AIM:
To use Wireshark to analyze web browser activities and inspect email headers from captured network traffic.

## DESIGN STEPS:
### Step 1:
Launch Wireshark and start capturing traffic on the appropriate network interface.

### Step 2:
Use filters like http, dns, or tcp.port == 80 to monitor web browser artifacts such as visited URLs, cookies, and user-agent strings.

### Step 3:
Apply filters like smtp, pop, or imap to locate and analyze email header details (e.g., sender, receiver, subject) from email communications.

## PROGRAM:
Wireshark Web and Email Traffic Filtering Steps

## OUTPUT:
Captured Web Activity and Email Header Information

1.Open Wireshark and start capturing on the active interface (Wi- Fi/Ethernet).

2.Perform activities like opening a website or sending an email through a client (e.g., Gmail via browser or Thunderbird).

3.Stop the capture once done.

![image](https://github.com/user-attachments/assets/f1ce5123-5dd3-4294-9515-5d9207e38c8f)

Analyzing Web Browser Artifacts
Analyze Queries:
-> Filter: http

![image](https://github.com/user-attachments/assets/6b3fcd64-89c3-4e24-b1f2-a37b331a584b)

Filter: tcp

![image](https://github.com/user-attachments/assets/333291ae-c0bd-48ca-95e7-1bb08159429d)

Inspect HTTP GET/POST requests

![image](https://github.com/user-attachments/assets/6ee7ac8f-5808-4b99-aa59-b203063321b8)

Analyze dns Queries:

![image](https://github.com/user-attachments/assets/6f432f48-dc48-4ae6-870b-2d91c9238a6e)

Email Header Analysis
Apply relevant filters
![image](https://github.com/user-attachments/assets/ad52da62-6b7b-4376-8b02-36e29457f144)

Locate email data

Look for SMTP packets to see sender/receiver email addresses. Use "Follow TCP Stream" to view the full email headers and body if unencrypted.

Extract Email Header Fields Analyze From, To, Subject, Date, Message-ID, and relay servers used in sending the email.

![image](https://github.com/user-attachments/assets/84154527-84a5-40e8-910e-fade4828cbf5)



## RESULT:
Web browser artifacts and email headers were successfully analyzed using Wireshark.

