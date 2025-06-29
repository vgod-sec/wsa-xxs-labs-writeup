
This lab showcases a **DOM-based Cross-Site Scripting (XSS)** vulnerability in a search functionality where untrusted input from `location.search` is processed by client-side JavaScript and inserted into the page using the insecure `document.write()` method. The vulnerable code writes user-controlled data directly into an `img src` attribute without any encoding or validation, making it possible for an attacker to break out of the HTML context and inject malicious scripts.

To exploit this, begin by entering any random search term, such as `test`, into the search box. Upon submission, inspect the resulting page and observe that the input is reflected within the `src` attribute of an `img` element. This confirms that the application is inserting raw input from the URL query string into the DOM via `document.write()`.

Next, craft a payload that exits the `img` tag’s `src` attribute context and injects a new HTML element containing JavaScript. Use the following payload in the URL: ?search=">
This breaks the context of the `img` tag and introduces a new `<svg>` element. When the browser renders the page, the `onload` event of the `<svg>` tag is triggered, executing `alert(1)` and confirming a successful XSS attack.

**Impact:**  
DOM-based XSS is particularly dangerous because it executes entirely on the client side, bypassing server-side defenses. Successful exploitation can lead to:
- Session hijacking
- Credential theft
- DOM manipulation
- Unwanted redirections
- Execution of arbitrary JavaScript in the context of the vulnerable site

**Mitigation:**  
To prevent DOM-based XSS:
- Avoid using `document.write()`—prefer safer DOM APIs like `textContent`, `setAttribute`, or `createElement`.
- Sanitize and validate all user inputs, especially data sourced from `location.search`, `location.hash`, or `location.pathname`.
- Implement a strict **Content Security Policy (CSP)** to mitigate the impact of potential script injections.
- Utilize frameworks like React or Angular that enforce output encoding and reduce exposure to direct DOM manipulation.

**Key Takeaways:**  
This lab highlights how improper handling of client-side data using unsafe sinks such as `document.write()` can lead to DOM XSS vulnerabilities. Secure coding practices, context-aware encoding, and the use of modern frameworks and security headers are essential to protect against such client-side attacks.
