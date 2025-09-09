# Credential Harvesting via Social Engineering

## Overview

This project demonstrates how attackers can illegitimately capture users' login details through social engineering techniques. The process involves:

- **Creating a Malicious Website:** Attackers build a fake website that closely mimics a legitimate one.
- **Sending Phishing Emails:** Attackers craft and send emails containing a link to the malicious site, tricking victims into clicking the link.
- **Harvesting Credentials:** When victims enter their login details on the fake site, the credentials are captured and reported back to the attacker.

**This repository is for educational and authorized security testing purposes only.**

## Features

- Malicious website template for credential harvesting
- Phishing email example with embedded malicious link
- Activity reporting once credentials are captured

## How It Works

1. **Setup the malicious website** that looks like a legitimate login page.
2. **Send phishing emails** to targeted users, encouraging them to visit the fake site.
3. **Capture credentials** entered by the victims and log/report them to the attacker.

## Example Attack Flow

1. Victim receives a phishing email with a link to a fake login page.
2. Victim clicks the link and is redirected to the malicious website.
3. Victim enters their login details.
4. The harvester captures the credentials and reports them to the attacker.

## Process Walkthrough

Follow these steps to perform the credential harvesting activity using Kali Linux and the Social Engineering Toolkit (SET):

1. **Launch Social Engineering Toolkit (SET)**
   - Click on the **Application** tab in Kali Linux.
   - Navigate to **Social Engineering Tools**.
   - Click on **Social Engineering Toolkit (root)**.

2. **Authenticate as Root**
   - When prompted, enter your Kali Linux password to proceed.

3. **Select Attack Type**
   - Choose **Social Engineering Attacks** from the SET menu.
   - Select **Website Attack Vectors**.

4. **Choose Credential Harvester Method**
   - Select **Credential Harvester Attack Method**.

5. **Select Web Template**
   - Choose **Web Templates**.
   - For this activity, select the **Google template**.

6. **Confirm IP Address**
   - Take note of the IP address SET provides for hosting the malicious site.
   - Press **Enter** to accept and use the provided IP address.


## Phishing Email Creation

Follow these steps to create and send a phishing email that redirects the victim to your malicious website:

1. **Open Kali Terminal**
   - Launch the terminal on Kali Linux.

2. **Verify Your IP Address**
   - Type `ifconfig` to display and verify your IP address.  
   - Note this IP address, as it will be used in your phishing email link.

3. **Launch Thunderbird**
   - Start Thunderbird from the command line:
     ```bash
     thunderbird
     ```

4. **Set Up Your Email Account**
   - Configure Thunderbird with your existing email account.

5. **Compose a Phishing Email**
   - Create a new email message in Thunderbird.
   - Write a message designed to entice the recipient to click a link (e.g., "Please verify your account by clicking here").

### Steps to Insert the Malicious Link in Thunderbird

1. Click on the **Insert** tab.
2. Select **Link**.
3. Enter the text to display as a link (e.g., `here`).
4. Input the IP address of your malicious website in the link field.
5. Click **OK** to set the link.
6. Send the message to the victim.  
   - For testing purposes, you may send the message to yourself.


## Testing the Activity

To verify that the credential harvesting demonstration is working:

1. **Send a Test Phishing Email**
   - Use the Thunderbird email client on Kali Linux to send a phishing email containing the link to your malicious website (Google template).

2. **Access the Malicious Website**
   - On a test machine or in a separate browser, open the link to the malicious website.

3. **Enter Test Credentials**
   - Enter sample login details on the fake login page.

4. **Check Credential Capture**
   - On your Kali Linux machine, monitor the Social Engineering Toolkit (SET) terminal.
   - You should see the captured credentials displayed in the terminal or saved to a log file, depending on your SET configuration.

> **Note:**  
> Always perform testing in a controlled environment.  
> Never use real credentials or conduct unauthorized tests.
---

> **Note:**  
> Make sure you are working in a controlled lab environment with proper authorization.  
> Only use these methods for educational and authorized security testing.


## Ethical Disclaimer

> **Warning:**  
> This project is intended for educational purposes and for demonstrating security risks.  
> **Do not use this tool for unauthorized or illegal activities. Always obtain proper permission before conducting any security testing.**


## Contact

For questions or feedback, contact [PeterOnyeka-Cyber](https://github.com/PeterOnyeka-Cyber).
