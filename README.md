# automated_refactoring
![image](https://github.com/srivhash/RefactorAI/assets/132872965/9649be84-0499-478a-9ead-fa0195b59235)
How to Use  
Follow the steps below to use the script/tool:  
1. Prerequisites  
GitHub Repository: Provide the URL of the GitHub repository you want to analyze.  
GitHub Token: Ensure you have a GitHub token with the necessary permissions.  
2. Configure Environment Variables  
Create these Secret variables in your repository
- ACCESS_TOKEN : GitHub token with repository access.
- GOOGLE_API_KEY : API key for the Generative AI service.

4. Workflow
 script.py
a) Created a yml file in .github/workflows folder This file defines the
workflow for automated refactoring.
b) Defined the workflow triggers in .yml file, such as on push events or on a scheduled basis an automated refactoring will be done for the repository specified in the python script . Used cron to achieve this.
 Bonus.py
a Create a New Branch -A new branch is created to make changes without
affecting the main branch.
b Detect and Fix Design Smells - The tool uses Generative AI to analyze Java files, detect design smells, and suggest refactoring.
Automated Refactoring  Team 17 2
c Commit and Push Changes - The script adds, commits, and pushes the refactored code to the new branch.
d Create a Pull Request - A pull request is generated with the refactored code. The user can review and merge the changes.
5. Output
The script provides a list of design smells detected in the codebase. A pull request is created with the refactored code.
Example
Let's use an example repository: https://github.com/yatharth- gupta/automated_refactoring
Output:
List of detected design smells. Pull request link.
Conclusion
This tool automates the process of identifying and fixing design smells, streamlining the code review and enhancement process. It empowers developers to maintain clean and maintainable codebases.
