# Phishing-Emails-Analysis
Phishing email analysis report using PhishTool with screenshots and threat breakdown.

This project focuses on analyzing a real-world phishing email that impersonates the United Nations, promising a fake grant of £100,000. Through a detailed investigation, the email is classified based on technical and behavioral indicators as Malicious.

The Problem

In today’s digital world, email impersonation is becoming one of the most dangerous forms of phishing. Attackers are no longer sending random spam — they’re crafting messages that look like they’re from trusted organizations, government bodies, or well-known individuals.

One particularly manipulative tactic is the "Authority Impersonation Scam", where emails pretend to come from trusted entities like the United Nations, WHO, or even financial aid programs. Victims are often promised grants, relief funds, or job offers — all fake, but convincing enough to trick unsuspecting recipients into giving up their personal information.

These types of phishing attacks:

Exploit people's trust in global institutions

Create false hope during difficult times (like during economic hardship or crisis)

Bypass technical filters because they don’t always include malware — just persuasive text

This makes them harder to detect, and potentially more damaging — both financially and psychologically — for victims.

Project Goal

This project aims to:

Dissect the technical and behavioral elements of a phishing email

Classify the email as Malicious based on evidence

Understand how attackers craft convincing messages

Develop defensive skills by identifying red flags in real messages

Tool Used

PhishTool – A threat analysis platform used to examine the email's header, content, sender domain, and overall structure. It allowed for an organized breakdown of email metadata and visual evidence of suspicious indicators.

Email Analysis Structure

Each email was analyzed using four core techniques:

Header Analysis

From: familiesgrant@gmail.com — not an official UN domain

Return-Path: sangdeptrai84@gmail.com — another unrelated Gmail account

Originating IP: 209.85.220.41 — a Google IP address; passed SPF but lacks legitimacy due to unrelated domains

SPF/DKIM/DMARC: SPF passed, but no DMARC and neutral DKIM. These settings are either poorly configured or intentionally omitted to aid spoofing

Content Analysis

No official subject line, but the body starts with "Greetings Dear" — a vague and impersonal phrase typical of spam or phishing

Offers £100,000.00 grant and instructs the user to provide personal details like name, reference ID, and contact information

Signed off by Mr. C. Gunness “on behalf of the UN” — a real UN staff name used to increase credibility

Uses an unrelated domain (socialworker.net) for contact — a major red flag

Attachment / Link Analysis

No direct attachment

Prompts the user to contact via an unofficial email and a U.S. phone number. These indirect links are meant to lure the user into a prolonged scam

Behavioral Analysis

Attempts to create urgency by promising a reward and requesting immediate personal data submission

Uses authority (UN affiliation) and emotional appeal (grant opportunity) to manipulate the recipient into trusting the message

Final Verdict

This is a classic example of a Malicious phishing email. Here’s why:

Mismatched and untrusted sender domains

No valid email authentication mechanisms

Requests for sensitive personal data

Psychological manipulation (urgency, impersonation of authority)

Use of a real UN official’s name to build false credibility

Repository Contents

README.txt — This file

screenshots/ — Screenshots taken from PhishTool (headers, email body, indicators)

Report analysis.txt — Structured report summary

Author

Maryam Sulaiman

Why This Matters

Phishing is the number one attack vector in many cyber incidents, especially ransomware and identity theft. Projects like this help defenders and learners:

Understand how phishing works technically and psychologically

Improve phishing detection by practicing real-world analysis

Raise awareness about how simple emails can lead to major security breaches

Call to Action for Organizations:

Enforce SPF, DKIM, and DMARC on email domains

Educate staff continuously to spot social engineering tactics

Use threat detection and phishing protection tools

Encourage reporting without blame when phishing is suspected

By understanding and sharing how phishing works, we can all play a part in reducing its impact.
