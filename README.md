# DAV-6100-Teachback-Assignment
Presenting on how a REST API works 

# Presentation: Explaining How a REST API Works

## Purpose of the Repository

This repository complements the presentation on "Explaining How a REST API Works." It includes the presentation slides, code snippets, and resources used during the live demonstration. Feel free to explore the content to gain a deeper understanding of RESTful architectures and follow along with the presentation.

## Presentation Overview

The presentation covers fundamental concepts of RESTful APIs, including principles, HTTP methods, URI design, request/response structure, status codes, best practices, and tools. The live demonstration showcases practical aspects using Postman, illustrating how to make simple REST API requests, interpret responses, and understand different HTTP methods.

## Code Snippets and Examples

### 1. Making a GET Request using Postman

- **File:** `demo/get-request-example.http`
- **Description:** This example demonstrates how to make a simple GET request to a REST API endpoint using Postman.

```http
GET https://api.example.com/users/123

Resources
Postman Download
GitHub Repository for Further Exploration
-------------------------------------------
import requests

# Replace this URL with the actual endpoint you want to request
api_url = "https://api.example.com/users/123"

# Make a GET request
response = requests.get(api_url)

# Check the response status
if response.status_code == 200:
    # Print the response content (assuming it's in JSON format)
    print("Response Content:")
    print(response.json())
else:
    print(f"Failed to make GET request. Status Code: {response.status_code}")
    print(response.text)

#OR

#CODE-2

import requests
import base64

# Replace these values with your GitHub username, repository name, and personal access token
username = "your-username"
repository = "your-repository"
token = "your-personal-access-token"

# GitHub API endpoint for creating or updating a file
api_url = f"https://api.github.com/repos/{username}/{repository}/contents/README.md"

# Content of the README.md file
readme_content = """
# Your Presentation Title

This repository contains slides and resources for my awesome presentation.

## Slides

- [Presentation Slides](presentation-slides.pdf)

## Code Snippets

### Python Example

```python
print("Hello, world!")


# (Please replace the placeholder values (`your-username`, `your-repository`, `your-personal-access-token`) with your actual GitHub username, repository name, and a personal access token with the required permissions.

# Remember to install the `requests` library if you haven't already:

pip install requests

#This script sends a PUT request to the GitHub API, creating or updating the README.md file in your repository with the specified content. It's a basic example, and you might want to enhance it based on your specific requirements.
