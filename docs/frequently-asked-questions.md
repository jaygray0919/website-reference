# *Frequently Asked Questions* (FAQ)

###### last edit: 23-01-12

## Dialog: Anant and Jay

### AS-IS

> Anant@StripeSys:
>> Do you have any existing CI/CD Pipeline? If yes, where is it configured and how? CI/CD tools involved?

>> How many environments do you have currently?

>> Current deployment strategy?

> JG
>> We build and docker 10 instances of Python/MySQL apps on three AWS/EC2 servers

>> We build a Sphinx/Python instance from a GitHub repo and deploy simultaneously on ReadTheDocs and an AWS/EC2 server

### Project objectives: from a single GitHub repository, generate separate sites for 6 companies that are part of a single Consortium.

> Anant@StripeSys:
>> Do you have a clear demarcation of the six sites in terms of the codebase?

>> Please, provide the exact paths of the six sites in question.

>> Do they share anything in common or are completely separate/distinct and can be deployed, independently?

> JG
>> //afdsi.org

>> //ontomatica.io

>> //dailyfood.io

>> //dailycare.io

>> //electronic-label.io

>> //export-import-data.io

### Project status: Seeking a Developer with skills to solve specific problems; help to enable fully automated generation of Consortium sites.

> Anant@StripeSys:
>> What do you mean by automated generation of sites? Are you referring to the build process of the six sites on "push commits"?

> JG
>> Correct: push commits

>> We need to incrementally update a site after making changes to the shared repo

### CI/CD tools summary: Pipeline includes 60+ tools ranging from acorn to websockets

> Anant@StripeSys:
>> Would you be able to provide a short summary of tools with their exact function/purpose?

>> Which CI/CD tool has been used to host the pipelines?

>> Jenkins/TC/Travis/Azure DevOps/AWS CodeBuild?

>> Any artifactory in use?

### Core technologies: Grow is the static site generator

> Anant@StripeSys:
>> Is this supposed to be integrated into the pipeline for the automation purpose?

> JG
>> Correct. Grow is like all other static site generators.

>> Grow provides an open/close structure that contains substitution commands.

>> The substitution commands load libraries in \<head\> and content in \<body\>.

>> The substitution commands are very similar to Handlebars and Mustache.

>> Grow is designed to support sites with a large number of pages.

>> Grow also supports Natural Languages (NLs).

>> In the final state (sometime in the future) all sites will be delivered in 14 NLs.

>> The “RDF in 50 Words Or Less” example illustrates how we plan to do this.

- using Jinja templates: https://jinja.palletsprojects.com/en/3.0.x/

> Anant@StripeSys:
>> What are the expectations around this?

> JG
>> The templates used by Grow are Jinja templates

>> These are nearly identical to templates used by other static site generators.

>> The CI/CD pipeline also invokes node.js processes for server-side action such as search integration, page optimization and page compression.

> Anant@StripeSys:
>> What is CI/CD pipeline supposed to do after invoking the above mentioned actions?

> JG
>> node.js commands bind an action or perform a job.

>> Example: when a finished HTML page is generated, a node.js function triggers an optimizer that injects optimization routines into the page.

>> Another node.js function minimizes the HTML page.

>> Another node.js function uses Brotl to compress the page.

### Project tasks:

#### Use automation to document and visualize the pipeline.

> Anant@StripeSys:
>> What do you exactly mean by documenting and visualising the pipeline?

>> Are you referring to the visualisation of builds, build logs, UT, CC or something else? Need clarity on this.

> JG
>> In the past CircleCI provided visualization

>> More recently GitHub has implemented CircleCI-like visualization that seem to be “good enough”

>> Example: https://github.com/ampproject/amp.dev/runs/4615877272?check_suite_focus=true#step:10:11

#### Ensure that CI/CD works for both Apple/Mac/Homebrew and Windows/WSL and that test pages can be previewed on Apple/Mac or Windows.

> Anant@StripeSys:
>> Is the build/artifact supposed to work on Mac machines? If yes, then MAC agents would be required? Where are you exactly testing the Mac builds - Macbooks or Mac server?

> JG
>> Currently we can build and preview locally on a MacBook using Homebrew.

>> We also can build an AWS/EC2 instance.

>> We have not been able to build locally using Windows/WSL and Ubuntu.

>> We are experimenting with a Debian distro for WSL.

>> The Debian distro should work.

#### Where possible and appropriate, simplify the pipeline.

> Anant@StripeSys:
>> Any specified instruction/expectation around this?

> JG
>> Our thought is that a 3rd party, such as your organization, would see opportunities that we do not.

>> '#3' is saying to our CI/CD partner: “we’re willing to change this process if there is a better way”

#### We will generate pages for 14 Natural Languages (one of the reasons for using Grow).

> Anant@StripeSys:
>> Is this something of development team's interest or Devops or both?

>> Will this play any role with the setting up and maintaining the CI/CD Pipelines?

>JG
>> NL support is vital to the project. Arguably there is no higher priority.

>> The test site is ontomatica.io following the RDF-in-50 example.

>> At the end state, every page will be coded in 14 NLs.
