# Analyst Checklist - Phishing Investigation

## 1. Initial Triage
- [ ] Confirm who reported the email
- [ ] Preserve the original email
- [ ] Identify whether any links were clicked
- [ ] Identify whether credentials were entered
- [ ] Check whether attachments were opened

## 2. Email Header Review
- [ ] Review sender address
- [ ] Review reply-to address
- [ ] Check return-path
- [ ] Review received headers
- [ ] Check SPF, DKIM, and DMARC where available

## 3. Content Review
- [ ] Check for urgency or fear language
- [ ] Check for brand impersonation
- [ ] Check for generic greeting
- [ ] Check for spelling or domain tricks
- [ ] Extract all URLs and domains

## 4. IOC Extraction
- [ ] Sender email
- [ ] Sender domain
- [ ] Reply-to email
- [ ] URLs
- [ ] IP addresses
- [ ] File hashes if attachments exist

## 5. Containment
- [ ] Block sender domain
- [ ] Block URL/domain at proxy or DNS layer
- [ ] Search for similar emails
- [ ] Quarantine matching emails
- [ ] Reset credentials for impacted users
- [ ] Enforce MFA

## 6. Reporting
- [ ] Document findings
- [ ] Map to MITRE ATT&CK
- [ ] Record recommendations
- [ ] Share final report with stakeholders
