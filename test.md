ZAP Scanning Report
Generated with ZAP on Fri 10 Dec 2021, at 22:02:

Contents
About this report
Report parameters
Summaries
Alert counts by risk and confidence
Alert counts by site and risk
Alert counts by alert type
Alerts
Risk=Medium, Confidence=Medium (6)
Risk=Low, Confidence=High (2)
Risk=Low, Confidence=Medium (13)
Risk=Informational, Confidence=High (3)
Risk=Informational, Confidence=Medium (1)
Appendix
Alert types
About this report
Report parameters

Contexts
The following contexts were selected to be included:
asp.net
Sites
The following sites were included:
https://ehikebe.azurewebsites.net
(If no sites were selected, all sites were included by default.)
An included site must also be within one of the included contexts for its
data to be included in the report.
Risk levels
Included: High, Medium, Low, Informational
Excluded: None
Confidence levels
Included: User Confirmed, High, Medium, Low
Excluded: User Confirmed, High, Medium, Low, False Positive
Summaries
Alert counts by risk and confidence

This table shows the number of alerts for each level of risk and confidence
included in the report.

(The percentages in brackets represent the count as a percentage of the total
number of alerts included in the report, rounded to one decimal place.)

Confidence
User
Confirmed High Medium Low Total
Risk
High 0
(0.0%)
0
(0.0%)
0
(0.0%)
0
(0.0%)
0
(0.0%)
Medium 0
(0.0%)
0
(0.0%)
6
(24.0%)
0
(0.0%)
6
(24.0%)
Low 0
(0.0%)
2
(8.0%)
13
(52.0%)
0
(0.0%)
15
(60.0%)
Information
al
0
(0.0%)
3
(12.0%)
1
(4.0%)
0
(0.0%)
4
(16.0%)
Total 0
(0.0%)
5
(20.0%)
20
(80.0%)
0
(0.0%)
25
(100%)
Alert counts by site and risk

This table shows, for each site for which one or more alerts were raised, the
number of alerts raised at each risk level.

Alerts with a confidence level of "False Positive" have been excluded from
these counts.

(The numbers in brackets are the number of alerts raised for the site at or
above that risk level.)

Risk
High
(= High)
Medium
(>= Medi‐
um)
Low
(>= Low)
Informatio
nal
(>= Infor‐
mational)
Risk
High
(= High)
Medium
(>= Medi‐
um)
Low
(>= Low)
Informatio
nal
(>= Infor‐
mational)
Site
https://ehikebe.az
urewebsites.net
0
(0)
6
(6)
15
(21)
4
(25)
Alert counts by alert type

This table shows the number of alerts of each alert type, together with the
alert type's risk level.

(The percentages in brackets represent each count as a percentage, rounded
to one decimal place, of the total number of alerts included in this report.)

Alert type Risk Count
CSP: Wildcard Directive Medium 2
(8.0%)
CSP: script-src unsafe-inline Medium 2
(8.0%)
CSP: style-src unsafe-inline Medium 2
(8.0%)
Absence of Anti-CSRF Tokens Low 1
(4.0%)
Cookie with SameSite Attribute None Low 2
(8.0%)
Cookie without SameSite Attribute Low 2
(8.0%)
Total 25
Alert type Risk Count
Cross-Domain JavaScript Source File
Inclusion
Low 1
(4.0%)
Incomplete or No Cache-control Header
Set
Low 1
(4.0%)
Server Leaks Information via "X-Powered-
By" HTTP Response Header Field(s)
Low 2
(8.0%)
Server Leaks Information via 'X-Powered-
By' HTTP Response Header Field(s)(script)
Low 2
(8.0%)
Server Leaks Version Information via
'Server' HTTP Response Header
Field(script)
Low 2
(8.0%)
Unexpected Content-Type was returned Low 2
(8.0%)
Email addresses (script) Informational 1
(4.0%)
Information Exposure Through HTML
Comments (script)
Informational 1
(4.0%)
SameSite cookie attribute protection used Informational 2
(8.0%)
Total 25
Alerts
Risk=Medium, Confidence=Medium (6)

https://ehikebe.azurewebsites.net (6)
CSP: Wildcard Directive (2)

GET https://ehikebe.azurewebsites.net:
Alert tags OWASP_2021_A
OWASP_2017_A
Alert
description
The following directives either allow
wildcard sources (or ancestors), are not
defined, or are overly broadly defined:
img-src, connects-src, frame-src, frame-
ancestors, media-src, object-src,
manifest-src, prefetch-src, form-action
The directive(s): frame-ancestors, form-
action are among the directives that do
not fallback to default-src,
missing/excluding them is the same as
allowing anything.
Request Request line and header section (
bytes)
GET
https://ehikebe.azurewebsites.net:
443 HTTP/1.
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.
Pragma: no-cache
Cache-Control: no-cache
Authorization: Bearer null
Request body (0 bytes)
Response Status line and header section (
bytes)
HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-
Server: Microsoft-IIS/10.
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb
7119e709978d2cf1da299e8341753d6f
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 20:06:
GMT

