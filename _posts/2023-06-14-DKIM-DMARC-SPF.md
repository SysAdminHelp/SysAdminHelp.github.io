## What are DKIM/DMARC/SPF for?
DKIM, DMARC, and SPF are essential email security protocols that combat phishing and spoofing attacks. Let's explore their roles and how they utilize DNS for enhanced security. These technologies have a very heavy reliance on Domain Name Services.

## Explanation of each technology 
DKIM (DomainKeys Identified Mail):
DKIM adds a digital signature to emails, ensuring integrity and authenticity. For example, a small or medium-sized business signs outgoing emails with a private key. Recipients' mail servers verify the signature by retrieving the corresponding public key from a DKIM record in DNS, confirming the email's integrity.

DMARC (Domain-based Message Authentication, Reporting, and Conformance):
DMARC combines SPF and DKIM to establish policies for handling authentication failures. The business publishes a DMARC record in DNS, specifying actions like quarantining or rejecting failed emails. DMARC also provides valuable reports on authentication results and abuse.

SPF (Sender Policy Framework):
SPF verifies authorized email servers. The small or medium-sized business publishes an SPF record in DNS, listing approved servers. When recipients receive emails, their mail servers check the SPF record to validate the sender's authenticity, preventing spoofing and phishing.

## Conclusion
DKIM, DMARC, and SPF are vital for robust email security. DKIM ensures integrity, DMARC enforces policies and collects reports, and SPF validates authorized servers. By implementing these protocols and leveraging DNS, small or medium-sized businesses can enhance their email security and protect against malicious attacks.
