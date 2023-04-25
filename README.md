# week9Assignment
# Alexandro Galvez-Vega

# Pen Testing Live Targets

Time spent: 10 hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:

* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each color is vulnerable to only 2 of the 6 possible exploits. First discover which color has the specific vulnerability, then write a short description of how to exploit it, and finally demonstrate it using screenshots compiled into a GIF.

## Blue

Vulnerability #1: SQL Injection


Description: The URL of the salesmen page can betweaked. This is a case of an sql injection in a php web application. ' OR SLEEP(10)=0--' was used in this situation.  

<img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExNWUzOWZmYTgxYzk5Y2QyNjMwYTNjY2ZkMDcwM2FjMWJkNjcxODdjZiZlcD12MV9pbnRlcm5hbF9naWZzX2dpZklkJmN0PWc/NW3j2mHn3Ff7KmmDj8/giphy.gif">


## Green

Vulnerability #1: Stored Cross Site Scripting

Description: There is a contact us page. One simply needs to write a name, email and then something like: <script>alert('Alex was here');</script> in the comment area. It is visible when checking the feedback page. 

<img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExMjEyMmMzNTE1MjkwNDBiNjcwMzAwMmEwOWY5ZDM5ODEyZTc2YTM2MCZlcD12MV9pbnRlcm5hbF9naWZzX2dpZklkJmN0PWc/j8MAcxmnU2UMdbUO6o/giphy.gif">


## Red

Vulnerability #1:Insecure Direct Object Reference

Description: In the sales page it is possible to enter pages that shouldn't be available by changing the number in the url. 

<img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExOTYzZDFmZDI0YzA4ZDY2ZTgwZTRiZTkxZjYzZTgzMGQ3ZWUxOTJkYSZlcD12MV9pbnRlcm5hbF9naWZzX2dpZklkJmN0PWc/002FABQMZdCMOnpPv2/giphy.gif">

<img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExYmI5OTBlY2I2MzQ3YzFhYTZhY2ExNjhmOGZjODIzZjJjOGMwN2ZmZiZlcD12MV9pbnRlcm5hbF9naWZzX2dpZklkJmN0PWc/HxFojwEWJbN0lTK6Vv/giphy.gif">


## Notes

This was generally straightforward overall. 