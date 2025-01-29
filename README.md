# GitHub CRUD Operations Postman Collection

This repository contains a **Postman collection** for performing basic **CRUD (Create, Read, Update, Delete)** operations on GitHub repositories using the **GitHub API**.

## Overview

This collection allows you to perform the following operations with GitHub repositories:

1. **Create a Repository**
2. **Fetch Repository Information**
3. **Update Repository Information**
4. **Delete a Repository**

Each operation is tested with Postman scripts to validate the expected behavior. The operations make use of GitHub's RESTful API and require a valid **GitHub personal access token** for authentication.

## Prerequisites

Before using this Postman collection, ensure you have the following:

- A GitHub account with appropriate permissions to create, update, and delete repositories.
- A valid **GitHub personal access token**. You can create one by following the instructions on [GitHub's Personal Access Token](https://github.com/settings/tokens).
- [Postman](https://www.postman.com/downloads/) installed on your system.

## Collection Details

The following operations are implemented in the Postman collection:

### 1. Create Repository

- **Method**: POST
- **URL**: `https://api.github.com/user/repos`
- **Request Body**:
  ```json
  {
    "name": "Postman-repository",
    "description": "A new repository created via Postman",
    "private": false
  }
