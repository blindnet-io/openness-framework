# Checklist for blindnet Open Source Projects

> **How To Use This Document**
>
> 1. Create an issue for the Open Source project containing the following checklist
> 2. Check the boxes to report your progress
> 3. Add comments to discuss and explain how to fulfill complex requirements
> 4. Whenever a subtask become too complexe, open a related issue
>     - if using Github, just click on the circle in the upper-right corner of the task
> 5. Only close the issue after checking all boxes
>
> Please propose updates to this document whenever you see room for improvement, especially if the wording seems imprecise or unclear.
> Make sure to update this checklist every time a community member reports a non-technical issue.

## Basics

- [ ] Code repositories and issue trackers are present (best options: GitHub or Gitlab)
- [ ] No special permission or specific institutional affiliation is required to access the repositories and issue trackers
- [ ] No special permission or specific institutional affiliation is required to clone, build and run the project
- [ ] Project has an associated website
- [ ] No special permission or specific institutional affiliation is required to access any page of the website
- [ ] Website features a project description of less than 100 words
- [ ] Project description is consistent across platforms

## Onboarding

### README

- [ ] Project has README.md file in its root directory
- [ ] README content is clear, concise, and complete
- [ ] README content makes no infringements to the [plain language guidelines](https://www.plainlanguage.gov/media/FederalPLGuidelines.pdf)

### Naming and Presentation

- [ ] Project has a cool name that people can easily remember
- [ ] URL of the repository and title of the README contain the name of the project
- [ ] URL of the repository and title of the README are clear, concise, and do not include any dispensable word

### Onboarding guides

- [ ] Project home page features a quickstart guide for new users
- [ ] Project home page features a quickstart guide for new contributors
- [ ] Installation and first usage of the project can be done in a few minutes by anyone
- [ ] README explains installation and first usage in a few lines
- [ ] README presents a minimum viable feature that hooks the user
- [ ] Project is stable enough to offer this minimum viable feature without any bug or performance and security issue
- [ ] README underlines at least one undebatable and objective strength of the project
- [ ] Minimum viable feature confirms the presented strengths of the project

### Communication channels

- [ ] Project features communication channels exclusively for new users and contributors

## Documentation

- [ ] Documentation is available online
- [ ] Documentation includes a complete yet straightforward tutorial
- [ ] _(if applicable)_ Project as en embedded documentation (e.g. `--help` option for a CLI)
- [ ] Documentation is thorough (covers all use cases and APIs)
- [ ] All users and community members can easily find the documentation (i.e. a link exist and stand out in the README and website)
- [ ] Documentation doesn't present any bug on any tool used to consult it (e.g. a documentation website can be read with any evergreen browser)
- [ ] Anyone can easily report a documentation related issue
- [ ] Anyone can easily contribute to the documentation
- [ ] Community members are encouraged to propose improvements to the documentation
- [ ] Documentation makes as few infringements to [plain language guidelines](https://www.plainlanguage.gov/media/FederalPLGuidelines.pdf) as possible
- [ ] Documentation appears complete
- [ ] Documentation is stylistically consistent 
- [ ] Project features documentation specifically aimed at new users 
- [ ] Project has thoroughly documented installation processes 
- [ ] Project has thoroughly documented process of compiling source code 
- [ ] Project documentation includes use case examples
- [ ] Project creates and maintains documentation via automated processes

## License

- [ ] Project use a valid license according to the Blindnet Open Source Program
- [ ] Project does not require a contributor licensing statement or agreement
- [ ] Project does not feature code with per-file licensing
- [ ] Repository contains a LICENSE file containing the whole text of the license
- [ ] README contains a link to the LICENSE file
- [ ] License is consistent across the whole project (website, documentation, configuration files, code, etc.)
- [ ] License is referred to in every packaged distribution of the project (e.g. npm - package.json)
- [ ] Project doesn't contain any obvious code or dependency that could constitute an infringement of the license

## Development

### Contributing Guidelines

- [ ] The project includes a CONTRIBUTING.md file in its root directory
- [ ] Project clearly identifies opportunities for contributions of different types (code, documentation, design, etc.)

### Developer Documentation

- [ ] Repository includes a complete developer documentation
- [ ] Developer documentation include all installation steps, including prerequisites (with link to the specific part in the tool documentation whenever needed)
- [ ] Anyone, on any operating system, can fulfill the prerequisites for development (dev and testing tools) within an hour

### Testing

- [ ] Repository include testing tools
- [ ] Repository include unit tests
- [ ] Repository include a complete documentation of esting tools, methodes and conventions
- [ ] Anyone can install testing tools and run the tests by only refering to the documentation

### Release management

- [ ] Release policies are documented in the repository and/or website
- [ ] Releases follows a consistent versionning conventions (semver is recommanded by default)
- [ ] Release process is automated and documented
- [ ] Release process include clear guidelines to document changes and intentions in every release
- [ ] All releases are well documented
- [ ] Project has issued a release in the last 6 months
- [ ] Project publish releases at consistent intervals
- [ ] Project has implemented a quality assurance process
- [ ] Project uses automated continuous integration and development tooling
- [ ] Project releases are available from consistent download location
- [ ] Project releases software in multiple formats

### Activity

- [ ] The main branch of the repository 
- [ ] Project has issued a release in the past 12 months
- [ ] Project releases software at consistent intervals

## Organisation

### Governance

- [ ] Project has clearly identified lead maintainers 
- [ ] Project has identified means of contacting lead maintainers
- [ ] Project has identified various roles contributors can occupy
- [ ] README and CONTRIBUTING make mention of the Blindnet Openness Framework
- [ ] Project makes and records decisions publicly according to the Blindnet Openness Framework

### Code of Conduct

- [ ] A Code of Conduct has been defined for the project
- [ ] Code of Conduct is presented in README and CONTRIBUTING
- [ ] Anyone can easily identify where and how to report an infraction to the Code of Conduct
- [ ] Anyone can report an infraction to the Code of Conduct without any other requirement than having access to a largely used tool (e.g. email client or web browser)
- [ ] Report of an infraction to the Code of Conduct can be treated in less than two working days

## Outreach

### Prerequisites

- [ ] The Github repository for the project as a minimum amount of stars (20+) :arrow_right: Ask employees, partners, contributors, and friends to support the project before launching any large scale communication

### Instant Messaging Space

- [ ] An instant messaging space has been created for the project and is easily accessible
- [ ] Community members can easily find a link/invitation to the instant messaging space in the repository and documentation home page
- [ ] The instant messaging space is sufficiently active to allow any message to be answered within two hours (at least during working hours)

### Website

- [ ] Website features other publicly visible sites or subdomains
- [ ] Website contains clear description of project and its purpose
- [ ] Website features consistent stylistic and navigational elements
- [ ] Website features software binaries download link
- [ ] Website features multiple download formats
- [ ] Website content and copyright notices are current
- [ ] Website contains a GDPR policy and other relevant privacy policies
- [ ] Website explains project's governance model
- [ ] Website does not include references to outdated, unused, or legacy tooling

### Social Platforms

- [ ] The project has been presented on Reddit
- [ ] The project has been presented on Hacker News
- [ ] Project can be associated with a Twitter account
- [ ] Project can be associated with a LinkedIn organisation
- [ ] Each new version of the projects leads to a post on Twitter and Linkedin
- [ ] Project responds to social media inquiries within 12 hours
- [ ] Project updates its social media at least once per week
- [ ] All contributions leads to a tweet, with an short explainer and a thank you note to the contributor

### Blog

- [ ] A blog is associated with the project (organization, company, or project itself)
- [ ] README include a link to the blog
- [ ] At least one post on Dev.to and the blog introduce the strengths and minimum viable feature of the project
- [ ] Blog is updated to explain every new version of the project the same day it is published
- [ ] Blog is updated at least once per month
- [ ] All blog posts contain less than 1500 words (<15 minutes to read)
- [ ] Technical blog posts make as few infringements to [plain language guidelines](https://www.plainlanguage.gov/media/FederalPLGuidelines.pdf) as possible
- [ ] Every new blog publication is announced with a tweet and a post on LinkedIn

## Contributions

- [ ] README include an [all-contributors](https://github.com/all-contributors/all-contributors
) section as soon as more than three persons outside the core team contributed to the code base
- [ ] Any new issue and pull request receive an answer within 12 hours

<br/>

---

<br/>

## Definitions/Clarifications

- "Within X hours/days" only includes working hours and days

## References

Some parts of this document has been inspired by:

- The Red Hat [Checklist for measuring the health of an open source project](https://www.redhat.com/en/resources/open-source-project-health-checklist)
- The [Open source promotion cheat sheet](https://github.com/zenika-open-source/promote-open-source-project)
