# What is Burp Suite?

Burp Suite is a suite of tools from PortSwigger designed to aid in the penetration testing of web applications over both HTTP and HTTPS. The primary tool is a proxy designed to allow the analysis and editing of web traffic and can intercept web requests and responses and read and edit them in real-time before they reach their respective destinations. The proxy itself allows you to configure which domains have their web traffic intercepted and what sort of traffic is shown.

Integrated tools in Burp Suite:

- Intruder can import a request and then configure arrange of payloads to attempt and can then run through them automatically.

- Repeater can import a web request and then make manual modifications to it and see the response side by side allowing you to make minor adjustments to attempted exploits and easily see if it’s working.

- Sequencer is designed to analyse the randomness of data such as session IDs, CSRF tokens, and password reset tokens.

- Decoder can decode strings from a range of encoding standards as well as allowing you to encode data again.

- Comparer can compare two strings to check for minor differences.
