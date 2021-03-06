# Homework Review Process

This write-up documents the homework review workflow that I use when reviewing homework submitted as GitHub pull requests for the JavaScript 2 and 3 modules, but I think it is applicable to the other HYF modules too.

> Recently, I have started to use the VSCode **GitHub Pull Request** extension to streamline the review workflow. With this extension you can quickly check out pull requests without having to individually clone and `npm install` each student's repository.

When I'm assigned to teach a module I set myself up to **Watch** ('Be notified of all conversations') the corresponding repository on the HYF GitHub organization account, so I get notified when Pull Requests come in and again when they are updated. (I generally **Unwatch** when done teaching.)

If there are still pull requests from a preceding class I close them so we can start with a blank slate.

When a new pull request comes in, then, if not done already, I add the GitHub label `homeworkN` (where `N` is 1, 2 or 3) and the label `to review` to the pull request.

I generally start my reviews on the Friday (in the JS modules we have set the deadline for the pull request on Thursday evening, although only a portion of the students will meet that deadline). I continue the reviews on Saturday, but anything coming in on a Saturday night or Sunday morning will not get a timely review.

I start by opening my local (cloned) version of the module's HYF repository, say **JavaScript3** in VSCode (make sure that you run `npm install` after cloning).

Then, for each pull request, starting from the bottom (oldest pull request) working up (newer pull requests) I follow these steps:

1. I click on the GitHub Pull Request icon in the VSCode task bar and expand the **All** option. As shown in the picture below, you will see a list of the most recent Pull Requests for this repository.

   ![all-Prs](assets/all-PRs.png)

   **Figure 1**: GitHub Pull Requests extension

2. I right-click on the pull request I want to review and select the **Checkout Pull Request** menu option. This will create a local branch in the local repository, e.g. `pr/veliataseven/273` as shown in the VSCode status bar here:

   ![vscode-status-bar](assets/vscode-status-bar.png)

   **Figure 2**: VSCode status bar

3. While the VSCode Github Pull Request extension allows local commenting on the pull request, I prefer to do so online, directly in GitHub. To open the pull request in GitHub I right-click again on the pull request in VSCode and select **Open Pull Request in GitHub**.

4. On the GitHub pull request page I assign myself as Assignee, and change the label `to review` to `review in progress`. This to ensure that fellow mentors helping out with reviews do not start on the same pull request. (Of course, I'm expecting fellow mentors to do the same).

5. I now switch to the regular code window in VSCode by clicking on the Explorer icon in the VSCode task bar and start my actual review.

   > If the student installed additional dependencies in `package.json` you will need to run `npm install` again. For the JavaScript modules this should not be necessary.

6. If there are any unit tests as part of the repository I run them and review the results.

7. I also run the code (in Node for a CLI app or in the browser with the console open for an HTML app) to ensure that it at least runs without run-time errors.

8. On GitHub I then go through the code and insert comments in the pull request. When making the first comment I select **Start a Review**, instead of making single comments. Note that for each single comment GitHub sends out an email notification to all repository watchers. It will only send out a single notification for a complete review.

9. Because the JavaScript modules lay the foundation for much of the rest of the curriculum, I tend to comment a lot:

   - Naming: avoid generic names such as `data`, `item`, `element` if more descriptive names are possible; use plurals for arrays and a corresponding singular for an element of that array; avoid cryptic or ambiguous abbreviations; verb-based names for functions, noun-based names for variables and parameters etc.
   - No nested named functions, pass all required data through the parameter list.
   - In general I try to bring across best practice programming style, and give the rationale for doing things in a particular way.

10. I point out fragments of code that do not work, or do not meet the requirements of the assignment. I expect students to follow-up on these comments before their pull request can be approved.

11. Sometimes I make recommendations on how things can be done better, more elegant, more efficient, etc. However I don't consider these showstoppers for approving the pull request.

    > Before suggesting a non-trivial coding alternative to students, I try it out by modifying the code in the current branch and running it. When I'm satisfied I copy the relevant code snippet in a comment on GitHub and discard the local changes using the VSCode **Discard Changes** option.

12. When done I select **Review changes** in the pull request, add an overall assessment in the comment box and either **Approve** or **Request changes**.

13. Finally, I remove the label `review in progress` and either add the label `reviewed` in case the pull request was approved, or `needs work` if I requested changes.
