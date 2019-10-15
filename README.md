# Tech Debt - Prevention, Diagnosis and Cure

A tech debt reading and resources list. It contains lots of ways to diagnose, prevent and control tech debt.

This is a WIP! Please add any resources you find interesting by forking and creating a pull request.

**Table of Contents** 

- [🏁 Start here](#-start-here)
- [🎖 Case Studies](#-case-studies)
- [⛔ Prevention](#-prevention)
  - [🤝 Requirements](#-requirements)
  - [📡 Infrastructure](#-infrastructure)
  - [🏛️ Architectural](#-architectural)
  - [🎨 Design](#-design)
  - [💻 Code](#-code)
  - [✅ Testing](#-testing)
  - [🛠️ Build](#-build)
  - [📝 Documentation](#-documentation)
  - [🏚️ Versioning](#%EF%B8%8F-versioning)
- [🏥 Remediation](#-remediation)
  - [🔍 Post Mortems](#-post-mortems)
  - [💣 High Interest Debt First](#-high-interest-debt-first)
  - [🧭 Boy Scout Rule](#-boy-scout-rule)
  - [🧰 Tools](#-tools)
- [Contributing](#contributing)
- [Authors](#authors)
- [License](#license)
- [Sponsors](#sponsors)

## 🏁 Start here

[What is tech debt](https://www.youtube.com/watch?v=pqeJFYwnkjE)

* [Ward Cunningham](https://twitter.com/WardCunningham) coined the term "tech debt".
* Talks about history, motivation and common misunderstanding of the "debt metaphor" for refactoring.

[Classifying Technical Debt](https://martinfowler.com/bliki/TechnicalDebtQuadrant.html)

* [Martin Fowler](https://twitter.com/martinfowler) makes two disctions (1) prudent and reckless debt, and (2) deliberate and inadvertent debt. A classic

[Identifying when Technical Debt needs action](https://blog.crisp.se/2013/10/11/henrikkniberg/good-and-bad-technical-debt)

* [Henrik Kniberg](https://twitter.com/henrikkniberg) argues that older tech debt is bad, whereas new tech debt is acceptable in order to build prototypes.
* Concept of a qualitative debt ceiling technique to manage the level of technical debt.

[The Human Cost of Technical Debt?](https://daedtech.com/human-cost-tech-debt/)

* [Erik Dietrick](https://twitter.com/DaedTech) goes into depth for how technical debt can harm teams.
* There includes discussion on (1) unpleasant work (2) team infighting (3) atrophied skills (4) turnover and attrition.

## 🎖 Case Studies

[Ticketmaster](https://tech.ticketmaster.com/2015/06/30/what-ticketmaster-is-doing-about-technical-debt/)

* Step-by-step guidance on how Ticketmaster assessed their technical debt over 12 months.

[Stripe](https://www.infoq.com/presentations/stripe-technical-debt/)

* [Will Larson](https://twitter.com/lethain?lang=en) explains how Stripe use migrations to get away from tech debt.

[A large bank](http://neopragma.com/index.php/2019/03/30/technical-debt-the-man-the-metaphor-the-message/)

* [Dave Nicollete](https://twitter.com/davenicolette) covers a detailed case study, with costs, of resolving prudent-intentional debt.
* Costs of the cleanup and the business impact included.

[Optimizely design debt approach](https://medium.com/design-optimizely/pay-down-design-debt-with-polish-day-867eb59dd83d)

* [Dave Rau](http://daverau.info/) explains how when Optimizely got to 50 UI issues, they decided to do something about it.
* The team ran a 'Polish Day' once a week, with a points system for designers to prioritize work.

[Paddy Power](https://www.researchgate.net/publication/271635510_Continuous_Delivery_Huge_Benefits_but_Challenges_Too)

* [Lianping Chen](https://twitter.com/lianpingchen)'s article explains why the Paddy Power team decided to adopt Continuous Delivery, and explains the benefits and challenges involved.

## ⛔ Prevention

### 🤝 Requirements

[Creating a Product Canvas](https://www.ebgconsulting.com/blog/using-product-canvas-define-product-getting-started/)

* [Ellen Gottesdiener](https://twitter.com/ellengott) provides a canvas to convey what the product is, and how it is strategically positioned.
* The first part of the canvas comes _before_ everything else and gives the context. It goes from vision through other high level areas such as revenue, competitors, and the innovation landscape.
* The second part of the template is used to explain product requirements.

[Story Mapping](https://www.jpattonassociates.com/the-new-backlog/)

* [Jeff Patton](https://twitter.com/jeffpatton) invented the concept of Story Mapping (you can see a [video of this process](https://www.youtube.com/watch?v=XzaCaW8c3qE) here) 
* Flat product story backlogs are hard to understand - they are just a pile of features. By visualising an entire system with it can be much easier to spot opportunities or weaknesses, or indeed to work with other stakeholders in requirements gathering.
* Create a series of cards with big stories (activities) at the top, down to tasks and then sub tasks.

[Joint Application Design](https://www.pmi.org/learning/library/determining-project-requirements-best-practices-7278)

* This is a thorough run-through by the Project Management Institute for Joint Application Design. It gives guidance on how to run design sessions for multi-stakeholder requirements gathering.

### 📡 Infrastructure

[DevOps 101](https://opensource.com/article/19/4/devops-pipeline)

* [Bryant Son's](https://twitter.com/bryantjiminson) simple guide that guides you through the basic setup to enable you to build you first pipeline
* Covers (1) CI/CD Tools (2) source control management (3) build automation (4) web app servers (5) code testing coverage

*TODO*: Add better DevOps resources here

### 🏛️ Architectural

[Practical tips on Software Architecture Design](https://medium.com/@mbue/practical-tips-on-software-architecture-design-part-one-1c6bb0167157)

* [Marco Bürckel ](https://twitter.com/mbue86) gives a good 101 on how to architect a system, starting with what to do before you pick a software deign pattern, through to functional and non-functional requirements and iteration.

[Understanding software design patterns](https://opensource.com/article/19/7/understanding-software-design-patterns)

* [Bryant Son](https://twitter.com/bryantjiminson) provides detailed diagrams explaining different software patterns, including (1) Singleton (2) Factory (3) Observer, with code examples for each.

[Software Architecture Patterns](https://www.oreilly.com/library/view/software-architecture-patterns/9781491971437/)

* [Mark Richards'](https://twitter.com/markrichardssa) book, fully available for free, gives an overview of (1) layered architecture (2) event-driven architecture (3) microkernel architecture (4) microservices architecture (5) space-based architecture.
* Within each section, there is a run through of the circumstances that are appropriate for each architectural type.

### 🎨 Design

[What is design debt?](https://uxdesign.cc/what-is-design-debt-and-why-you-should-treat-it-seriously-4366d33d3c89)
* An extensive run through by [Michal Mazur](https://twitter.com/mazi_mazur), from his experiences at Kurt Geiger, where they had people drop out of the funnel because of inconsistent design.

[Marginal Brand Degredation](https://markboulton.co.uk/journal/marginal-degredation/)
* Just 1.6% is the difference in DNA between a gorilla and a human. [Mark Boulton](https://twitter.com/markboulton) uses a powerful analogy to explain the importance of marginal brand degradation.

[Design Systems](https://github.com/alexpate/awesome-design-systems)
* An enormous set of example design systems collated by [Alex Pate](https://twitter.com/alexjpate)
* Covers components, voice and tone, designers kit and source code availability.

[Primer Interface Guidelines](https://github.com/primer/design)
* Repository to generate documentation for UI patterns and interaction guidelines.

### 💻 Code
[SOLID Principles of Object Oriented and Agile Design](https://www.youtube.com/watch?v=TMuno5RZNeE)

* Bob Martin ('Uncle Bob') explains software design principles.
* This covers the principles of: Single Repository, Open Closed, Liskov Substitution, Interface Segregation, Dependency Inversion

### ✅ Testing
[Test Driven Development](https://www.eecs.yorku.ca/course_archive/2003-04/W/3311/sectionM/case_studies/money/KentBeck_TDD_byexample.pdf)

* [Kent Beck](https://twitter.com/KentBeck) came up with the concept of Test Driven Development (TDD)
* Test Driven Development is defined by writing tests before writing any functionality.

### 🛠️ Build
[Continuous Integration](https://martinfowler.com/articles/continuousIntegration.html)

* [Martin Fowler](https://twitter.com/martinfowler)'s overview explains how Continuous Integration - where members of a team integrate their work frequently, usually daily by each developer - can ensure the codebase is more coherent and bugs are easier to find.
* The article covers the practices, but also the benefits and how to introduce Continuous Integration into the way a team works.

[Continuous Delivery - a systemic review of approaches](https://ieeexplore.ieee.org/document/7884954)

* This paper represents a state of the art, based on peer-reviewed papers from 2004 to 2016, by [Mojtaba Shahin](https://twitter.com/mojtabashahin), [Ali Babar](https://twitter.com/alibabar?lang=en), and [Liming Zhu](https://twitter.com/limingz).
* The paper identifies 30 approaches and associated tools, including succesful applications to both greenfield and existing codebases, with the issues and opportunities that continuous practices summarised.

### 📝 Documentation
[Real life examples of great documentation](https://www.atlassian.com/blog/add-ons/5-real-life-examples-beautiful-technical-documentation)

* [Katrina Morales](https://twitter.com/katrinahmorales) gives examples covering (1) providing answers fast (2) creating community through comments (3) great navigation (4) design (5) rich content.

[Extreme Programming Documentation](https://ronjeffries.com/xprog/articles/expdocumentationinxp/)

* [Ron Jeffries](https://twitter.com/RonJeffries), one of the three founders of Extreme Programming, covers the documentation of (1) requirements (2) design (3) code (4) manuals.

[The Eight Rules of Good Documentation](https://www.oreilly.com/ideas/the-eight-rules-of-good-documentation)

* This excerpt from [Adam Scott](https://twitter.com/adamdscott)'s '[Collaborative Web Development](https://www.safaribooksonline.com/library/view/collaborative-web-development/9781491996096/?_ga=2.191768554.1140860929.1571121117-2134570287.1570721867)' book, walks through not the "what" of documentation, but the "how".

### 🏚️ Versioning
[Version control best practices](https://www.git-tower.com/blog/version-control-best-practices/)

* A simple set of rules from [Tobias Günther](https://twitter.com/gntr), the founder of Tower (a Git client) hat will help make sure the whole team can work with the commits that each developer makes.

[Writing good commit messages](https://chris.beams.io/posts/git-commit/)

* You will default into messy commit messages. [Chris Beams](https://twitter.com/cbeams) shows what good looks like.

## 🏥 Remediation

### 🔍 Post Mortems

[PagerDuty Toolbox]([https://postmortems.pagerduty.com](https://postmortems.pagerduty.com/))

* PagerDuty have put together a completely all encompassing set of templates and an approach to the Post Mortem.

[Language to use, understanding causation, and how to share](https://fractio.nl/2015/10/30/blame-language-sharing/)

* [Lindsay Holmwood](https://twitter.com/auxesis) discusses how a thoughtful approach to learning from failure is key.
* When to use "how" versus "what" versus "why".
* Confirmation and hindsight bias.
* Creating a safe culture to discuss failure.

### 💣 High Interest Debt First

['State of the Art - research summary'](https://arxiv.org/pdf/1904.12538.pdf)

* 38 research papers summarised found there isn't a distinct "best practice" that has become clear yet.
* Code and architecture are by far the two most focussed on areas, yet there are many more forms of debt (requirements, and tests, for example).

### 🧭 Boy Scout Rule
[The Boy Scout Rule explained](https://dev.to/_arunsasi/the-boy-scout-rule)

* [Arun Sasidharan](https://twitter.com/voidmaindev) creates a great explanation of Bob Martin's rule.
* The premise is to create a culture of leaving the code in a better state than when you started.

### 🧰 Tools
* Continuous tracking of Tech Debt based on merges: [Hiberly](https://hiberly.com)
* Code coverage, Cyclomatic complexity: [Sonarqube](http://www.sonarqube.org/)
* Time to Interact: [Yottaa](http://www.yottaa.com/)
* Application security: [Veracode](http://www.veracode.com/)
* Infrastructure performance: [Splunk](http://www.splunk.com/)
* Scalability: [SOASTA](http://www.soasta.com/)

## Contributing

Please read [CONTRIBUTING.md](/CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.


## Authors

* **James Hawkins** - *Initial work* - [jamesefhawkins](https://github.com/jamesefhawkins)
* **Tim Glaser** - *Editing* - [timgl](https://github.com/timgl)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

## Sponsors

[<img src="https://s3-eu-west-2.amazonaws.com/hiberly-wordpress/wp-content/uploads/2019/07/31001245/small-logo-whiteback-blockdots-blacktext-1-e1564532005680.png" alt="Hiberly Logo" width="100"/>](https://hiberly.com?utm_campaign=os&utm_medium=techdebtreadinglist&utm_source=sponsorship)

Hiberly prioritizes tech debt by grabbing feedback from developers after each merge.

You can then draw cool graphs of your code versus happiness / frustration to help explain the impact of refactoring.