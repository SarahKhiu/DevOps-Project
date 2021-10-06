# DevOps-Project
-	for Show and Tell

**Create a Customised GitHub Action:**
<br>
Using node and JavaScript to add a new comment, "Thank you!" to the person who creates a pull request in the repository, along with a GIF from the Tenor API to make it a little extra fun.

**Application code in action yml file:**
name: Thank You
on:
pull_request:
types: [opened]
jobs:
thanks:
runs-on: ubuntu-latest
steps:
-uses: colbyfayock/thank-you-action@master
 with:
 GITHUB_TOKEN: ${{secrets.GITHUB_TOKEN}}
 TENOR_TOKEN: ${{secrets.TENOR_TOKEN}}
<br>

**Notes, a reminder for myself:**
•	Difference between actions and workflows on GitHub:
- “Actions” are individual tasks that can be combined to create jobs and customize workflow.           
- “Workflows” are custom ‘automated’ processes that you set up in your repository to build, test, package, release or deploy any project on GitHub. 
<br>
• Workflows: automated process, defined in yaml files stored in workflows directory. Consist of event, machine, job and steps. Many actions make up a workflow.
<br>
• Basic syntax for a workflow is:
<br>
*on* — the event that triggers the workflow
<br>
*runs-on* — the machine each job should run
<br>
*jobs* — the jobs that make the workflow
<br>
*steps* —the tasks each job should run
<br>
*run* —the command the step should run
<br>
**Elements of a CI/CD pipeline:**
<br>
![image](https://user-images.githubusercontent.com/89820671/136135996-d09b99b1-5def-47ee-b2d7-79703712076e.png)
<br>
**Build** - where the application is compiled.
<br>
**Test** - where code is tested. Automation here can save both time and effort.
<br>
**Release** - where the application is delivered to the repository.
<br>
**Deploy** - where code is deployed to production.
<br>
**Validation and Compliance** - Steps to validate a build are determined by the needs of your organization. Image security scanning tools can ensure the quality of images by comparing them to Common Vulnerabilities and Exposures (CVEs).

