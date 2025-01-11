# GitInsight
GitInsight is a web-app that provides a quick summary of your recent GitHub activity along with a detailed Smart Summary. Quick Summary gives a view of your event count (commits, PRs, etc) on a repository level. Smart Summary is a very powerful way to get feedback on your coding self from multiple LLM powered personas.

## Usage
https://github.com/user-attachments/assets/e730f46f-e9f8-4a27-a59e-a744dd034a46

## Features
- [x] Fetches all public events of a GitHub user
- [x] Filters and stores the following in memory for each repo:
  - [x] Starred status
  - [x] Commit count and messages
  - [x] Pull Request Open count
  - [x] Pull Request Comment count and messages
  - [x] New Members added count
  - [x] Open Issues count
  - [x] Issue Comment count and messages
- [x] LLM Parsing of GitHub Summary with the persona of
  - [x] Software Architect
  - [x] HR Recruiter
  - [x] Potential Partner
- [x] One-page UI for both Quick & Smart Summary
- [x] V1.0.0 Release

## Tech Stack
- Frontend: Thymeleaf for templating HTML, Bootstrap for CSS, HTMX for minimal JS
- Backend: Java, Maven, Spring Boot
- LLM: Gemini API

## Dev Setup
Prerequisites: 
- Java and Maven
- [Create a GitHub API key](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens#creating-a-fine-grained-personal-access-token)
- [Create a Gemini API key](https://ai.google.dev/gemini-api/docs/api-key)

```bash
# Set Environment Variables
export GITHUB_ACCESS_KEY=github_pat_xxx
export GEMINI_ACCESS_KEY=xxxx

# Run the app
mvn spring-boot:run

# Build JAR
mvn clean package -DskipTests
```

## Contributing
Contributions to GitInsight are welcome! If you'd like to contribute, please follow these steps:
- Fork the Repository: Fork the project on GitHub. 
- Create a Branch: Create a new branch for your feature or bug fix. 
- Make Changes: Implement your changes and ensure they are well-tested. 
- Submit a Pull Request: Submit a pull request with a detailed description of your changes.

## License
This code is licensed under the MIT license.

---

_This projects extends the functionality of a [coding challenge](https://roadmap.sh/projects/github-user-activity) in an attempt to make it more useful and accessible for everyone._
