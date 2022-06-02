# Class35 Reading Notes

Readings: API Deployment

Below you will find some reading material, code samples, and some additional resources that support today’s topic and the upcoming lecture.

Review the Submission Instructions for guidance on completing and submitting this assignment.

Reading

[Django Settings Best Practices](https://djangostars.com/blog/configuring-django-settings-best-practices/)

1. Keep settings in environment variables.
2. Write default values for production configuration (excluding secret keys and tokens).
3. Don’t hardcode sensitive settings, and don’t put them in VCS.
4. Split settings into groups: Django, third-party, project.
5. Follow naming conventions for custom (project) settings.

-- Naming Conventions Give meaningful names to your settings. Always use the prefix with the project name for your custom (project) settings. Write descriptions for your settings in comments.

**12 Factors** is a collection of recommendations on how to build distributed web-apps that will be easy to deploy and scale in the Cloud. 

Codebase
Dependencies
Config
Backing services
Build, release, run
Processes
Port binding
Concurrency
Disposability
Dev/prod parity
Logs
Admin processes

[SSH Tutorial](https://www.hostinger.com/tutorials/ssh-tutorial-how-does-ssh-work)

SSH, or Secure Shell Protocol, is a remote administration protocol that allows users to access, control, and modify their remote servers over the internet.

The SSH command consists of 3 distinct parts:

ssh {user}@{host}

-The SSH key command instructs your system that you want to open an encrypted Secure Shell Connection. 

-{user} represents the account you want to access.

-{host} refers to the computer you want to access. 

Symmetrical encryption -Symmetric encryption is a form of encryption where a secret key is used for both encryption and decryption of a message by both the client and the host.

Asymmetrical encryption -asymmetrical encryption uses two separate keys for encryption and decryption.

Hashing -One-way hashing is another form of cryptography used in Secure Shell Connections. 

There are two stages to establishing a connection – first, both the systems must agree upon encryption standards to protect future communications, and second, the user must authenticate themselves. If the credentials match, then the user is granted access.

Bookmark and Review

[White Noise](http://whitenoise.evans.io/en/stable/)

[IaaS](https://en.wikipedia.org/wiki/Infrastructure_as_a_service)

[PaaS](https://en.wikipedia.org/wiki/Platform_as_a_service)

[CORS](https://en.m.wikipedia.org/wiki/Cross-origin_resource_sharing)


----

## Things I want to know more about

----
[Home](https://github.com/MISalz/401_Reading_Notes/blob/main/README.md)