Response body (10759 bytes)
Evidence default-src 'self'^
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
Solution Ensure that your web server, application
server, load balancer, etc. is properly
configured to set the Content-Security-
Policy header.
HEAD https://ehikebe.azurewebsites.net:

Alert tags OWASP_2021_A
OWASP_2017_A
Alert
description
The following directives either allow
wildcard sources (or ancestors), are not
defined, or are overly broadly defined:
img-src, connects-src, frame-src, frame-
ancestors, media-src, object-src,
manifest-src, prefetch-src, form-action
The directive(s): frame-ancestors, form-
action are among the directives that do
not fallback to default-src,
missing/excluding them is the same as
allowing anything.
Request Request line and header section (
bytes)
HEAD
https://ehikebe.azurewebsites.net:
443 HTTP/1.
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.
Pragma: no-cache
Cache-Control: no-cache
Content-Length: 0
Request body (0 bytes)
Response Status line and header section (
bytes)

HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-
Server: Microsoft-IIS/10.
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb
7119e709978d2cf1da299e8341753d6f
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 18:08:
GMT
Response body (0 bytes)
Evidence default-src 'self'^
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
Solution Ensure that your web server, application
server, load balancer, etc. is properly
configured to set the Content-Security-
Policy header.
CSP: script-src unsafe-inline (2)

GET https://ehikebe.azurewebsites.net:
Alert tags OWASP_2021_A
OWASP_2017_A

Alert
description

script-src includes unsafe-inline.
Request Request line and header section (
bytes)

GET
https://ehikebe.azurewebsites.net:
443 HTTP/1.
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.
Pragma: no-cache
Cache-Control: no-cache
Authorization: Bearer null
Request body (0 bytes)
Response Status line and header section (
bytes)

HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-
Server: Microsoft-IIS/10.
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb
7119e709978d2cf1da299e8341753d6f
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 20:06:
GMT
Response body (10759 bytes)
Evidence default-src 'self'^
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content

Solution Ensure that your web server, application
server, load balancer, etc. is properly
configured to set the Content-Security-
Policy header.
HEAD https://ehikebe.azurewebsites.net:

Alert tags OWASP_2021_A
OWASP_2017_A
Alert
description
script-src includes unsafe-inline.
Request Request line and header section (
bytes)
HEAD
https://ehikebe.azurewebsites.net:
443 HTTP/1.
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.
Pragma: no-cache
Cache-Control: no-cache
Content-Length: 0
Request body (0 bytes)
Response Status line and header section (
bytes)
HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-
Server: Microsoft-IIS/10.
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb
7119e709978d2cf1da299e8341753d6f
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 18:08:
GMT
Response body (0 bytes)
Evidence default-src 'self'^
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'

https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
Solution Ensure that your web server, application
server, load balancer, etc. is properly
configured to set the Content-Security-
Policy header.
CSP: style-src unsafe-inline (2)

GET https://ehikebe.azurewebsites.net:
Alert tags OWASP_2021_A
OWASP_2017_A
Alert
description
style-src includes unsafe-inline.
Request Request line and header section (
bytes)
GET
https://ehikebe.azurewebsites.net:
443 HTTP/1.
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.
Pragma: no-cache
Cache-Control: no-cache
Authorization: Bearer null
Request body (0 bytes)
Response Status line and header section (
bytes)

HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-
Server: Microsoft-IIS/10.
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb
7119e709978d2cf1da299e8341753d6f
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 20:06:

GMT
Response body (10759 bytes)
Evidence default-src 'self'^
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
Solution Ensure that your web server, application
server, load balancer, etc. is properly
configured to set the Content-Security-
Policy header.
HEAD https://ehikebe.azurewebsites.net:

Alert tags OWASP_2021_A
OWASP_2017_A
Alert
description
style-src includes unsafe-inline.
Request Request line and header section (
bytes)
HEAD
https://ehikebe.azurewebsites.net:
443 HTTP/1.
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.
Pragma: no-cache
Cache-Control: no-cache
Content-Length: 0
Request body (0 bytes)
Response Status line and header section (
bytes)

HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-
Server: Microsoft-IIS/10.
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb
7119e709978d2cf1da299e8341753d6f
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 18:08:
GMT
Response body (0 bytes)
Evidence default-src 'self'^
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
Solution Ensure that your web server, application
server, load balancer, etc. is properly
configured to set the Content-Security-
Policy header.
Risk=Low, Confidence=High (2)

https://ehikebe.azurewebsites.net (2)
Unexpected Content-Type was returned (2)
GET https://ehikebe.azurewebsites.net:
Alert A Content-Type of text/html was
description returned by the server.

This is not one of the types expected to
be returned by an API.
Raised by the 'Alert on Unexpected
Content Types' script
Request Request line and header section (
bytes)

GET
https://ehikebe.azurewebsites.net:
443 HTTP/1.
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.
Pragma: no-cache
Cache-Control: no-cache
Authorization: Bearer null
Request body (0 bytes)
Response Status line and header section (
bytes)

HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-
Server: Microsoft-IIS/10.
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e709
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb5
7119e709978d2cf1da299e8341753d6f63
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 20:06:29
GMT
Response body (10759 bytes)
Evidence text/html
HEAD https://ehikebe.azurewebsites.net:443

Alert
description
A Content-Type of text/html was
returned by the server.
This is not one of the types expected to
be returned by an API.
Raised by the 'Alert on Unexpected
Content Types' script
Request Request line and header section (242
bytes)

HEAD
https://ehikebe.azurewebsites.net:
443 HTTP/1.1
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.0
Pragma: no-cache
Cache-Control: no-cache
Content-Length: 0
Request body (0 bytes)
Response Status line and header section (1142
bytes)

HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-8
Server: Microsoft-IIS/10.0
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e709
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb5
7119e709978d2cf1da299e8341753d6f63
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 18:08:33
GMT
Response body (0 bytes)
Evidence text/html
Risk=Low, Confidence=Medium (13)

https://ehikebe.azurewebsites.net (13)
Absence of Anti-CSRF Tokens (1)
GET https://ehikebe.azurewebsites.net:443
Alert tags OWASP_2021_A01
WSTG-v42-SESS-05
OWASP_2017_A05
Alert
description

No Anti-CSRF tokens were found in a
HTML submission form.
A cross-site request forgery is an attack
that involves forcing a victim to send an
HTTP request to a target destination
without their knowledge or intent in
order to perform an action as the victim.
The underlying cause is application
functionality using predictable URL/form
actions in a repeatable way. The nature
of the attack is that CSRF exploits the
trust that a web site has for a user. By
contrast, cross-site scripting (XSS)
exploits the trust that a user has for a
web site. Like XSS, CSRF attacks are not
necessarily cross-site, but they can be.
Cross-site request forgery is also known
as CSRF, XSRF, one-click attack, session
riding, confused deputy, and sea surf.
CSRF attacks are effective in a number
of situations, including:
* The victim has an active session on
the target site.
* The victim is authenticated via HTTP
auth on the target site.
* The victim is on the same local
network as the target site.
CSRF has primarily been used to
perform an action against a target site
using the victim's privileges, but recent
techniques have been discovered to
disclose information by gaining access to
the response. The risk of information
disclosure is dramatically increased
when the target site is vulnerable to
XSS, because XSS can be used as a
platform for CSRF, allowing the attack to
operate within the bounds of the same-
origin policy.
Other info No known Anti-CSRF token [anticsrf,
CSRFToken, __RequestVerificationToken,
csrfmiddlewaretoken,
authenticity_token,
OWASP_CSRFTOKEN, anoncsrf,
csrf_token, _csrf, _csrfSecret,
__csrf_magic, CSRF, _token,
_csrf_token] was found in the following
HTML form: [Form 1: "email" "name"
"phone" ].

Request Request line and header section (250
bytes)

GET
https://ehikebe.azurewebsites.net:
443 HTTP/1.1
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.0
Pragma: no-cache
Cache-Control: no-cache
Authorization: Bearer null
Request body (0 bytes)
Response Status line and header section (1142
bytes)

HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-8
Server: Microsoft-IIS/10.0
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e709
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb5
7119e709978d2cf1da299e8341753d6f63
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 20:06:29
GMT
Response body (10759 bytes)
Evidence

Solution Phase: Architecture and Design

