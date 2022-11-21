# Cross-site scripting

Cross-site scripting (also known as XSS) is a web security vulnerability that allows an attacker to compromise the interactions that users have with a vulnerable application. XSS lets an attacker circumvent the same origin policy, which is designed to segregate different websites from each other. XSS works by manipulating a vulnerable web site so that it returns malicious JavaScript to users, which the attacker can use to fully compromise their interaction with the application.

You can confirm most kinds of XSS vulnerability by injecting a payload that causes your own browser to execute some arbitrary JavaScript. The vast majority of XSS vulnerabilities can be found quickly and reliably using Burp Suite's web vulnerability scanner.

Three main types of XSS attacks:

- Reflected XSS: where the malicious script comes from the current HTTP request.

- Stored XSS: where the malicious script comes from the website's database.

- DOM-based XSS: where the vulnerability exists in client-side code rather than server-side code.

How to prevent XSS attacks:

- Filter input on arrival.

- Encode data on output.

- Use appropriate response headers.

- Content Security Policy.
