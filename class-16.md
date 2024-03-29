# Anatomy of a Cloud Breach

On July 29, 2019, the FBI arrested Paige Thompson (also known by the alias “erratic” and a former AWS engineer) for allegedly hacking into Capital One databases and stealing the data located on AWS cloud servers. Capital One disclosed that the event affected approximately 100 million individuals in the United States and approximately 6 million in Canada. It also included data loss of approximately 1 million Social Insurance Numbers of Canadian credit card customers, about 140,000 Social Security numbers, and 80,000 linked bank account numbers of the credit card customers.

Erratic used TOR (The Onion network) to attempt connections, develop command scripts and other readiness activities. Multiple connections were made to connect to the servers, download pilot files to test out the end-to-end scenarios. Capital One’s customer information (700 folders worth of data) were posted on erratic’s public GitHub pages the IP address of a specific AWS server.

Code for 3 commands used for the attack:

Get Credentials - First command when executed obtained security
credentials known as -WAF-Role account (an IAM account) for an
elevated role access AWS Web Application Firewall (WAF)

List Buckets - Second command, when executed, used the security
credentials -WAF-Role account to list files and folders (aka S3 buckets)

Download Files - Third command, when executed used the -WAF-Role
account to download files that were accessible by the credentials