Use a vetted library or framework that
does not allow this weakness to occur or
provides constructs that make this
weakness easier to avoid.
For example, use anti-CSRF packages
such as the OWASP CSRFGuard.
Phase: Implementation
Ensure that your application is free of
cross-site scripting issues, because most
CSRF defenses can be bypassed using
attacker-controlled script.
Phase: Architecture and Design
Generate a unique nonce for each form,
place the nonce into the form, and verify
the nonce upon receipt of the form. Be
sure that the nonce is not predictable
(CWE-330).
Note that this can be bypassed using
XSS.
Identify especially dangerous
operations. When the user performs a
dangerous operation, send a separate
confirmation request to ensure that the
user intended to perform that operation.
Note that this can be bypassed using
XSS.
Use the ESAPI Session Management
control.
This control includes a component for
CSRF.
Do not use the GET method for any
request that triggers a state change.
Phase: Implementation
Check the HTTP Referer header to see if
the request originated from an expected
page. This could break legitimate
functionality, because users or proxies
may have disabled sending the Referer
for privacy reasons.
Cookie with SameSite Attribute None (2)

GET https://ehikebe.azurewebsites.net:443
Alert tags OWASP_2021_A01
WSTG-v42-SESS-02
OWASP_2017_A05
Alert
description
A cookie has been set with its SameSite
attribute set to "none", which means
that the cookie can be sent as a result
of a 'cross-site' request. The SameSite
attribute is an effective counter measure
to cross-site request forgery, cross-site
script inclusion, and timing attacks.
Request Request line and header section (250
bytes)
GET
https://ehikebe.azurewebsites.net:
443 HTTP/1.1
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.0
Pragma: no-cache
Cache-Control: no-cache
Authorization: Bearer null
Request body (0 bytes)
Response Status line and header section (1142
bytes)

HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-8
Server: Microsoft-IIS/10.0
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e709
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb5
7119e709978d2cf1da299e8341753d6f63
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 20:06:29
GMT
Response body (10759 bytes)
Solution Ensure that the SameSite attribute is set
to either 'lax' or ideally 'strict' for all
cookies.
HEAD https://ehikebe.azurewebsites.net:443

Alert tags OWASP_2021_A01
WSTG-v42-SESS-02
OWASP_2017_A05
Alert
description
A cookie has been set with its SameSite
attribute set to "none", which means
that the cookie can be sent as a result
of a 'cross-site' request. The SameSite
attribute is an effective counter measure
to cross-site request forgery, cross-site
script inclusion, and timing attacks.
Request Request line and header section (242
bytes)
HEAD
https://ehikebe.azurewebsites.net:
443 HTTP/1.1
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.0
Pragma: no-cache
Cache-Control: no-cache
Content-Length: 0
Request body (0 bytes)
Response Status line and header section (1142
bytes)

HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-8
Server: Microsoft-IIS/10.0
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e709
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb5
7119e709978d2cf1da299e8341753d6f63
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 18:08:33
GMT
Response body (0 bytes)
Solution Ensure that the SameSite attribute is set
to either 'lax' or ideally 'strict' for all
cookies.
Cookie without SameSite Attribute (2)

GET https://ehikebe.azurewebsites.net:443
Alert tags OWASP_2021_A01
WSTG-v42-SESS-02
OWASP_2017_A05
Alert
description
A cookie has been set without the
SameSite attribute, which means that
the cookie can be sent as a result of a
'cross-site' request. The SameSite
attribute is an effective counter measure
to cross-site request forgery, cross-site
script inclusion, and timing attacks.
Request Request line and header section (250
bytes)
GET
https://ehikebe.azurewebsites.net:
443 HTTP/1.1
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.0
Pragma: no-cache
Cache-Control: no-cache
Authorization: Bearer null
Request body (0 bytes)
Response Status line and header section (1142
bytes)

HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-8
Server: Microsoft-IIS/10.0
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e709
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb5
7119e709978d2cf1da299e8341753d6f63
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 20:06:29
GMT
Response body (10759 bytes)
Parameter ARRAffinity
Evidence Set-Cookie: ARRAffinity
Solution Ensure that the SameSite attribute is set
to either 'lax' or ideally 'strict' for all
cookies.
HEAD https://ehikebe.azurewebsites.net:443

Alert tags OWASP_2021_A01
WSTG-v42-SESS-02
OWASP_2017_A05
Alert
description
A cookie has been set without the
SameSite attribute, which means that
the cookie can be sent as a result of a
'cross-site' request. The SameSite
attribute is an effective counter measure
to cross-site request forgery, cross-site
script inclusion, and timing attacks.
Request Request line and header section (242
bytes)
HEAD
https://ehikebe.azurewebsites.net:
443 HTTP/1.1
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.0
Pragma: no-cache
Cache-Control: no-cache
Content-Length: 0
Request body (0 bytes)
Response Status line and header section (1142
bytes)

HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-8
Server: Microsoft-IIS/10.0
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e709
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb5
7119e709978d2cf1da299e8341753d6f63
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 18:08:33
GMT
Response body (0 bytes)
Parameter ARRAffinity
Evidence Set-Cookie: ARRAffinity
Solution Ensure that the SameSite attribute is set
to either 'lax' or ideally 'strict' for all
cookies.
Cross-Domain JavaScript Source File Inclusion (1)

