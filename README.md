# WAF-Bypass-Payloads
List of payloads that can be generated for the open source WAF bypasser from @nemesida-waf. The following are deemed to be usable within the repo:
```
FP - False Positive payloads
API - API testing payloads
CM - Custom HTTP Method payloads
GraphQL - GraphQL testing payloads
LDAP - LDAP Injection etc. payloads
LFI - Local File Include payloads
MFD - multipart/form-data payloads
NoSQLi - NoSQL injection payloads
OR - Open Redirect payloads
RCE - Remote Code Execution payloads
RFI - Remote File Inclusion payloads
SQLi - SQL injection payloads
SSI - Server-Side Includes payloads
SSRF - Server-side request forgery payloads
SSTI - Server-Side Template Injection payloads
UWA - Unwanted Access payloads
XSS - Cross-Site Scripting payloads
```

# encode-me
This tool takes in input a payload and generates a list of encoded payloads based on 34 tampering functions.
The list of encoded payloads can be used to test the WAF.


# Usage

Generate about 40k encoded payload based on tampering functions
```
go run encode-me.go -p "<script> alert(1) </script>"  > list.txt
```
