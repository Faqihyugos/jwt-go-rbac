# Role-based Access Control in Golang with jwt-go

As a security engineer, what's the first thing you check when testing a web or mobile application? Access control misconfigurations must be at the top of your list if you like going for the low hanging fruits first.

Surprisingly, access control is one of the components that application developers think will be simple, but ends up taking much of their time with no end user value, and even worse ends being poorly done, tremendous exposing the application to security risks. It is no coincidence that Authentication and Authorization related issues take the first two positions in the OWASP Top 10 - 2023 list of common API security risks.

For this reason, in this article I am going to illustrate the application of Role-based Access Control; a simple and yet secure access control approach for enterprise APIs.

## Role-based Access Control (RBAC)

Role-based Access Control is a mechanism that restricts access to an information system based on user job functions or roles. Access to data is restricted through permissions and privileges that are attached to different user roles.

Let's Build
By the end of this article we are going build a simple room booking API with Go that will allow visitors to view available rooms as well as register, login and book rooms. There will also be an administrator who will have the permissions map user to permissions as well as add and update rooms information.

<!-- image -->

![Diagram](./img/diagram.avif)

## Prerequisites

- Basic knowledge of Go
- Basic knowledge of RESTful APIs
- Patience 😄