GET https://ehikebe.azurewebsites.net:443
Alert tags OWASP_2021_A08
Alert
description
The page includes one or more script
files from a third-party domain.
Request Request line and header section (250
bytes)
GET
https://ehikebe.azurewebsites.net:
443 HTTP/1.1
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.0
Pragma: no-cache
Cache-Control: no-cache
Authorization: Bearer null
Request body (0 bytes)
Response Status line and header section (1142
bytes)

HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-8
Server: Microsoft-IIS/10.0
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e709
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb5
7119e709978d2cf1da299e8341753d6f63
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 20:06:29
GMT
Response body (10759 bytes)
Parameter https://cdn.jsdelivr.net/npm/boots
trap@5.1.3/dist/js/bootstrap.bundl
e.min.js
Evidence <script^
src="https://cdn.jsdelivr.net/npm/
bootstrap@5.1.3/dist/js/bootstrap.
bundle.min.js"></script>
Solution Ensure JavaScript source files are loaded
from only trusted sources, and the
sources can't be controlled by end users
of the application.
Incomplete or No Cache-control Header Set (1)

GET https://ehikebe.azurewebsites.net:443
Alert tags WSTG-v42-ATHN-06
Alert
description
The cache-control header has not been
set properly or is missing, allowing the
browser and proxies to cache content.
Request Request line and header section (250
bytes)

GET
https://ehikebe.azurewebsites.net:
443 HTTP/1.1
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.0
Pragma: no-cache
Cache-Control: no-cache
Authorization: Bearer null
Request body (0 bytes)
Response Status line and header section (1142
bytes)

HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-8
Server: Microsoft-IIS/10.0
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e709
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb5
7119e709978d2cf1da299e8341753d6f63
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 20:06:29
GMT
Response body (10759 bytes)
Parameter Cache-Control
Solution Whenever possible ensure the cache-
control HTTP header is set with no-
cache, no-store, must-revalidate.
Server Leaks Information via "X-Powered-By" HTTP
Response Header Field(s) (2)

GET https://ehikebe.azurewebsites.net:443
Alert tags OWASP_2021_A01
WSTG-v42-INFO-08
OWASP_2017_A03
Alert
description
The web/application server is leaking
information via one or more "X-
Powered-By" HTTP response headers.
Access to such information may facilitate
attackers identifying other
frameworks/components your web
application is reliant upon and the
vulnerabilities such components may be
subject to.
Request Request line and header section (250
bytes)

GET
https://ehikebe.azurewebsites.net:
443 HTTP/1.1
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.0
Pragma: no-cache
Cache-Control: no-cache
Authorization: Bearer null
Request body (0 bytes)
Response Status line and header section (1142
bytes)

HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-8
Server: Microsoft-IIS/10.0
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e709
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb5
7119e709978d2cf1da299e8341753d6f63
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 20:06:29
GMT
Response body (10759 bytes)
Evidence X-Powered-By: ASP.NET
Solution Ensure that your web server, application
server, load balancer, etc. is configured
to suppress "X-Powered-By" headers.
HEAD https://ehikebe.azurewebsites.net:443

Alert tags OWASP_2021_A01
WSTG-v42-INFO-08
OWASP_2017_A03
Alert
description

The web/application server is leaking
information via one or more "X-
Powered-By" HTTP response headers.
Access to such information may facilitate
attackers identifying other
frameworks/components your web
application is reliant upon and the
vulnerabilities such components may be
subject to.
Request Request line and header section (242
bytes)

HEAD
https://ehikebe.azurewebsites.net:
443 HTTP/1.1
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.0
Pragma: no-cache
Cache-Control: no-cache
Content-Length: 0
Request body (0 bytes)
Response Status line and header section (1142
bytes)

HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-8
Server: Microsoft-IIS/10.0
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e709
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb5
7119e709978d2cf1da299e8341753d6f63
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 18:08:33
GMT
Response body (0 bytes)
Evidence X-Powered-By: ASP.NET

Solution Ensure that your web server, application
server, load balancer, etc. is configured
to suppress "X-Powered-By" headers.

Server Leaks Information via 'X-Powered-By' HTTP Response
Header Field(s)(script) (2)

