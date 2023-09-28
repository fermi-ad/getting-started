# Secure sensitive data

Sensitive data, including credentials, should not be stored anywhere in the repositories.

Securing configuration files separately from your code is an essential practice to protect sensitive information such as private keys, database credentials, or other configuration settings. 

Here are several approaches and tools you can use to achieve this:

- Configuration Files Outside the Repository:
Store configuration files outside of your code repository in a separate, secured location on your server. Access to these files should be tightly controlled through permissions and access controls.


- Git Exclusions:
Use .gitignore file  to ignore specific configuration files or directories. This prevents accidentally committing them to your repository.

- Environment Variables:
Store sensitive configuration values, like IPs and hostnames,  as environment variables on your server. This approach keeps sensitive data out of your codebase. You can access these variables in your code programmatically. 

- Secrets Management Systems:
Utilize secrets management systems like HashiCorp Vault  to securely store and manage sensitive configuration data. These systems provide robust security features, access controls, and auditing capabilities. Your application can then retrieve secrets from these systems at runtime.
