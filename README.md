# xAPI.NET

THIS DOCUMENT IS CURRENTLY IN DRAFT.

xAPI.NET is a Microsoft ASP.NET Core solution implementing a full Learning Record Store (LRS), and Learning Management System (LMS) using the Experience API (xAPI).

## What is the Experience API (xAPI)?

The Experience API (xAPI), formily known as the Tin Can API, is an open-source e-learning software specification that allows learning content and learning systems to speak to each other in a manner that records and tracks all types of learning experiences. This new specification is the successor to SCORM (Sharable Content Object Reference Model). 

To learn more please read [Advanced Distributed Learning's Overview of xAPI](https://www.adlnet.gov/adl-research/performance-tracking-analysis/experience-api/).

## What is a Learning Record Store (LRS)?

A Learning Record Store (LRS) is essentially the server used to store learning data collected with the xAPI. The server would listen to requests (GET, PUT, POST, etc) and perform CRUD operations to a database. This project will be utilizing Entity Framework Core ORM and SQL Server.

## What is a Learning Management System (LMS)?

A Learning Management System (LMS) is simply a piece of software designed for learners to interact with your course content. Typically this software is seen as a web site or web app that handles user authentication, course registration, course completion, and some account management. The LMS is what and how your learners consume your course content.

The LMS sometimes includes, or is accompanied by a LCMS (Learning Content Management System). If the LMS is the "front-end" of the app, you can think of the LCMS as being the "back-end" of the app. This is where courses can be authored, published, and maintained. 

## Why xAPI.NET?

The ADL maintains a lot of their documentation, as well as example code, [here on GitHub](https://github.com/adlnet). Much of what can be found across the web are either proprietary software offerings - CoTS or SaaS, or bits and peices of functioning code written in PHP, Python, or Java.

What I discovered was a huge gap: little to nothing is provided for in-house teams to get started with xAPI in a Microsoft environment (or anywhere that runs ASP.NET Core framework). Thus I've decided to simultanously teach myself everything there is to know about xAPI, and provide a foundation fluid enough to be used in any project that can benefit from all that xAPI has to offer.

It's important to note that while this project aims to provide a web site or web app solution, other solutions are easily achievable. You may later on discover a business case where native apps (mobile, tablet) or desktop software (Windows, Mac, Linux) may make sense. The Web API portion of this project will prove useful and provide the extensibility you need to execute these projects with ease.

### Scope & Roadmap

1. Microsoft Identity configured for Local Accounts, Active Directory, and various oAuth providers.
2. Complete implementation of the xAPI specification using ASP.NET Core Web API.
3. Port the [ADL's LRS](https://github.com/adlnet/ADL_LRS) to ASP.NET Core and SQL.
4. Port or implement the [ADL's LRS Conformance Test Suite](https://github.com/adlnet/lrs-conformance-test-suite) to validate our LRS against specs.
5. Design then develop a simple LMS to accompany xAPI and LRS for a full-featured solution.

### Dependencies

Dependencies are TBD at this stage of the project.

### Requirements

- Server environment with support for ASP.NET Core framework.
- Accessible Microsoft SQL Server database.
- Evergreen or latest version of a popular web browser: IE11, Edge, Chrome, Firefox, Brave, or Safari.