GET https://ehikebe.azurewebsites.net:443
Alert
description
The web/application server is leaking
information via one or more 'X-Powered-
By' HTTP response headers. Access to
such information may facilitate attackers
identifying other
frameworks/components your web
application is reliant upon and the
vulnerabilities such components may be
subject to.
Request Request line and header section (250
bytes)
GET
https://ehikebe.azurewebsites.net:
443 HTTP/1.1
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.0
Pragma: no-cache
Cache-Control: no-cache
Authorization: Bearer null
Request body (0 bytes)
Response Status line and header section (1142
bytes)
HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-8
Server: Microsoft-IIS/10.0
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e709
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb5
7119e709978d2cf1da299e8341753d6f63
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 20:06:29
GMT
Response body (10759 bytes)
Evidence [ASP.NET]

Solution Ensure that your web server, application
server, load balancer, etc. is configured
to suppress 'X-Powered-By' headers.
HEAD https://ehikebe.azurewebsites.net:443

Alert
description
The web/application server is leaking
information via one or more 'X-Powered-
By' HTTP response headers. Access to
such information may facilitate attackers
identifying other
frameworks/components your web
application is reliant upon and the
vulnerabilities such components may be
subject to.
Request Request line and header section (242
bytes)
HEAD
https://ehikebe.azurewebsites.net:
443 HTTP/1.1
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.0
Pragma: no-cache
Cache-Control: no-cache
Content-Length: 0
Request body (0 bytes)
Response Status line and header section (1142
bytes)
HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-8
Server: Microsoft-IIS/10.0
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e709
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb5
7119e709978d2cf1da299e8341753d6f63
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 18:08:33
GMT
Response body (0 bytes)
Evidence [ASP.NET]

Solution Ensure that your web server, application
server, load balancer, etc. is configured
to suppress 'X-Powered-By' headers.
Server Leaks Version Information via 'Server' HTTP Response
Header Field(script) (2)

GET https://ehikebe.azurewebsites.net:443
Alert
description
The web/application server is leaking
version information via the 'Server'
HTTP response header. Access to such
information may facilitate attackers
identifying other vulnerabilities your
web/application server is subject to.
Request Request line and header section (250
bytes)
GET
https://ehikebe.azurewebsites.net:
443 HTTP/1.1
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.0
Pragma: no-cache
Cache-Control: no-cache
Authorization: Bearer null
Request body (0 bytes)
Response Status line and header section (1142
bytes)
HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-8
Server: Microsoft-IIS/10.0
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e709
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb5
7119e709978d2cf1da299e8341753d6f63
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 20:06:29
GMT
Response body (10759 bytes)
Evidence [Microsoft-IIS/10.0]

Solution Ensure that your web server, application
server, load balancer, etc. is configured
to suppress the 'Server' header or
provide generic details.
HEAD https://ehikebe.azurewebsites.net:443

Alert
description
The web/application server is leaking
version information via the 'Server'
HTTP response header. Access to such
information may facilitate attackers
identifying other vulnerabilities your
web/application server is subject to.
Request Request line and header section (242
bytes)
HEAD
https://ehikebe.azurewebsites.net:
443 HTTP/1.1
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.0
Pragma: no-cache
Cache-Control: no-cache
Content-Length: 0
Request body (0 bytes)
Response Status line and header section (1142
bytes)
HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-8
Server: Microsoft-IIS/10.0
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e709
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb5
7119e709978d2cf1da299e8341753d6f63
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 18:08:33
GMT
Response body (0 bytes)
Evidence [Microsoft-IIS/10.0]

Solution Ensure that your web server, application

server, load balancer, etc. is configured
to suppress the 'Server' header or
provide generic details.
Risk=Informational, Confidence=High (3)

https://ehikebe.azurewebsites.net (3)
Email addresses (script) (1)
GET https://ehikebe.azurewebsites.net:443
Alert
description
Email addresses were found
Other info name@example.com
Request Request line and header section (250
bytes)
GET
https://ehikebe.azurewebsites.net:
443 HTTP/1.1
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.0
Pragma: no-cache
Cache-Control: no-cache
Authorization: Bearer null
Request body (0 bytes)
Response Status line and header section (1142
bytes)
HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-8
Server: Microsoft-IIS/10.0
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e709
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb5
7119e709978d2cf1da299e8341753d6f63
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 20:06:29
GMT

Response body (10759 bytes)
Solution Remove emails that are not public
SameSite cookie attribute protection used (2)

GET https://ehikebe.azurewebsites.net:443
Alert
description
The current site use the 'SameSite'
cookie attribute protection on cookie
named 'ARRAffinitySameSite', value is
set to 'None' protection level.
Other info https://tools.ietf.org/html/draft-west-
first-party-cookies
https://chloe.re/2016/04/13/goodbye-
csrf-samesite-to-the-rescue
Request Request line and header section (250
bytes)
GET
https://ehikebe.azurewebsites.net:
443 HTTP/1.1
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.0
Pragma: no-cache
Cache-Control: no-cache
Authorization: Bearer null
Request body (0 bytes)
Response Status line and header section (1142
bytes)
HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-8
Server: Microsoft-IIS/10.0
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e709
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb5
7119e709978d2cf1da299e8341753d6f63
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 20:06:29
GMT

