# Experiment 04: Email Header Analysis & Spoofing Detection

## Objective
To analyze email headers and detect possible email spoofing using the Mail Header Analyzer (MHA).

---

## Tools Used
- Mail Header Analyzer (MHA)
- Email Clients (Gmail, Outlook, Yahoo, etc.)
- WHOIS / IP Lookup tools
- MXToolbox / G Suite Toolbox

---

## Procedure
1. **Access the Email Header**
   - Gmail → Open email → More options (⋮) → *Show original*  
   - Outlook → File → Properties → *Internet headers*  
   - Yahoo → More (⋮) → *View raw message*

2. **Copy the Email Header**
   - Extract the full header text.  
   - This contains metadata such as From, To, Received, Message-ID, SPF, DKIM, and DMARC.

3. **Analyze Key Fields**
   - **From:** Sender’s email address  
   - **To:** Recipient’s email address  
   - **Received:** Servers the email passed through (important for tracing origin)  
   - **Return-Path:** Bounce address  
   - **Message-ID:** Unique identifier for the email  
   - **SPF / DKIM / DMARC:** Authentication checks

4. **Check the ‘Received’ Fields**
   - Verify each server hop in reverse order (last server to first).  
   - Look for mismatched IPs or unexpected hostnames.

5. **Authentication Results**
   - SPF → Ensures the sending server is authorized.  
   - DKIM → Confirms message content was not altered.  
   - DMARC → Ensures alignment between SPF/DKIM.  

6. **Look for Anomalies**
   - Mismatched domains in From, Return-Path, or Message-ID.  
   - Suspicious or unknown IP addresses.  
   - Abnormal timestamps.  

---

## Example Screenshots
- ![Step 1 - Extract Header](screenshots/exp04_step1_extract_header.png)  
- ![Step 2 - Analyze with MHA](screenshots/exp04_step2_mha.png)  
- ![Step 3 - Check SPF/DKIM/DMARC](screenshots/exp04_step3_authentication.png)  

---

## Result
- Successfully extracted and analyzed email headers using MHA.  
- Identified anomalies in SPF/DKIM/DMARC results that indicate possible spoofing.  
- Documented suspicious IPs and mismatched domains.  

---

## Conclusion
Email header analysis is a crucial step in digital forensics to detect spoofing and phishing attempts. By examining header metadata, authentication mechanisms, and server hops, investigators can trace email origins and validate authenticity.
