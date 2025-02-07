# SecureCode
# OWASP Based Checklist  • 200+ Test Cases  Content  
C JAVA  C++  PYTHON  JAVASCRIPT  RUST  GOLANG

# 1. Input Validation
 The "Input validation" section in your Secure Coding Practices checklist involves measures to ensure that data coming into your application is safe and free from potential security 
 risks. It includes practices like conducting validation on trusted systems, distinguishing between trusted and untrusted data sources, specifying character sets, validating data types, 
 lengths, and ranges, and being cautious about potentially hazardous characters. The goal is to prevent malicious data from entering your application and to handle it safely if it must be 
 allowed. These practices help safeguard against common security vulnerabilities, such as injection attacks, by ensuring that only well-formed, expected, and safe data is processed.

# 1.1 Conduct all data validation on a trusted system
  Ensure that all data validation is performed on the server, not onthe client side.
  This prevents validation rules from being Bypassed by manipulating client-side code. 
  When a user submits a form, the server checks the input data for validity and rejects it if it doesn't meet the criteria. Client-side JavaScript should not be relied upon for validation.

# 1.2 Identify all data sources and classify them 
 Classify data sources as trusted (e.g., internal databases) or untrusted (e.g., user input, external APIs). Validate all data from untrusted sources to prevent malicious input. 
 When processing data from user-submitted forms and external APIs, ensure that all input is thoroughly validated, regardless of its source.

# 1.3 Centralized input validation routine
Implement a centralized input validation routine to ensure consistent and thorough validation across the application.
Create a single validation function that is called for all user input, ensuring that every input is consistently validated according to predened rules.