Response body (10759 bytes)
Parameter Cookie named:^
'ARRAffinitySameSite'
Evidence None
Solution CSRF possible vulnerabilities presents on
the site will be mitigated depending on
the browser used by the user (browser
defines the support level for this cookie
attribute).
HEAD https://ehikebe.azurewebsites.net:443

Alert
description
The current site use the 'SameSite'
cookie attribute protection on cookie
named 'ARRAffinitySameSite', value is
set to 'None' protection level.
Other info https://tools.ietf.org/html/draft-west-
first-party-cookies
https://chloe.re/2016/04/13/goodbye-
csrf-samesite-to-the-rescue
Request Request line and header section (242
bytes)
HEAD
https://ehikebe.azurewebsites.net:
443 HTTP/1.1
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.0
Pragma: no-cache
Cache-Control: no-cache
Content-Length: 0
Request body (0 bytes)
Response Status line and header section (1142
bytes)

HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-8
Server: Microsoft-IIS/10.0
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e709
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb5
7119e709978d2cf1da299e8341753d6f63
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 18:08:33
GMT
Response body (0 bytes)
Parameter Cookie named:^
'ARRAffinitySameSite'
Evidence None
Solution CSRF possible vulnerabilities presents on
the site will be mitigated depending on
the browser used by the user (browser
defines the support level for this cookie
attribute).
Risk=Informational, Confidence=Medium (1)

https://ehikebe.azurewebsites.net (1)
Information Exposure Through HTML Comments (script) (1)
GET https://ehikebe.azurewebsites.net:443
Alert
description
While adding general comments is very
useful, some programmers tend to leave
important data, such as: filenames
related to the web application, old links
or links which were not meant to be
browsed by users, old code fragments,
etc.
Other info <!-- Favicon-->,<!-- Bootstrap icons-->,
<!-- Core theme CSS (includes
Bootstrap)-->,<!-- Navigation-->,<!--
Header-->,<!-- Features section-->,<!--
* * * * * * * * * * * * * * *-->,<!-- * *
SB Forms Contact Form * *-->,<!-- * *
* * * * * * * * * * * * *-->,<!-- This
form is pre-integrated with SB Forms.--
>,<!-- To make this form functional,
sign up at-->,<!--
https://startbootstrap.com/solution/cont
act-forms-->,<!-- to get an API token!--
>,<!-- Name input-->,<!-- Email
address input-->,<!-- Phone number
input-->,<!-- Message input-->,<!--
Submit success message-->,<!---->,<!-
This is what your users will see when
the form-->,,,,,<!-
an error submitting the form-->,,,,
Request Request line and header section (250
bytes)

GET
https://ehikebe.azurewebsites.net:
443 HTTP/1.1
Host: ehikebe.azurewebsites.net
User-Agent: Mozilla/5.0 (Windows
NT 10.0; Win64; x64; rv:92.0)
Gecko/20100101 Firefox/92.0
Pragma: no-cache
Cache-Control: no-cache
Authorization: Bearer null
Request body (0 bytes)
Response Status line and header section (1142
bytes)

HTTP/1.1 200 OK
Content-Length: 10759
Content-Type: text/html;
charset=utf-8
Server: Microsoft-IIS/10.0
Strict-Transport-Security: max-
age=31536000; includeSubDomains;
preload
X-XSS-Protection: 1; mode=block
Content-Security-Policy: default-
src 'self'
https://images.unsplash.com data:
https:;script-src 'self' 'unsafe-
inline' 'unsafe-eval'
https://ajax.aspnetcdn.com
https://cdn.jsdelivr.net;style-
src 'self' 'unsafe-inline'
https://cdn.jsdelivr.net;font-src
'self' https://fonts.gstatic.com
https://cdn.jsdelivr.net;block-
all-mixed-content
X-Frame-Options: Deny
X-Content-Type-Options: nosniff
Referrer-Policy: no-referrer
Permissions-Policy: accelerometer=
(), camera=(), geolocation=(),
gyroscope=(), magnetometer=(),
microphone=(), payment=(), usb=()
X-Powered-By: ASP.NET
Set-Cookie:
ARRAffinity=79e06db539acb57119e709
978d2cf1da299e8341753d6f6345007fca
b3f69bc5;Path=/;HttpOnly;Secure;Do
main=ehikebe.azurewebsites.net
Set-Cookie:
ARRAffinitySameSite=79e06db539acb5
7119e709978d2cf1da299e8341753d6f63
45007fcab3f69bc5;Path=/;HttpOnly;S
ameSite=None;Secure;Domain=ehikebe
.azurewebsites.net
Date: Fri, 10 Dec 2021 20:06:29
GMT

