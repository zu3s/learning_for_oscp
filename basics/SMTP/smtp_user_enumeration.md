# SMTP User Enumeration
quoted from [this site](https://pentestlab.blog/2012/11/20/smtp-user-enumeration/)

SMTP is a service that can be found in most infrastructure penestration tests. This service can help the penestration tester to perform username enumeration via the EXPN and VRFY commands if these commands have not been disabled by the system administrator. There are a number of ways which this enumeration through the SMTP can be achieved.

The role of the EXPN command is to reveal the actual address of users aliases and lists of email and VRFY which can confirm the existence of names of valid users.

The SMTP enumeration can be performed manually through utilities like telnet and netcat or automatically via
a variety of tools like metasploit, nmap and smtp-user-enum. The following 2 screenshots are showing how we can enumerate users with the VRFY and RCPT commands by using the telnet service.
![](https://pentestlab.files.wordpress.com/2012/11/smtp5.jpeg)
![](https://pentestlab.files.wordpress.com/2012/11/smtp6.jpeg?w=500)

Another tool that can be used is **smtp-user-enum** representative way to use it in backtrack is shown below.
`perl smtp-user-enum.pl -M VRFY -U users.txt -t 172.16.212.133` 
It also can be used for discovery valid email addresses.
`perl smtp-user-enum.pl -M VRFY -D 


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTkwNjk4MjkxOCwxNjk5NjcxNzc3LDIwMT
QyMTA5MDNdfQ==
-->