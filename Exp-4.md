# Experiment No. 4: Analyze Email Headers and Detect Email Spoofing Using MHA

## Aim

To analyze email headers using Mail Header Analyzer (MHA), examine the email routing information, verify SPF, DKIM and DMARC authentication, perform IP address investigation using WHOIS, and identify possible signs of email spoofing.

---

## Description

Email headers contain important information about an email, including the sender, recipient, message ID, return path, mail servers, IP addresses and authentication results.

In this experiment, an email received in Gmail is analyzed using an online Mail Header Analyzer (MHA). The header information is examined to understand the email's delivery path and verify its authenticity using SPF, DKIM and DMARC.

---

# Procedure

## 1. Access the Email Header

Open the email in Gmail and view the email received from the sender.

The email used for analysis has the subject:

**"You will be charged for your iCloud+ plan in 5 days"**

The email appears to be from:

**iTunes Store <do_not_reply@email.apple.com>**

<img width="959" height="572" alt="1" src="https://github.com/user-attachments/assets/be6e7a40-8897-4fe8-961f-f66d0dde0719" />


---

## 2. Copy the Email Header

Open the email options in Gmail and select the option to view the original message.

Copy the complete email header containing fields such as:

- From
- To
- Subject
- Return-Path
- Received
- Message-ID
- SPF
- DKIM
- DMARC

The copied header is then used for further analysis using the Mail Header Analyzer.

---

## 3. Identify Key Header Fields

The original message information contains important fields such as:

- **Message-ID:** A unique identifier for the email.
- **From:** iTunes Store `<do_not_reply@email.apple.com>`
- **To:** The recipient's Gmail address.
- **Subject:** You will be charged for your iCloud+ plan in 5 days.
- **SPF:** PASS
- **DKIM:** PASS
- **DMARC:** PASS

<img width="959" height="571" alt="6" src="https://github.com/user-attachments/assets/3b69dee6-645a-4ec4-b3ba-15f1f7571fbc" />


---

## 4. Analyze the Received Fields

The `Received` field shows the servers involved in delivering the email.

The header contains information such as:

- Sending server hostname
- Sending IP address
- Receiving mail server
- SMTP information
- Date and time of delivery

The header shows a connection involving an Apple mail server and Google's mail server.

<img width="728" height="74" alt="4" src="https://github.com/user-attachments/assets/9b79a026-d9d8-46ca-aad5-1d0bc13a6bb3" />


---

## 5. Check for IP Addresses and Hostnames

The IP address identified during the analysis can be investigated using a WHOIS lookup.

The WHOIS result for:

**IP Address: 209.85.220.69**

shows:

- **NetRange:** 209.85.128.0 - 209.85.255.255
- **CIDR:** 209.85.128.0/17
- **NetName:** GOOGLE
- **Organization:** Google LLC (GOGL)
- **NetType:** Direct Allocation

This indicates that the IP address belongs to Google's network.

<img width="551" height="478" alt="3" src="https://github.com/user-attachments/assets/a8489cdd-16fa-4688-9847-b64b0af89a0d" />


---

## 6. Examine SPF, DKIM and DMARC Results

The email authentication results were checked to determine whether the email passed the standard authentication mechanisms.

### SPF

SPF shows:

**PASS with IP 17.23.6.48**

This indicates that the sending IP passed the SPF authentication check.

### DKIM

DKIM shows:

**PASS with domain email.apple.com**

This indicates that the email passed DKIM authentication.

### DMARC

DMARC shows:

**PASS**

This indicates that the email passed the DMARC authentication check.
<img width="464" height="127" alt="5" src="https://github.com/user-attachments/assets/d6ea01f5-e87d-4622-afde-1831d9a7ef0e" />


---

## 7. Analyze the Message-ID

The Message-ID is a unique identifier associated with the email.

The analyzed email contains a Message-ID ending with:

**@email.apple.com**

The sender is also associated with:

**email.apple.com**

The Message-ID and sender domain can therefore be compared during the analysis.

<img width="959" height="571" alt="6" src="https://github.com/user-attachments/assets/c0d37362-614f-4c67-b93c-6841c7350531" />


---

## 8. Look for Anomalies

The email header was checked for possible abnormalities such as:

- Domain mismatch
- Suspicious IP addresses
- Incorrect authentication results
- Unusual mail routing
- Suspicious timestamps
- Mismatch between sender and authentication information

The Mail Header Analyzer shows:

- **DMARC Compliant**
- **SPF Alignment**
- **SPF Authenticated**
- **DKIM Alignment**
- **DKIM Authenticated**

The relay delay shown by the analyzer is approximately **1 second**.

<img width="779" height="429" alt="2" src="https://github.com/user-attachments/assets/6e73b796-fd6f-4a11-a8f3-7e50f45a419f" />


---

## 9. Use Online Tools

The email header was analyzed using **MXToolbox Mail Header Analyzer**.

The analyzer provides information about:

- Email delivery
- DMARC compliance
- SPF authentication
- DKIM authentication
- Relay information
- Mail server path



---

## 10. Document and Report Findings

The results obtained from the email header analysis are summarized below:

| Parameter | Result |
|-----------|--------|
| Sender | iTunes Store |
| Sender Domain | email.apple.com |
| Subject | You will be charged for your iCloud+ plan in 5 days |
| SPF | PASS |
| DKIM | PASS |
| DMARC | PASS |
| DMARC Status | Compliant |
| SPF Alignment | Authenticated |
| DKIM Alignment | Authenticated |
| WHOIS Organization | Google LLC |
| Relay Delay | Approximately 1 second |

---

# Result

The email header was successfully analyzed using Mail Header Analyzer. The Received fields, IP address, Message-ID, SPF, DKIM and DMARC information were examined.

The analyzed email shows **SPF PASS, DKIM PASS and DMARC PASS**, with the MHA result indicating that the message is **DMARC compliant** and both SPF and DKIM are authenticated.

Therefore, based on the analyzed header information, **no clear evidence of email spoofing was identified in the authentication results**.

---

# Conclusion

The experiment demonstrated how email headers can be analyzed to trace email delivery information and verify sender authenticity.

Mail Header Analyzer and WHOIS were used to examine the email routing, IP address ownership and authentication mechanisms. SPF, DKIM and DMARC results were successfully checked to determine the authenticity of the analyzed email.