Response body (10759 bytes)
Solution Remove comments which have sensitive
information about the
design/implementation of the
application. Some of the comments may
be exposed to the user and affect the
security posture of the application.
Appendix
Alert types

This section contains additional information on the types of alerts in the
report.

CSP: Wildcard Directive
Source raised by a passive scanner (CSP)
CWE ID 693
WASC ID 15
Reference http://www.w3.org/TR/CSP2/
http://www.w3.org/TR/CSP/
http://caniuse.com/#search=content+security
+policy
http://content-security-policy.com/
https://github.com/shapesecurity/salvation
https://developers.google.com/web/fundament
als/security/csp#policy_applies_to_a_wide_var
iety_of_resources
CSP: script-src unsafe-inline

Source raised by a passive scanner (CSP)
CWE ID 693
WASC ID 15
Reference http://www.w3.org/TR/CSP2/
http://www.w3.org/TR/CSP/
http://caniuse.com/#search=content+security
+policy
http://content-security-policy.com/
https://github.com/shapesecurity/salvation
https://developers.google.com/web/fundament
als/security/csp#policy_applies_to_a_wide_var
iety_of_resources
CSP: style-src unsafe-inline

Source raised by a passive scanner (CSP)
CWE ID 693
WASC ID 15
Reference http://www.w3.org/TR/CSP2/
http://www.w3.org/TR/CSP/
http://caniuse.com/#search=content+security
+policy
http://content-security-policy.com/
https://github.com/shapesecurity/salvation
https://developers.google.com/web/fundament
als/security/csp#policy_applies_to_a_wide_var
iety_of_resources
Absence of Anti-CSRF Tokens

Source raised by a passive scanner (Absence of Anti-
CSRF Tokens)
CWE ID 352
WASC ID 9
Reference http://projects.webappsec.org/Cross-Site-
Request-Forgery
http://cwe.mitre.org/data/definitions/352.html
Cookie with SameSite Attribute None

Source raised by a passive scanner (Cookie without
SameSite Attribute)
CWE ID 1275
WASC ID 13
Reference https://tools.ietf.org/html/draft-ietf-httpbis-
cookie-same-site
Cookie without SameSite Attribute

Source raised by a passive scanner (Cookie without
SameSite Attribute)
CWE ID 1275
WASC ID 13
Reference https://tools.ietf.org/html/draft-ietf-httpbis-
cookie-same-site
Cross-Domain JavaScript Source File Inclusion

Source raised by a passive scanner (Cross-Domain
JavaScript Source File Inclusion)
CWE ID 829
WASC ID 15
Incomplete or No Cache-control Header Set

Source raised by a passive scanner (Incomplete or No
Cache-control Header Set)
CWE ID 525
WASC ID 13
Reference
https://cheatsheetseries.owasp.org/cheatsheet
s/Session_Management_Cheat_Sheet.html#we
b-content-caching
https://developer.mozilla.org/en-
US/docs/Web/HTTP/Headers/Cache-Control
Server Leaks Information via "X-Powered-By" HTTP Response
Header Field(s)

Source raised by a passive scanner (Server Leaks
Information via "X-Powered-By" HTTP
Response Header Field(s))
CWE ID 200
WASC ID 13
Reference
http://blogs.msdn.com/b/varunm/archive/201
3/04/23/remove-unwanted-http-response-
headers.aspx
http://www.troyhunt.com/2012/02/shhh-
dont-let-your-response-headers.html
Server Leaks Information via 'X-Powered-By' HTTP Response
Header Field(s)(script)

Source raised by a passive scanner (Script Passive
Scan Rules)
CWE ID 200
WASC ID 13
Server Leaks Version Information via 'Server' HTTP Response
Header Field(script)

Source raised by a passive scanner (Script Passive
Scan Rules)
CWE ID 200
WASC ID 13
Unexpected Content-Type was returned

Source raised by other tools/functionalities in ZAP (for
example, fuzzer, HTTPS Info add-on, custom
scripts...) (plugin ID: 100001)
Email addresses (script)

Source raised by a passive scanner (Script Passive
Scan Rules)
Information Exposure Through HTML Comments (script)

Source raised by a passive scanner (Script Passive
Scan Rules)
CWE ID 615
WASC ID 13
SameSite cookie attribute protection used

Source raised by a passive scanner (Script Passive
Scan Rules)
CWE ID 352
WASC ID 9
