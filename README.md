# Secure Software Implementation – Artemis Financial

This repository contains my completed artifact for the Practices for Secure Software report created as part of my coursework in CS-305: Software Security. It demonstrates how I refactored an existing Spring Boot application to implement secure communications using SSL/TLS and cryptographic hash functions. The project is based on the needs of a fictional client, Artemis Financial.

## 📄 Artifact: Practices for Secure Software Report

The selected artifact for this portfolio submission is the **Practices for Secure Software Report** from Project Two. It showcases my ability to identify software vulnerabilities, apply cryptographic hashing, enable HTTPS using self-signed certificates, and verify that my refactoring did not introduce any new vulnerabilities.

---

## 🧠 Reflection

### Who was the client and what issue did they want solved?

The client was **Artemis Financial**, a company that develops personalized financial plans for its customers. Their goal was to modernize their application and implement secure mechanisms to protect customer financial data during transmission. Specifically, they requested a file verification step using a checksum and the addition of HTTPS support.

### What did I do well in securing the code?

I successfully implemented a SHA-256 checksum generation endpoint and configured the app to use HTTPS by creating and integrating a self-signed SSL certificate. These changes ensure that both data integrity and secure transmission are enforced. Secure coding helps prevent data breaches, strengthens trust, and upholds regulatory compliance—critical for any financial service.

### What part of the vulnerability assessment was most helpful or challenging?

The most helpful part was learning to use the **OWASP Dependency Check** tool to detect known CVEs in third-party libraries. The challenge was reviewing and distinguishing between inherited vulnerabilities and those introduced by new code.

### How did I increase layers of security?

I increased security by:
- Adding a hash-based file verification step
- Using SSL to encrypt traffic
- Ensuring no insecure HTTP endpoints remained active

In future projects, I would use tools like OWASP ZAP, Snyk, and static analyzers like SonarQube to evaluate vulnerabilities and help decide on mitigation strategies.

### How did I ensure the application remained functional and secure?

After refactoring, I manually tested the new `/hash` endpoint over HTTPS and verified expected output. I ran the dependency check again to confirm that **no new vulnerabilities** were introduced during the update.

### What resources or practices were helpful?

The most helpful practices included:
- Using the `keytool` CLI to generate SSL certificates
- Relying on Maven for dependency management and static security testing
- Following Spring Boot best practices for `application.properties` security configuration

These are skills I will apply to future work with secure web services.

### What would I show a future employer from this assignment?

I would show:
- My ability to integrate SSL and cryptographic hashing into a Java web application
- The vulnerability scan report before and after refactoring
- Screenshots of the functional app over HTTPS
- The written technical report that documents secure software practices

This project demonstrates both technical skills and the ability to communicate about software security clearly and professionally.

