# Threat Model

## Scenario

Stephen is a teacher in high school. His classroom is equiped with a macintosh computer, connecting to the internet through wifi, rather than using hardwire. His desk is miles away from the ethernet outlet, so it was decided that it would be beneficial to use wifi that is already available school-wide in strong signals rather than using a very long ethernet cable in a cumbersome manner.

Stephen requires frequent access to his computer to pull up his data for class use or to send files to and receive emails from other staff of the school, so it is often the case that he gravitates toward not using any password or pattern to secure his computer. However it should be noted that his computer is constantly under his supervision. The computer is always in front of him when he's at his desk, except when he is in front of the class to teach, or leaves the classroom during lunch time from time to time.

Stephen's general accounts for emails and filesharing services have same email, same password, and logged in all the time for the convenience of quick access. It seems that he prefers to store files on cloud and use emails to send prepared class materials or quizzes/tests from home (rather than using traditional USB sticks) so that he has a backup of his files as long has he has access to internet.

The school wifi which provides internet access to all staff members of the school is password locked. The students are locked out of internet access to restrict them from using smartphones during class, but some students seems to be able to use the wifi for unknown reason.

### Attack Surface
- Lack of password/pattern on his computer
- All accounts are logged in at all times
- All accounts share same password, same email.
- Absence during lunctime -- however infrequent it may be -- leaves his computer exposed.
- Using email or cloud services to store important information.

### Adversaries
- Students
- Other teachers (unlikely)

### Attack vectors
- Possible using USB stick to directly access his computer during his absence in lunctime:

``` 
- Password theft/cracking by injecting script to mine his password for his accounts
- inject keylogger
- inject script to steal password for wifi for school
- stealing important materials (class materials, solutions to tests, quizes)
- invade private information through personal social media (likely to have same passwords and username as his emails)
```

### Mitigations
- Start using some kind of password for his computer to deny initial access to his computer.
- Use different password for his email and cloud service accounts.
- Use 2-factor authentications for all accounts that provide the security measure.
- Use password manager to encrypt; use different password for each account.
- Do not use social media or leave it logged in on company computer (i.e. macintosh)
- Use wired internet rather than wifi for macintosh. (compromises wifi password.)
- Use laptop to access class materials and quizzes/test from cloud or log out every time you don't need to use cloud services on the company computer.
- screenlock/log out or turn computer off when leaving for lunch time.
