# Tech Debt - Prevention, Diagnosis and Cure

A tech debt reading and resources list - to help diagnose, prevent and control tech debt.

We created this project as we felt that it is almost an inevitability that some level of "tech debt" is encountered in every company, and many projects. The reason being that to get a feature out, it needs shaping and that involves - rationally - taking shortcuts.

## Start here

[What is tech debt](https://www.youtube.com/watch?v=pqeJFYwnkjE)

* Ward Cunningham created the term in the first place.
* History, motivation and common misunderstanding of the "debt metaphor" for refactoring.

[Classifying Technical Debt](https://martinfowler.com/bliki/TechnicalDebtQuadrant.html)

* Martin Fowler makes two disctions (1) prudent and reckless debt, and (2) deliberate and inadvertent debt, this is known as the TechnicalDebtQuadrant.

[Identifying when Technical Debt needs action](https://blog.crisp.se/2013/10/11/henrikkniberg/good-and-bad-technical-debt)

* [Henrik Kniberg](https://twitter.com/henrikkniberg) argues that older tech debt is bad, whereas new tech debt is acceptable in order to build prototypes.
* Concept of a qualitative debt ceiling technique to manage the level of technical debt.

[The Human Cost of Technical Debt?](https://daedtech.com/human-cost-tech-debt/)

* Erik Dietrick goes into depth for how technical debt can harm teams.
* There includes discussion on (1) unpleasant work (2) team infighting (3) atrophied skills (4) turnover and attrition

## Case Studies

[A large bank](http://neopragma.com/index.php/2019/03/30/technical-debt-the-man-the-metaphor-the-message/)

* [Dave Nicollete](https://twitter.com/davenicolette) covers a detailed case study, with costs, of resolving prudent-intentional debt.
* Costs of the cleanup and the business impact included.

[Ticketmaster](https://tech.ticketmaster.com/2015/06/30/what-ticketmaster-is-doing-about-technical-debt/)

* Step-by-step guidance on how Ticketmaster assessed their technical debt over 12 months.

[Stripe](https://www.infoq.com/presentations/stripe-technical-debt/)

* [Will Larson](https://twitter.com/lethain?lang=en) explains how Stripe use migrations to get away from tech debt

## Prevention

### Requirements

[Creating a Product Canvas](https://www.ebgconsulting.com/blog/using-product-canvas-define-product-getting-started/)

* 

[Story Mapping](https://www.jpattonassociates.com/the-new-backlog/)

* [Jeff Patton](https://twitter.com/jeffpatton) invented the concept of Story Mapping (you can see a [video of this process](https://www.youtube.com/watch?v=XzaCaW8c3qE) here) 
* Flat product story backlogs are hard to understand - they are just a pile of features. By visualising an entire system with it can be much easier to spot opportunities or weaknesses, or indeed to work with other stakeholders in requirements gathering.
* Create a series of cards with big stories (activities) at the top, down to tasks and then sub tasks.

[Agile Product Management](http://burozeven.nl/robbinschuurman/2017/11/14/10-tips-for-product-owners-on-agile-product-management/)

* 

[Joint Application Design](https://www.pmi.org/learning/library/determining-project-requirements-best-practices-7278)

* This is a thorough run-through by the Project Management Institute for Joint Application Design, designed for multi-stakeholder situations.

### Infrastructure

[DevOps 101](https://opensource.com/article/19/4/devops-pipeline)

* [Bryant Son's](https://twitter.com/bryantjiminson) simple guide that guides you through the basic setup to enable you to build you first pipeline
* Covers (1) CI/CD Tools (2) source control management (3) build automation (4) web app servers (5) code testing coverage

[Continuous Integration](https://martinfowler.com/articles/continuousIntegration.html)

* Continuous integration makes it easier to build cohesive software more rapidly. It involves every team member integrating their work frequently - normally, daily.
* It makes bugs show up more quickly because there are fewer areas where they could be lurking (ie diff-debugging is possible)

### Architectural

http://www.exa.unicen.edu.ar/escuelapav/cursos/slidesclements.pdf
https://www.oreilly.com/library/view/software-architecture-patterns/9781491971437/

### Design
Todo
### Code
Todo
### Testing
Todo
### Build
Todo
### Documentation
Todo
### Versioning
Todo

## Remediation

### Post Mortems

[PagerDuty Toolbox]([https://postmortems.pagerduty.com](https://postmortems.pagerduty.com/))

* PagerDuty have put together a completely all encompassing set of templates and an approach to the Post Mortem.

[Language to use, understanding causation, and how to share](https://fractio.nl/2015/10/30/blame-language-sharing/)

* [Lindsay Holmwood](https://twitter.com/auxesis) discusses how a thoughtful approach to learning from failure is key.
* When to use "how" versus "what" versus "why".
* Confirmation and hindsight bias.
* Creating a safe culture to discuss failure.

### High Interest Debt First

['State of the Art - research summary'](https://arxiv.org/pdf/1904.12538.pdf)

* 38 research papers summarised found there isn't a distinct "best practice" that has become clear yet.
* Code and architecture are by far the two most focussed on areas, yet there are many more forms of debt (requirements, and tests, for example).

### Boy Scout Rule
Todo

###Tools
Continuous tracking of Tech Debt based on merges: [Hiberly](https://hiberly.com)
Code coverage, Cyclomatic complexity: [Sonarqube](http://www.sonarqube.org/)
Time to Interact: [Yottaa](http://www.yottaa.com/)
Application security: [Veracode](http://www.veracode.com/)
Infrastructure performance: [Splunk](http://www.splunk.com/)
Scalability: [SOASTA](http://www.soasta.com/)

## Contributing

Please read [CONTRIBUTING.md](to follow!) for details on our code of conduct, and the process for submitting pull requests to us.


## Authors

* **James Hawkins** - *Initial work* - [jamesefhawkins](https://github.com/jamesefhawkins)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details