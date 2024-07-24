Management of Non-Secret Keys and Sensible Configuration Values
===============================================================

## Purpose

The purpose of this document is to outline the different types of Keys and Configuration that might not be considered 
secrets. They do not provide access to sensitive data or critical functionalities and is considered low risk if exposed. 
While it is not classified as a secret, it is still preferred to manage it properly to maintain best practices in code 
management and security hygiene.

## Guidelines for Management

### Storage
- **Environment Variables**: Store non-secret API keys in environment variables rather than hardcoding them in the 
  source code. This helps in maintaining cleaner code and reduces the risk of accidental exposure.
- **Configuration Files**: If using configuration files, ensure they are not committed to version control. 
 Use .gitignore file to exclude these configuration files from the repository.
- **Secret Management Tools**: By using secret management tools, you can ensure that this values are securely stored
  outside the codebase.

### Documentation:
- **Include Instructions**: Provide clear documentation on how to configure and use non-secret API keys, including steps 
- for setting environment variables or using local configuration files.

### Usage:
- **Exclude from Codebase**: Do not hardcode non-secret API keys directly in the codebase. Use placeholder values in the
  code and provide instructions on how to replace them with actual values during the deployment or development setup 
  process.
- **Code References**: In the code, refer to these values as references and **never hard-code the values**

## Use cases

- **Internal URLs**: Internal or External Service URLs are not considered secrets or keys and they can be included in
  the code. (i.e. https://jenkins.visitscotland.com/service)
- **IP Address**: They are not considered secret and they classify as _Internal URLs_ but it is best practices not to 
  use IP addresses as these addresses might change and they reveal information about internal topology. Please request 
  an equivalent domain URL when possible. (i.e. http://192.168.20.24:1234)
- **Public API keys**: For accessing free, rate-limited services. They should not be included in the code base 
  (i.e. marketo-munch, recaptcha key, GTM id, etc ...)
- **Access Token**: Even though this keys might be exposed in a webpage they might need to be treated as **secret** 
  please read carefully the Terms and Condition of the Contract **before using** any access token.

## Policy Compliance

Compliance with these guidelines is encouraged to maintain high standards of code management and security. While 
non-secret API keys do not pose significant risks, adhering to these practices helps in maintaining a secure and 
professional codebase.

This policy is significantly more important for Open-Source Projects.

