Secret Management Policy
=============================

## Purpose

The purpose of this policy is to outline the procedures and responsibilities for managing keys in the codebase and 
mitigating the risks associated with secrets leaked in the codebase. This ensures that our systems remain secure and 
that sensitive information is protected against unauthorized access.

##  Scope

_* This policy applies to all software development projects, repositories, and environments within VisitScotland. It 
covers the detection, handling, and remediation of leaked secrets across all stages of the software development 
lifecycle._

## Definitions

- **Secret**: Sensitive information such as passwords, API keys, tokens, encryption keys, and other credentials that 
  grant access to systems or data or authenticate requests
- **Production Secret**: A secret used in the production environment, essential for the operation of live systems. These
  secrets are rarely shared with developers and they tend to be used only in production and staging environments.
- **Test Secret**: A secret used in non-production environments, such as development or testing, used for testing 
  purposes only. However, Test secrets need to be carefully handled as they might grant access to services or result in
  a breach of agreement with third-party systems. 
- **Non-Secret Key**: An API key that does not provide access to sensitive data or critical functionalities and is 
  considered low-risk if exposed. The most common example is a key that needs to be used by JavaScript and can be read 
  in the source code of a page. While it is not classified as a secret, it is still preferred to manage it properly to 
  maintain best practices in code management and security hygiene. See more information about 
  [Non-Secret Key Management](key-management.md)

### Types of Secrets

- **API Keys**: Credentials used to authenticate applications with external services.
- **Passwords**: Credentials used to access databases, services, or systems.
- **Tokens**: Access tokens or refresh tokens used for authentication and authorization.
- **Certificates**: SSL/TLS certificates or other cryptographic keys used for securing communications.
- **Environment Variables**: Sensitive data stored as environment variables in deployment configurations.


## What to do when a vulnerability is found

### Assessment

1. **Alert**: Use GitGuardian to detect and alert on leaked secrets on code commit.  
2. **Review**: If the secret is a false positive. In case of false positive resolve the issue and including an 
   explanation why the issue is considered a false positive. Note: Test Secrets are not false positive and they need to
   be carefully considered as they might grant access to public facing services
3. **Determine the Type**: Identify whether the leaked secret is a production secret, a test secret or a non-secret key.
4. **Assess the Impact**: Evaluate the severity and potential impact of the leak on systems, data, and user security.
5. **Open Source**: Identify whether the project is Open Source or not. Open Source projects
6. **Report**: Report the issue to your technical leader to make sure that the issue has been dealt correctly. They 
   might help to validate that the proper action has been or will be performed
   
### Remediation
If the secret relates to an Open Source Repository
1. **Revoke the Secret**: Immediately revoke the leaked secret to prevent unauthorized access. For instance, rotate API 
   keys, reset passwords, or invalidate tokens.
2. **Update Configuration**: Replace the leaked secret with a new, secure value in all relevant systems and codebases.
3. **Remove from History**: Ensure the secret is removed from the code repository history. Use tools like 
 _git filter-branch_ or _BFG Repo-Cleaner_ to clean the repository history.


### Report
1. **Document the Incident**: Record details of the leak in GitGuardian, including the type of secret, the steps taken 
   to remediate it, and any lessons learned. 
2. **Implement Preventive Measures**: Update security practices, tools, and workflows to prevent similar incidents in 
   the future. This may include enhancing code review practices, improving secret management practices, or increasing 
   training for developers.

## Best Practices for Secret Management

   **Environment Variables**: Store secrets in environment variables instead of hardcoding them in the source code or
   properties files
   **Secret Management Tools**: Utilize dedicated secret management tools like AWS Secrets Manager to manage and store 
   secrets securely.
   **Principle of least privilege**: Ensure that only necessary services and users have access to secrets.


## Policy Compliance
Compliance with this policy is mandatory. Failure to comply with this policy will result in stricter processes
