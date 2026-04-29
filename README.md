# FUTURE_CS_01
A vulnerability assessment report of a live website conducted using ethical, read-only security analysis. This project identifies potential security risks, classifies their impact, and provides practical remediation steps in a business friendly format. This was conducted on a deliberately vulnerable application

## SCOPE & METHODOLODGY 
The assesment was performaed on the following target:

-Target: http://demo.testfire.net

## TOOLS USED
-Nmap: this was used for network scanning and port analysis.  
-OWASP ZAP: this was used for web application vulnerability scanning. 

### Method:
1. Network scanning using Nmap to identify open ports and services.
2. Web applications scanning using OWASP ZAP (spider and active scan)
3. Analysis and classificatoin of vulnerablities
4. Recommendation of remediation steps.

## IDENTIFIED VULNERABILITILES

### HIGH Risk
- SQL Injection
- Cross-Site Scripting (XSS)
### Medium Risk
- Absence of Anti-CSRF Tokens
- Cookies without Samesite Attributes
### Low Risk
- Missing security Headers  (CSP,X-Frame-Options, X-Content-Type-Options).
- Information Disclosure (Server Version Exposure).

  ## RISK CLASSIFICATION:
| Risk Level | Description  |
|------------|--------------|
| High       | Critical vulnerabilties that can lead to data breaches|
| Medium     | Vulnerabilities that may be exploited under certain conditions |
| Low        | Minor issues that weaken security posture |

## REMEDIATION STEPS
- Make use of parameterized queries to prevent SQL injection
- Sanitize and validate all user input to prevent XSS
- Implement Anti-CSRF tokens for sensitve actions
- Configure cookies with secure and samesite attributes
- Add security headers such as CSP, HSTS and X-Frame-Options
- Hide server version information

  ## TOOLS & TECHNOLOGIES
  - Nmap
  - OWASP ZAP
  - Windows Command Prompt
    
 ## EVIDENCE 
 Screenshots of scans and findings are included in the respository:
 
 -Nmap scan results 
 
 -OWASP ZAP alerts and vulnerabilty details. 

 ## CONCLUSION
 The assessment identified serveral critiacal and moderate vulnerabilties that could compromise the security of the application. Immediate remediation is recommended, particularly for high-risk vulnerabilties such as SQL injection and Coss-Scripting. The project demonstrates the importance of regular security testing and secure coding practices in modern web applications. 
  
