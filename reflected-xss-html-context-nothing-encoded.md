
Lab Title: Reflected XSS into HTML context with nothing encoded  
Level: Apprentice  
Tags: XSS, Reflected, HTML Context, No Encoding  
Description: This lab contains a reflected cross-site scripting vulnerability where user input is embedded into an HTML page without any encoding or sanitization, allowing an attacker to inject malicious scripts.  
Extended Description: Reflected XSS in HTML context with no encoding allows direct script injection and execution.  
Objective: Inject a payload that triggers alert(1) by exploiting the reflected XSS vulnerability.  
Steps:  
1. Click "ACCESS THE LAB" to open the lab.  
2. In the search input, enter the payload: <script>alert(1)</script>  
3. Click the "Search" button.  
4. The alert(1) popup will appear.  
5. Lab is marked as solved.  
Payload Used: <script>alert(1)</script>  
Mitigation and Key Takeaways: Reflected XSS occurs when input is included in the HTML output without encoding. Always perform output encoding based on context (HTML, attribute, JavaScript). Escape special characters like < > " ' &. Use security frameworks like React or Angular that automatically escape content. Implement Content Security Policy (CSP) to prevent inline script execution. Never trust user input. Validate and sanitize all data both on client and server sides.  
References:  
- https://portswigger.net/web-security/cross-site-scripting/reflected  
- https://cheatsheetseries.owasp.org/cheatsheets/XSS_Prevention_Cheat_Sheet.html
