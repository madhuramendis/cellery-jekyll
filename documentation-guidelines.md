Documentation Guidelines
========================
This document describes how to create documentation for your contributions to WSO2 products. It contains the following sections:

- [Documenting a new feature](#documenting-a-new-feature)
- [Documenting a REST API](#documenting-a-rest-api)
- [Documenting a sample](#documenting-a-sample)
- [Guidelines for writing great documentation](#guidelines-for-writing-great-documentation)
 
Documenting a new feature
-------------------------
When you contribute a feature to WSO2 products, you must include a feature document that fully describes the feature, how it’s used, the problems it solves, etc. The feature document should contain high-quality content that can be used as the foundation for the product documentation, marketing content, and training materials with minimal editing. For a list of resources to help you write the best possible content, see [Guidelines for writing great documentation](#guidelines-for-writing-great-documentation).

The document should be in Markdown format and accompany your pull request. Following is a template for this feature document and what each section should include. 

### Description

The introduction is your 30-second elevator pitch for your feature. Write a brief paragraph or two that summarizes the purpose and function of this feature. Start with a one- or two-sentence summary of what the feature does and/or what problem it solves. 

You can give more descriptive information in a second paragraph. This paragraph should answer the questions: "What does this feature *do*?" and "*Why* would I use it?" If your feature has a range of functionality (installation, configuration, management, etc.), you can briefly mention them here and go into detail later in the subsequent sections.

### Usage
Explain the user stories/scenarios that the feature applies to. 

### Impact on installation
* Files, packages, services, or operations that the feature will alter, impact, or execute.
* Dependencies that your feature automatically installs.
* Warnings or other important notices.

### Upgrading
If your most recent release breaks compatibility or requires particular steps for upgrading, describe the required steps here.

### Setup requirements
Specify the required environment (e.g., JDK, OS, and database versions that have been successfully tested). If your feature requires anything extra before setting up (another feature, etc.), mention it here. 

### Configuration
Use this section to list special notes about the configuration of this feature, including but not limited to permissions. The configuration section is necessary even when little configuration is required. 

Explicitly explain the following: 
How enabling/disabling the feature will affect the product UI vs. file-based configuration, where the config actions are stored, and how a restart would affect it (which configs require a restart and which do not). 

### Example
Show what the feature does as concisely as possible. Users should be able to figure out how your feature solves their problem by looking at the example. Make sure the functionality you are showing off is obvious that your code/configuration is short and concise, and that any related APIs, configurations, data types, and other elements are included or mentioned. 

### Tutorial/training lab
Create a tutorial that the user can use to learn how to use the feature to solve business problems. Specify an objective, introduce the business problem/scenario, summarize how you’ll solve it with this feature, and then provide complete steps the user must follow to complete the tutorial. Include sample files such as back-end services as needed. 
Reference
Users need a complete list of your feature’s APIs, configurations, and data types, along with the parameters for each. 

For all parameters used in APIs and configurations, each element should include:

  * The data type, if applicable.
  * A description of what the parameter/element does
  * Valid values, if the data type doesn't make it obvious.
  * Default value, if any.

### API reference
Provide a complete list of APIs related to the feature.

### Configuration reference
Provide a complete list of configurations related to the feature

### Limitations
Describe infrastructure compatibility, version compatibility, etc. If there are known issues, include them under their own heading here.

### Best practices
Highlight the best practices for using this feature. For example, if you can configure it in two different ways, specify when you would choose one way over the other. 

### Tests
Describe and show how to run the tests to ensure that the feature works right from the user’s perspective. This is not about functional or unit testing. This is more about user acceptance testing (UAT). Think how would the user verify that the feature works the way it should. 

### Troubleshooting & FAQs
Address questions that are likely to be asked frequently by users. Outline common problems that users would encounter along with solutions. Explain how the users may get to the root of the problem through troubleshooting. A list of error codes resulting from the feature, problem logs with causes, and an exception table would help here. 

Documenting a REST API
----------------------
If you are adding a REST API to a WSO2 product, include a markdown file that covers the following information:

- Introduction to the API. Should explain what the API does.
- Parameters of the API. Should cover each parameter’s name, description, datatype, and default and fixed values (if any).
- Request format.
- Response format.
- Sample request. For example, the Curl command.

Documenting a sample
--------------------
When you add a sample to any WSO2 product, include a readme.md file that uses the following template. 

### Title
Use a meaningful name for the title of the sample so that the business use case addressed in the sample is clear. The title should also contain possible search terms.

For example: 
Poor title: Excel Sample
Good title: Service Enabling the Data in an Excel Sheet

### Introduction
Explain the following as applicable:

- The objective of the sample and the use case it demonstrates.
- The technical concepts, or if the concept is already explained in the documentation, link to the relevant pages. Otherwise, provide an appropriate external reference. For example, when a sample demonstrates the usage of MTOM capability, explain or provide reference to what ‘MTOM’ is.
- Assumptions you are making. One possible assumption is that the user knows certain industry standards and well-known technical concepts. We can state them here so that users are aware of what they are expected to know to follow the sample. 

### Prerequisites
- Additional software and databases required to run the sample, and how to download, install, and configure them. If already explained, link to the current doc or external sources.
- Any packages or files (such as .jar files) to be installed and URLs to change.
- Any existing config files that need to be changed and how.

Wherever possible and appropriate, explain why the user needs each prerequisite. We want the users to understand the context of what they are doing along the way.

### Building the sample
Describe the aample file location and how to build the sample. (E.g., using Ant).

### Executing the sample
Give step-by-step instructions to execute the sample and view results. This section may include:

- Sub-titles and diagrams as appropriate.
- Configuration files and code blocks.
- Management Console screenshots.
- How to run any sample clients.
- How to view results and screenshots of results.

Wherever possible and appropriate, explain why they are taking the current step and what the results indicate. We want users to understand the context.

### Conclusion/analysis of results
Analyze the results and derive conclusions.

Guidelines for writing great documentation
------------------------------------------
The following resources help you understand the standard conventions and best practices for writing technical documentation. These guidelines will help ensure that the feature document you submit is clear, accurate, easy to understand, and requires minimal editing before the content is used in the product documentation, marketing content, and training materials. 

### Fundamentals of technical writing

- [A Beginner's Guide to Writing
   Documentation](http://www.writethedocs.org/guide/writing/beginners-guide-to-docs/)
-  [Documentation
   Principles](http://www.writethedocs.org/guide/writing/docs-principles/)
- [Essentials of Technical
   Writing](http://jacquelynwheeler.blogspot.com/2017/07/essentials-of-technical-writing.html)
- [Creating Better
   Documentation](https://www.techrepublic.com/blog/10-things/10-things-you-can-do-to-create-better-documentation/)
- [Writing for an International Audience](https://wiki.ubuntu.com/DocumentationTeam/StyleGuide/InternationalAudience) 

### Writing mechanics
- [Spelling, Punctuation, and Grammar](https://wiki.ubuntu.com/DocumentationTeam/StyleGuide/SpellingPunctuationGrammar) 
- Using Commas: [Part One](http://jacquelynwheeler.blogspot.com/2017/06/using-commas-part-one.html) and [Part Two](http://jacquelynwheeler.blogspot.com/2017/06/using-commas-part-two.html)
- [Hyphens and Dashes](http://jacquelynwheeler.blogspot.com/2017/07/hyphens-and-dashes.html)
- [Commonly Confused Words](https://wiki.ubuntu.com/DocumentationTeam/StyleGuide/CommonlyConfusedWords) 

### Writing tools
[StackEdit](https://stackedit.io/) is an in-browser editor for creating Markdown files. It allows you to save the file in Google Drive so you can collaborate, add comments, and publish directly to Github.

[Grammarly](https://www.grammarly.com/) is an in-browser grammar/spelling checker that helps you spot errors as you type. 
