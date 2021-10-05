# DevOps-Project
-	for Show and Tell

**Create a Customised GitHub Action:**
<br>
Using node and JavaScript to add a new comment, "Thank you!" to the person who creates a pull request in the repository, along with a GIF from the Tenor API to make it a little extra fun.

Application code:
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

