# Application Configuration Documentation

## Create a YAML Configuration for an Application

## Module

Scripting & Cloud Fundamentals

## Document Type

Technical Documentations

---

## 1. Introduction

This document describes the process of creating, validating, and converting a YAML configuration file for a sample web application. The configuration defines core application settings such as application metadata, server details, and database connection parameters.

YAML (YAML Ain't Markup Language) is widely used in cloud computing, DevOps, and infrastructure automation due to its readability and structured format.

---

## 2. Objective

The objective of this documentation is to:

* Demonstrate correct YAML syntax and structure
* Validate a YAML configuration file
* Convert YAML configuration into JSON format
* Provide evidence of successful validation and conversion

---

## 3. Prerequisites

To complete this task, the following were required:

* A text editor (VS Code or equivalent)
* Basic understanding of indentation and key-value data structures
* Internet access for validation and conversion tools

---

## 4. Application Configuration Structure

The configuration file is organized into three main sections:

* **Application**: Defines the application name, version, and environment
* **Server**: Specifies the host address and port number
* **Database**: Contains database engine and connection credentials

---

## 5. YAML Configuration File

**File Name:** `app-config.yaml`

```yaml
application:
  name: my-web-app
  version: 1.0.0
  environment: production

server:
  host: 0.0.0.0
  port: 8080

database:
  engine: mysql
  host: db.example.com
  port: 3306
  username: admin
  password: mysecurepassword
```

This file uses consistent two-space indentation and follows standard YAML formatting rules.

---

## 6. YAML Validation

The YAML file was validated to ensure correctness and absence of syntax errors.

**Validation Tool Used:**

* [https://www.yamllint.com](https://www.yamllint.com)

**Validation Result:**

* The file passed validation successfully with no errors.

A screenshot of the validation result is stored as `validateyaml.png`.

---

## 7. YAML to JSON Conversion

After validation, the YAML configuration was converted into JSON format.

**Converted File Name:** `app-config.json`

```json
{
  "application": {
    "name": "my-web-app",
    "version": "1.0.0",
    "environment": "production"
  },
  "server": {
    "host": "0.0.0.0",
    "port": 8080
  },
  "database": {
    "engine": "mysql",
    "host": "db.example.com",
    "port": 3306,
    "username": "admin",
    "password": "mysecurepassword"
  }
}
```

**Conversion Tool Used:**

* [https://jsonformatter.org/yaml-to-json](https://jsonformatter.org/yaml-to-json)

A screenshot of the conversion result is stored as `yml_to_json.png`.

---

## 8. Project Directory Structure

```
Create_a_YAML_Configuration/
├── app-config.yaml
├── app-config.json
└── screenshots/
    ├── validateyaml.png
    ├── yml_to_json.png
    └── links.txt
```

The `links.txt` file contains references to the validation and conversion tools used.

---

## 9. Best Practices

* Use consistent indentation (2 or 4 spaces)
* Avoid tabs in YAML files
* Do not store sensitive credentials in plain text for production environments
* Always validate configuration files before deployment

---

## 10. Conclusion

This documentation demonstrates the successful creation, validation, and conversion of a YAML configuration file for a web application. The task reinforces best practices in configuration management and provides a foundation for working with YAML in cloud and DevOps environments.

---
