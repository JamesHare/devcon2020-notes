# Working with Cucumber

What is cucumber?
It is a bahavoir-driven development tool using Gherkin syntax. You can use it to record and test requirements. It is designed to be non-technical, human readable, and in the plain language of business. Cucumber requirements are broken into Features, which are comprised of one of more Scenarios.

Feature: describes what's going on, at a very high level.
Scenario: describes a more targeted, concrete business rule.
Given: provide context, set up prereqs.
WhenL an action or event
Then: the expected results

Each scenario tells a succinct, complete behavior.

Scenario Outline: Allows you to test multiple similar  ehabiors using variables.
Examples: a table of conditions
The Scenario Outline has turned one test into three.

Cucumber tags help group Scenarios and Feature files for reporting.

Downsides:

* Some requirements can't be tested with cucumber.
* No built in wyay to cross-reference or embed other requirements.
* Test data creation and cleanup loads to collisions and failed test runs.
* Tests run each time the code is built in Jenkins: More requirements means more tests and longer build time.