---
author: Alfie Farren
pubDatetime: 2024-06-26T00:00:00Z
title: A Successful Approach to Migrating your API Docs to GitBook
postSlug: api-docs-gitBook-fast-pipeline-scalable
featured: true
draft: false
tags:
  - Documentation
  - Protected
  - Hosted
  - Auth0
  - Github
  - Actions
  - AWS
  - Integration
  - Postman
  - ApiDog
  - GitBook
description:
  Apparently this is not quite straight forward without too much effort, firstly when Postman collections are converted to MD or MDX files a lot of compatibility issues and side-effects happen with CLI tools that are used to consume and turn them into static websites.
---

## Introduction
Migrating API documentation can be a daunting task, especially when dealing with compliance requirements and the need for a visitor-protected environment. Here’s a journey of how I overcame several challenges to successfully migrate my API documentation to GitBook in less than 2 hours.

## The Challenge
It all started with a compliance request to put our product API docs behind a visitor-protected environment to control access to the content. Initially, we used Postman collections for our API documentation, but this approach came with its own set of challenges.

## The Problems Encountered
1. **Postman Collection Conversion Issues:**
    - The Postman collections did not convert properly to MD or MDX files, leading to numerous compatibility issues with CLI tools.

2. **Lack of Essential Features in Postman:**
    - Postman doesn't support integration with Auth0 or visitor-protected features, which are crucial for our compliance requirements.

3. **Initial Setup and Migration Hurdles:**
    - There was a lack of comprehensive content available about migrating Postman collections to Authorized spaces, making the process more complex.

## The Turning Point
After several trials and errors, I found a more streamlined approach using a combination of GitBook and APIDog. Here’s how it all came together:

## Understanding the Tools
1. **GitBook:**
    - GitBook is a powerful documentation platform that allows you to create beautiful documentation with ease. It supports Markdown, offers extensive customization options, and integrates seamlessly with various authentication providers to ensure secure access.

2. **APIDog:**
    - APIDog is a tool designed to help developers manage and convert API documentation. It can take Postman collections and convert them into Markdown files, making it easier to integrate with platforms like GitBook.

## The Solution
1. **Export Postman Collection:**
    - I exported the Postman collection as Collection 2.1, which provided a JSON file that was easier to work with.

2. **Import to APIDog:**
    - The JSON file was then imported to APIDog, a tool that facilitated the conversion and extraction process.

3. **Extract Markdown File:**
    - APIDog enabled me to extract a Markdown (MD) file from the JSON, which was crucial for the next steps.

4. **Setup GitBook Account:**
    - I set up an account on GitBook, a platform known for its powerful documentation capabilities and user-friendly interface.

5. **Import to GitBook:**
    - The Markdown file was then imported into GitBook, where it could be further customized and organized.

6. **Customization and Integration:**
    - I customized the domain and styles to match our brand's look and feel.
    - Integrated with an authentication provider to ensure the documentation was secure and compliant with the visitor-protected requirement.

7. **Enhanced Editorial Functions:**
    - Finally, I integrated GitBook with GitHub, Google Docs, and Slack, streamlining the content editorial process and enabling faster updates and collaboration.

## The Result
The end result was a beautifully hosted API documentation site on [https://api-docs.quickclaim.io](https://api-docs.quickclaim.io). The site not only met our compliance requirements but also provided a much more efficient and user-friendly documentation experience. Impressively, this entire setup and migration process took less than 2 hours.

## Conclusion
Migrating API documentation can be complex, but with the right tools and a bit of perseverance, it is definitely achievable. Using GitBook and APIDog proved to be a game-changer, turning a challenging project into a success story.

