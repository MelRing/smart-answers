# Smart Answers

> Smart answers are a great tool for content designers to present complex information in a quick and simple way. Defining what they are – decision trees? calculators? tools? is immaterial – what they do is provide a reusable technical framework to build a quick and simple answer to a complex question.

Read more in [Lisa Scott's GDS blog post](https://gds.blog.gov.uk/2012/02/16/smart-answers-are-smart/).

## Screenshots

![Student Finance Forms screenshot](./doc/assets/govuk-student-finance-forms.png)

## Live examples

* [Look up Meursing code](https://www.gov.uk/additional-commodity-code)
* [Maternity and paternity calculator for employers](https://www.gov.uk/maternity-paternity-calculator)
* [Towing: licence and age requirements](https://www.gov.uk/towing-rules)

## Nomenclature

* **Smart Answer**: The flow, questions and outcomes.

* **Landing page**: The page containing the "Start now" button that describes the Smart Answer.

* **Flow**: Ruby code describing the questions, outcomes and rules for navigating between them.

* **Question**: An individual question that's asked in order to help the user arrive at the answer to the overall flow question.

* **Outcome**: ERB template containing the answer(s) to the overall flow question, based on the user's responses to the individual questions.

* **Node**: Questions and Outcomes are Nodes.

## Technical documentation

This is a Ruby on Rails application that both contains and serves the Smart Answers stored in this repository. Smart Answers are presented to public users.

**NOTE.** This application doesn't use a database.

### Dependencies

* [alphagov/static](https://github.com/alphagov/static): provides static assets (JS/CSS) and the GOV.UK templates.

### Running the application

See [development using the GDS development virtual machine](developing-using-vm.md).

### Running the test suite

    $ bundle exec rake

## Table of Contents

* Types of Smart Answer
  * [Ruby](doc/smart-answer-flows.md)
* Process
  * [Archiving a Smart Answer](doc/archiving.md)
  * [Continuous integration](doc/continuous-integration.md)
  * [Deploying changes for Factcheck](doc/factcheck.md)
  * [Deploying](doc/deploying.md)
  * [Merging pull requests from the content team](doc/merging-content-prs.md)
* Development
  * Adding [content-ids](doc/content-ids.md) to Smart Answers.
  * [Developing using the VM](doc/developing-using-vm.md)
  * [Issues and Todo](https://github.com/alphagov/smart-answers/issues)
  * [Rubocop](doc/rubocop.md)
  * [Testing](doc/testing.md)
  * [Updating worldwide fixture data](doc/updating-worldwide-fixture-data.md)
* Debugging
  * [Viewing landing pages and outcomes as Govspeak](doc/viewing-templates-as-govspeak.md)
  * [Viewing state of a Smart Answer](doc/viewing-state.md)
  * [Visualising flows](doc/visualising-flows.md)
