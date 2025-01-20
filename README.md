# Burp Suite Match and Replace Rules

This repository contains a comprehensive collection of **Burp Suite Match and Replace rules** for various vulnerability categories. These rules are designed to aid penetration testers and security researchers in efficiently testing web applications for common and advanced vulnerabilities. Each set of rules is tailored to a specific use case and helps in automating the injection of payloads into HTTP requests and responses.

## Table of Contents
- [Introduction](#introduction)
- [Categories and Use Cases](#categories-and-use-cases)
  - [API Testing](#api-testing)
  - [Authentication](#authentication)
  - [Authorization](#authorization)
  - [Broken Access Control](#broken-access-control)
  - [Business Logic Testing](#business-logic-testing)
  - [Command Injection](#command-injection)
  - [CORS (Cross-Origin Resource Sharing)](#cors-cross-origin-resource-sharing)
  - [CSRF (Cross-Site Request Forgery)](#csrf-cross-site-request-forgery)
  - [File Upload](#file-upload)
  - [General Rules](#general-rules)
  - [GraphQL](#graphql)
  - [Host Header Injection](#host-header-injection)
  - [HTML Injection](#html-injection)
  - [IDOR (Insecure Direct Object Reference)](#idor-insecure-direct-object-reference)
  - [JWT (JSON Web Token)](#jwt-json-web-token)
  - [LFI (Local File Inclusion)](#lfi-local-file-inclusion)
  - [NoSQL Injection](#nosql-injection)
  - [OAuth Testing](#oauth-testing)
  - [Open Redirect](#open-redirect)
  - [Privilege Escalation](#privilege-escalation)
  - [RFI (Remote File Inclusion)](#rfi-remote-file-inclusion)
  - [SQL Injection](#sql-injection)
  - [SSRF (Server-Side Request Forgery)](#ssrf-server-side-request-forgery)
  - [SSTI (Server-Side Template Injection)](#ssti-server-side-template-injection)
  - [WAF General Rules](#waf-general-rules)
  - [WAF Bypass Payloads](#waf-bypass-payloads)
  - [Web Cache Poisoning](#web-cache-poisoning)
  - [XSS (Cross-Site Scripting)](#xss-cross-site-scripting)
  - [XXE (XML External Entity)](#xxe-xml-external-entity)
- [How to Use](#how-to-use)
- [Contributing](#contributing)
- [License](#license)

---

## Introduction

The **Burp Suite Match and Replace rules** provided in this repository are intended to help security testers automate their workflow when testing web applications. These rules enable users to modify HTTP requests and responses dynamically, allowing them to inject payloads into headers, parameters, cookies, and more.

Each category includes payloads and rules specific to a particular vulnerability type, ensuring comprehensive test coverage.

---

## Categories and Use Cases

### API Testing
- Modify headers and parameters to test API endpoints for security misconfigurations and vulnerabilities.

### Authentication
- Rules to test login mechanisms, multi-factor authentication, and session handling.

### Authorization
- Validate access controls by injecting invalid or unauthorized identifiers.

### Broken Access Control
- Test for improper access restrictions using custom payloads.

### Business Logic Testing
- Inject custom payloads to test for flaws in application workflows.

### Command Injection
- Payloads to test for OS command injection vulnerabilities.

### CORS (Cross-Origin Resource Sharing)
- Rules to test CORS configurations for security weaknesses.

### CSRF (Cross-Site Request Forgery)
- Inject anti-CSRF token bypass techniques and test token validation mechanisms.

### File Upload
- Test file upload functionality for insecure handling and bypass techniques.

### General Rules
- Basic rules to test general application security.

### GraphQL
- Inject payloads to test GraphQL endpoints for security issues like over-fetching or unauthorized access.

### Host Header Injection
- Test applications for host header injection vulnerabilities.

### HTML Injection
- Payloads to test for insecure rendering of HTML content.

### IDOR (Insecure Direct Object Reference)
- Test for IDOR vulnerabilities in applications exposing sensitive object references.

### JWT (JSON Web Token)
- Inject payloads to test for vulnerabilities in JWT handling and verification.

### LFI (Local File Inclusion)
- Payloads to test for file inclusion vulnerabilities in local file systems.

### NoSQL Injection
- Rules to test NoSQL databases for injection vulnerabilities.

### OAuth Testing
- Test OAuth implementations for misconfigurations and vulnerabilities.

### Open Redirect
- Test applications for insecure redirection mechanisms.

### Privilege Escalation
- Test for unauthorized access leading to privilege escalation.

### RFI (Remote File Inclusion)
- Payloads to test for remote file inclusion vulnerabilities.

### SQL Injection
- Rules to test for SQL injection in applications.

### SSRF (Server-Side Request Forgery)
- Payloads to test for SSRF vulnerabilities in application endpoints.

### SSTI (Server-Side Template Injection)
- Inject template-specific payloads to test for SSTI vulnerabilities.

### WAF General Rules
- General rules to test web application firewalls for security configurations.

### WAF Bypass Payloads
- Rules and payloads to bypass web application firewalls.

### Web Cache Poisoning
- Test applications for vulnerabilities in caching mechanisms.

### XSS (Cross-Site Scripting)
- Inject payloads to test for reflected, stored, and DOM-based XSS.

### XXE (XML External Entity)
- Rules to test for XXE vulnerabilities in XML parsers.

---

## How to Use

1. Import the JSON files from this repository into Burp Suite under:
   - **Proxy > Options > Match and Replace**
2. Enable the rules relevant to your testing.
3. Send requests through Burp Suite Proxy to dynamically apply the rules.
4. Observe the results and identify potential vulnerabilities.

---

## Contributing

Contributions are welcome! If you have new rules or improvements to existing ones, feel free to submit a pull request. Please ensure that your rules are properly tested before submitting.

---

## License

This repository is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute the contents of this repository.
