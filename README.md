# DevOps-Project

-	"Show and Tell"
-	Used two repositories: **DevOps-Project** (this) and **Google-Cloud-Run-Git-Hub-Actions** (https://github.com/SarahKhiu/Google-Cloud-Run-Git-Hub-Actions#:~:text=SarahKhiu,Git-Hub-Actions)
- **Thought Processes and Learnings** file is appended in the repository

## Create a Customisd GitHub Action
Using node and JavaScript to add a new comment, "Thank you!" to the person who creates a pull request in the repository, along with a GIF from the Tenor API to make it a little fun.

**Application code inside [action.yml] file:**

![Screenshot (64)](https://user-images.githubusercontent.com/89820671/136189422-31f43e13-f11f-426a-a883-c67f2c3931e8.png)

Code source: https://www.youtube.com/watch?v=Ef0gPGUh9oo&t=780s
## Notes (a reminder to self):
- **Difference between actions and workflows on GitHub:**
***“Actions”*** are individual tasks that can be combined to create jobs and customize workflow. ***“Workflows”*** are custom ‘automated’ processes that you set up in your repository to build, test, package, release or deploy any project on GitHub.
- **Workflows:** automated process, defined in yaml files stored in workflows directory. Consist of event, machine, job and steps. Many actions make up a workflow.
- **Basic syntax for a workflow is:**
   - *on*: the event that triggers the workflow
   - *runs-on*: the machine each job should run
   - *jobs*: the jobs that make the workflow
   - *steps*: the tasks each job should run
   - *run*: the command the step should run
   
- **Elements of a CI/CD pipeline:**

![ci-cd_pipeline](https://user-images.githubusercontent.com/89820671/136138509-d0f453b7-b538-4371-bdd5-7cd5882f5550.png)

1. **Build** - where the application is compiled.
2. **Test** - where code is tested. Automation here can save both time and effort.
3. **Release** - where the application is delivered to the repository.
4. **Deploy** - where code is deployed to production.
5. **Validation and Compliance** - Steps to validate a build are determined by the needs of your organization. Image security scanning tools can ensure the quality of images by comparing them to Common Vulnerabilities and Exposures (CVEs).

