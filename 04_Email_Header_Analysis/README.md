# Experiment 04: Email Header Analysis & Spoofing Detection

## Objective
To analyze email headers and detect possible email spoofing using the Mail Header Analyzer (MHA).

---

## Tools Used
- Mail Header Analyzer (MHA)
- Email Clients (Gmail, Outlook, Yahoo, etc.)
- MXToolbox / G Suite Toolbox

---

## Procedure
1. **Access the Email Header**
   - Gmail → Open email → More options (⋮) → *Show original*  
   - Outlook → File → Properties → *Internet headers*  
   - Yahoo → More (⋮) → *View raw message*

<img width="1631" height="514" alt="Image" src="https://github.com/user-attachments/assets/61c1e415-dda1-4fe3-a73a-467ef5c925b0" />

2. **Copy the Email Header**
   - Extract the full header text.  
   - This contains metadata such as From, To, Received, Message-ID, SPF, DKIM, and DMARC.

<img width="1596" height="872" alt="Image" src="https://github.com/user-attachments/assets/5b93d46c-9a4f-4293-9bfb-314f68c37179" />

3. **Analyze Key Fields**
   - **From:** Sender’s email address  
   - **To:** Recipient’s email address  
   - **Received:** Servers the email passed through (important for tracing origin)  
   - **Return-Path:** Bounce address  
   - **Message-ID:** Unique identifier for the email  
   - **SPF / DKIM / DMARC:** Authentication checks

<img width="1088" height="697" alt="Image" src="https://github.com/user-attachments/assets/c14e7010-77b1-446a-bf56-fa0839a84fdc" />

4. **Check the ‘Received’ Fields**
   - Verify each server hop in reverse order (last server to first).  
   - Look for mismatched IPs or unexpected hostnames.

<img width="1011" height="632" alt="Image" src="https://github.com/user-attachments/assets/5ce24a13-8cc8-4280-9d52-c7783e22370b" />

5. **Authentication Results**
   - SPF → Ensures the sending server is authorized.  
   - DKIM → Confirms message content was not altered.  
   - DMARC → Ensures alignment between SPF/DKIM.  

<img width="1816" height="878" alt="Image" src="https://github.com/user-attachments/assets/efe498a1-0691-4c4b-a2d5-103e1b4630cd" />

6. **Look for Anomalies**
   - Mismatched domains in From, Return-Path, or Message-ID.  
   - Suspicious or unknown IP addresses.  
   - Abnormal timestamps.  

<img width="1872" height="870" alt="Image" src="https://github.com/user-attachments/assets/e01bdf27-def3-40b6-b415-c1135b926d02" />

---


## Result
- Successfully extracted and analyzed email headers using MHA.  
- Identified anomalies in SPF/DKIM/DMARC results that indicate possible spoofing.  
- Documented suspicious IPs and mismatched domains.  

<img width="1853" height="862" alt="Image" src="https://github.com/user-attachments/assets/01d7d1e5-f20c-4a96-ae8c-0d6cba80f808" />

<img width="1875" height="873" alt="Image" src="https://github.com/user-attachments/assets/760bacec-9327-479e-99a2-f2cfdc99a2bf" />

---

## Conclusion
Email header analysis is a crucial step in digital forensics to detect spoofing and phishing attempts. By examining header metadata, authentication mechanisms, and server hops, investigators can trace email origins and validate authenticity.
