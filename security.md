# Don’t Trust the User


The principle of least trust offers a solution. Any data that enters your application has to be validated before it is used. Act like border patrol--inspect any data trying to come into your application, determine if it’s safe, then let it in. If it’s unsafe or you can’t tell, reject it (nicely, in case of an actual error on the part of a legitimate user).

Many tools used by unsophisticated attackers depend on vulnerabilities like injection and XSS to gain easy access. Don’t be an easy target for the 12-year-old down the street.


# Keep It Secure and Simple (KISS)

Simple is easier to secure. Keep your designs simple, and you can prove the security of a system.

Unfortunately, some developers overthink the design (it happens to everyone at some point) and add too many hoops, bells, and whistles. Over time, an application may grow and become a complex behemoth that is hard to understand and even harder to secure. Try your best not to let this happen.

Think of your software in terms of the business outcome it enables. Software isn’t a place to create works of art or to impress your friends with how clever you can be. One visit to The Daily WTF will show you how strange software architecture can get.



# Automation is Your Friend


Unfortunately, security has been viewed as an impediment to getting things done instead of an enabler. That mindset has to change on both sides.

An effective way to incorporate security into your code is through automation. Automation reduces the chance of human error. It puts important processes on autopilot and can eliminate dangerous variables.



# Threat Model Your Software


Threat modeling is the practice of examining a software design to find places where attackers could compromise it. Threat modeling helps developers to understand how attackers could compromise their software so they can build in the appropriate defenses.

The first step to building secure software is not learning new syntax or coding techniques. You need to understand how attackers break into software systems. Walk through a compromise to see how easy a data breach could happen if you write code or design the application in the wrong way.

If you’ve never threat modeled an application before, here are the basic steps:

Document how the application functions, focusing on the flow of data through the application.

Find threats against the application by following the flow of data and identifying places weak to certain exploits (attack databases work well here).

Address threats by rating them and deciding on mitigation strategies.

Validate the model to make sure you didn’t miss anything.




# Get Your Cryptography Right

Data is the lifeblood of the business and the life of your users. A massive data breach can take years, and millions of dollars, to recover from. Good cryptographic processes help to mitigate the damage if the worst happens.

When done incorrectly, cryptography is a waste. Making common cryptographic mistakes leads to disaster when good attackers figure out what you’re doing. Here are some do’s and don’ts for cryptography:

DON’T store cryptographic keys in the same place as the data it encrypts.

DON’T hard code cryptographic keys in the code.

DO use secure key vaults to store cryptographic keys (Vault, AWS KMS, and Azure Key Vault).

DON’T create your own cryptographic algorithms or use broken algorithms.

DO use known good algorithms provided by your framework (AES-256, Argon2, PBKDF2).

DO encrypt data at rest and in transit.

DO have a security expert review any code using cryptography.