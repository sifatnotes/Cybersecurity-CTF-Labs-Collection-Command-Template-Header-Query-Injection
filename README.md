# Cybersecurity-CTF-Labs-Collection-Command-Template-Header-Query-Injection
A curated, searchable index of hands-on CTF labs covering OS Command Injection, SSTI, Expression Language Injection, GraphQL Query Abuse, CRLF/Header Splitting, and CSV Formula Injection from Learn SecByte.
# Injection Vulnerabilities & Protocol Abuse CTF Labs Collection

A structured, searchable index of hands-on cybersecurity labs focusing on OS Command Injection, Server-Side Template Injection (SSTI), Expression Language (EL) Injection, GraphQL Query Abuse, CRLF/HTTP Header Splitting, Email/Log Injection, and CSV Formula Execution hosted on Learn SecByte.

This collection is designed for application security engineers, penetration testers, CTF competitors, security analysts, and backend developers seeking practical, hands-on training in input validation, query parsing, and injection defenses.

---

## Table of Contents
- [Introduction](#introduction)
- [Lab Collection & Index](#lab-collection--index)
- [Categories](#categories)
  - [Server-Side Code & Command Execution](#server-side-code--command-execution)
  - [Query Language & API Injections](#query-language--api-injections)
  - [Header, Protocol & Log Injections](#header-protocol--log-injections)
  - [Client Reflection & Data Export Injections](#client-reflection--data-export-injections)
- [Learning Path](#learning-path)
- [How to Use the Labs](#how-to-use-the-labs)
- [Disclaimer](#disclaimer)

---

## Introduction

Injection vulnerabilities remain among the most dangerous application security flaws, consistently enabling remote code execution, internal data exfiltration, and protocol manipulation. Whether an application unsafely interpolates user input into operating system commands, template engines, database/API queries, or HTTP headers, proper input sanitization and parameterized interfaces are critical.

This repository organizes hands-on cybersecurity labs from Learn SecByte into structured learning paths covering modern injection mechanisms and defensive engineering.

---

## Lab Collection & Index

| Lab Title | Primary Category | Vulnerability / Focus | Access Link |
| :--- | :--- | :--- | :--- |
| **Reflected XSS** | Client-Side Security | Input Reflection & Contexts | [Access Lab](https://learn.secbyte.org/ctf/reflected-xss-from-input-reflection-to-safe-exploitation-and) |
| **HTTP Header Injection** | Protocol Abuse | Response Splitting & Reflection | [Access Lab](https://learn.secbyte.org/ctf/http-header-injection-from-reflection-to-response-splitting) |
| **CRLF Injection** | Protocol Abuse | Header Splitting & Cache Poisoning | [Access Lab](https://learn.secbyte.org/ctf/crlf-injection-header-splitting-cache-poisoning) |
| **Log Injection** | Infrastructure Security | Log Forgery & Parsing Abuse | [Access Lab](https://learn.secbyte.org/ctf/log-injection-turning-logs-into-an-attack-surface) |
| **Email Header Injection** | Application Logic | Parsing Bugs & Mail Abuse | [Access Lab](https://learn.secbyte.org/ctf/email-header-injection-from-parsing-bugs-to-abuse-detection) |
| **CSV Formula Injection** | Client-Side Export | Spreadsheet Command Execution | [Access Lab](https://learn.secbyte.org/ctf/csv-formula-injection) |
| **Template Sandbox Escape** | Server-Side Execution | SSTI Sandbox Bypasses | [Access Lab](https://learn.secbyte.org/ctf/template-sandbox-escape) |
| **GraphQL Injection** | API Security | Query Abuse & Introspection Bypasses | [Access Lab](https://learn.secbyte.org/ctf/graphql-injection-query-abuse-introspection-bypass-technique) |
| **Expression Language Injection** | Server-Side Execution | OGNL / SpEL / EL RCE | [Access Lab](https://learn.secbyte.org/ctf/expression-language-injection-from-templating-to-exploitatio) |
| **Server-Side Template Injection** | Server-Side Execution | SSTI to System Code Execution | [Access Lab](https://learn.secbyte.org/ctf/server-side-template-injection) |
| **OS Command Injection** | Server-Side Execution | Operating System Command Execution | [Access Lab](https://learn.secbyte.org/ctf/os-command-injection-from-vulnerability-to-defense) |
| **XPath Injection** | Query Injection | Query Logic & Data Exfiltration | [Access Lab](https://learn.secbyte.org/ctf/xpath-injection-from-query-logic-to-data-exfiltration) |

---

## Categories

### Server-Side Code & Command Execution
Hands-on CTF labs detailing operating system command execution, template engine exploitation, and expression language sandbox escapes:

* **OS Command Injection:** Exploiting un-sanitized shell execution routines to execute arbitrary system commands.
  * Lab Link: https://learn.secbyte.org/ctf/os-command-injection-from-vulnerability-to-defense
* **Server-Side Template Injection (SSTI):** Identifying unsafe template engine interpolation (Jinja2, Twig, Freemarker) and achieving RCE.
  * Lab Link: https://learn.secbyte.org/ctf/server-side-template-injection
* **Template Sandbox Escape:** Breaking out of restrictive template engine execution sandboxes and restricted environments.
  * Lab Link: https://learn.secbyte.org/ctf/template-sandbox-escape
* **Expression Language (EL) Injection:** Abusing Spring SpEL, OGNL, or MVEL expressions to invoke reflection mechanisms and execute server-side commands.
  * Lab Link: https://learn.secbyte.org/ctf/expression-language-injection-from-templating-to-exploitatio

### Query Language & API Injections
Practical security labs focused on web API introspection, structured document query manipulations, and data extraction:

* **GraphQL Query Abuse & Introspection Bypass:** Subverting GraphQL authorization boundaries, abusing introspection queries, and executing batching attacks.
  * Lab Link: https://learn.secbyte.org/ctf/graphql-injection-query-abuse-introspection-bypass-technique
* **XPath Query Injection:** Manipulating XML path query logic to bypass authentication logic and extract structured data.
  * Lab Link: https://learn.secbyte.org/ctf/xpath-injection-from-query-logic-to-data-exfiltration

### Header, Protocol & Log Injections
Security labs covering character encoding manipulation (`\r\n`), HTTP response splitting, header injection, and log parsing vulnerabilities:

* **HTTP Header Injection:** Injecting arbitrary response headers via untrusted input reflection.
  * Lab Link: https://learn.secbyte.org/ctf/http-header-injection-from-reflection-to-response-splitting
* **CRLF Injection:** Exploiting Carriage Return Line Feed (`\r\n`) characters to execute HTTP response splitting and web cache poisoning.
  * Lab Link: https://learn.secbyte.org/ctf/crlf-injection-header-splitting-cache-poisoning
* **Log Injection:** Injecting malicious newline sequences and false entries into application access and audit logs.
  * Lab Link: https://learn.secbyte.org/ctf/log-injection-turning-logs-into-an-attack-surface
* **Email Header Injection:** Manipulating mail form headers (`Cc`, `Bcc`, `Subject`) through un-sanitized newline characters in contact forms.
  * Lab Link: https://learn.secbyte.org/ctf/email-header-injection-from-parsing-bugs-to-abuse-detection

### Client Reflection & Data Export Injections
Labs detailing client-side input reflection and dangerous payload execution within client applications:

* **Reflected XSS:** Identifying non-persistent input reflection and executing arbitrary client-side script contexts.
  * Lab Link: https://learn.secbyte.org/ctf/reflected-xss-from-input-reflection-to-safe-exploitation-and
* **CSV Formula Injection:** Injecting dynamic spreadsheet formulas (`=CMD()`, `@SUM()`) into downloadable CSV/XLS exports to compromise client end-user devices.
  * Lab Link: https://learn.secbyte.org/ctf/csv-formula-injection

---

## Learning Path

Follow this structured roadmap to master injection vulnerability testing and code remediation:

1. **Header & Protocol Injection Basics**
   - Practice CRLF injection, HTTP response splitting, and email/log header injection.
   - Evaluate client-side CSV formula exports for dynamic formula execution risks.
2. **Reflected Input & Query Injection**
   - Analyze reflected input contexts for XSS and manipulate XPath queries.
   - Test GraphQL endpoints for introspection exposure, query depth limit missing, and injection flaws.
3. **Template Engine & Expression Language Analysis**
   - Identify template engine syntax and construct SSTI payloads.
   - Practice sandbox escapes and Expression Language (SpEL/OGNL) injections.
4. **OS Command Injection & Full System Remediation**
   - Execute command injection bypasses against shell character filters.
   - Implement parameterized APIs, safe templating engines, strict allowlists, and non-shell command execution APIs.

---

## How to Use the Labs

1. Select a practice scenario from the index table or category breakdown above.
2. Access the target lab environment directly on Learn SecByte.
3. Utilize web proxies (e.g., Burp Suite) to inject newline characters, alter API queries, manipulate template strings, and craft shell command delimiters.
4. Review defensive controls to learn how context-aware encoding, parameterized queries, strict input sanitization, and non-shell system calls protect applications.

---

## Disclaimer

This repository is strictly intended for educational research, authorized security testing, and defensive engineering training. All concepts, techniques, and lab environments are provided to help cybersecurity practitioners identify vulnerabilities and harden systems against injection attacks. Unsanctioned testing or attacks against external systems without prior written authorization are strictly illegal.
