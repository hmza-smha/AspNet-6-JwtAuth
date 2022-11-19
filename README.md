# Jwt (JSON Web Token) ASP.NET 6

JWT, or JSON Web Token, is an open standard used to share security information between two parties — a client and a server. Each JWT contains encoded JSON objects, including a set of claims. JWTs are signed using a cryptographic algorithm to ensure that the claims cannot be altered after the token is issued.

- need to install packages
- **Microsoft.EntityFrameworkCore.SqlServer**
- **Microsoft.EntityFrameworkCore.Tools**
- **Microsoft.AspNetCore.Identity.EntityFrameworkCore**
- **Microsoft.AspNetCore.Authentication.JwtBearer**

First of all, we should clarify the difference between these two dependent facets of security. The simple answer is that **Authentication is the process of determining who you are**, while **Authorisation revolves around what you are allowed to do, i.e. permissions**.

## Types of Authentication in ASP.NET:
1. Role Based
1. Claims Based
1. Policy Based

## Role base
- It is something like a boolean type: Do you have this role ? Yes / No
- If you have a driving license, then you can drive a car

## Claims Based
- A set of information that the user give about him self (key/value) pair
- If you have a driving license, then the expire date, gender, type of the car, BOD, ... these are the claims
- Even if you have a driving license you cannot drive any car

## Policy Based
- A set of functions, rules or conditions which are used to check the permission is granted or denied
- claims are rules, a set of rules is a policy
- Do you have a driving license? Is it expired? Can you driva a normal car?
- These conditions are a Ploicy