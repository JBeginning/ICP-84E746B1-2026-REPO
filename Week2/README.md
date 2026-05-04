# Week 2: Secure Static Website Deployment

## 🎯 Objective
Deploy a globally distributed, high-availability static website while enforcing a security-first architecture.

## 🛠️ Technical Stack
- **Hosting:** Amazon S3 (Simple Storage Service)
- **CDN:** Amazon CloudFront
- **Security:** AWS WAF (Web Application Firewall)
- **Encryption:** SSL/TLS (HTTPS)

## 🛡️ Security Implementation
- **Origin Access Control (OAC):** Restricted S3 bucket access to CloudFront service principals only. Direct public access to the S3 bucket is blocked to prevent origin bypass.
- **Traffic Encryption:** Configured CloudFront to enforce HTTPS, ensuring all data in transit is encrypted.
- **WAF Integration:** Enabled managed rule sets to protect the distribution against common web vulnerabilities (SQLi, XSS).

## 🚀 Key Results
- [x] Successfully deployed `index.html` to a global CDN.
- [x] Verified 100% private S3 origin with "Access Denied" on direct object URLs.
- [x] Confirmed zero-cost alignment with AWS Free Tier.
