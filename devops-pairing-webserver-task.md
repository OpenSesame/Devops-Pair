DevOps Pairing Exercise
=======================

This exercise is limited to 30 minutes. Feel free to ask questions as you go.
You don't have to have all the answers, and we encourage you to look things up
as you need them. You may also ask the interviewer for information. Think of it
as pair-programming, where the interviewer will happily help with language
syntax or similar questions.

# Goal

Create a web server in AWS, and serve some static content to the Internet. At
the end of this exercise, anyone should be able to hit an IP address or URL and
see the content.

## Mandatory Task

You are required to provision and deploy a new service in AWS. It must:

* Be publicly accessible on port 80
* Serve static content (e.g. a `version.txt` file, or a string)

You may use your own AWS account, or one that OpenSesame provides.

Provision the server however you wish. Be prepared to justify your decision.

## Next Steps

If there is time remaining after the task is completed, implement one or more of
the following ideas. You may also come up with your own idea for a next step, as
long as you discuss it with the interviewer.

* "Dockerize" it: build the content server as a docker image, and deploy that
  docker image into a new service in AWS to host that server on the Internet.

* Deploy changes to the server architecture and/or the content served using a
  CI/CD pipeline. Justify the strategy you use (e.g. "Git Flow", "GitHub Flow").

* Provide a healthcheck script that can be run externally to periodically check
  if the server is up and serving the expected content.

* Write a README file that describes how to:
  * Run the server locally
  * Create a new deployment of the server
  * Run the healthcheck script
  * Anything else a new contributor might need to know about the service

* Make the service resilient in 2 availability zones.

* Use the healthcheck script to start the service if it is not running or unhealthy.

* Deploy the server architecture using an Infrastructure-as-Code solution, like `terraform`, or AWS CloudFormation.

# Questions

## What AWS account should I use?

You may set up a new free-tier AWS account tied to your email address.
Alternatively, the interviewer will have one available you can sign into to use.

## What scripting/programming languages can I use?

Any you like. We'll ask you to justify your decision. We use Bash, Python, Go
and JavaScript internally. Please pick something you're familiar with, as
you'll need to be able to discuss it.

## What will you be grading me on?

* Your understanding of relevant technologies
* How you approach problem-solving
* Architectural decisions and what different aspects of development you consider

## Will I have a chance to explain my choices?

Hopefully this will emerge as we pair and converse, but feel free to comment your code, or put explanations in documentation.
