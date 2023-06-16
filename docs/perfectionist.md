# Perfectionist: a cloud-based LQA Tool

**Perfectionist** is a Web service for measuring translation quality, post editing quality, and raw machine translation quality. 

With this service you can:
- Outsource LQA tasks to internal and third-party experts
- Review random translation samples of given size
- Exclude repeated translation units from the scope of review
- Keep track of reviewes in the LQA reports repository
- Download LQA reports

For translation quality evaluation, you can choose from several embedded quality metrics:
- standard LQA metrics based on MQM error typology
- advanced LOGIPEM metrics for most adequate and precise quality evaluation of raw and post edited machine translation
- any user-defined metrics (by request)

The service is built in accordance with the most recent proceedings of ASTM International Committee F43 featuring an advanced analytic-holistic LQA methodology.

For enterprises, any customizations of the service functionality can be provided upon request.

## Supported File Formats

You can review bilingual files of the following formats: 
- **XLSX** (a sample is available on the requestor page)
- **XLIFF**, **XLF**, **SDLXLIFF**, **TSV**

# User Account and Role

**Perfectionist** uses the same user accounts as the https://cloud.logrusglobal.com/ portal. 

A user will have one of three roles: **Requestor**, **Reviewer** or **Stakeholder**.

## Requestor

A **Requestor** operates the **Requestor Room** page at https://lqa.logrusglobal.com/requestor-room. This user role has the capability of creating new LQA projects and new testing projects for evaluating personnel.

### Creating New Projects

This is done by using the **Create Project** button on the top right of the screen. 

![perf0](perfN0.png)

This button calls a simple dialog window where you can name the new project.

![perf1](perfN1.png)

After you have named the new project, it will appear in the **Requestor Room**'s table of projects. Each line in the table represents a different project, lists its type and number of tasks (files) in in, as well as enables the **Reviewer** to download its results or delete it.

Clicking on a name of a new project with zero tasks brings you to the **New Job** window, where you can set the project up with tasks. The sample.xlsx file is also available there.

Clicking the **Create** button calls up a special dialog box where you can drag and drop suitable bilingual files; you can also click on the box itself to call up a standard Explorer interface to look for the files you need.

![perf2](perfN2.png)

All repeated translation units are excluded from the file when uploading it to the service.

If a project has already had files assigned to it, clicking on its name in the list of project will take you to its project page, with a list of tasks assigned to it. You can assign more tasks with the **Create Task** button.

![perf3](perfN3.png)

You can also invite other users to be the the project's **Stakeholders** with the **Add User** button. It calls a simple dialog window where you can enter another user's email address to add them to the list of **Stakeholders**.

![perf4](perfN4.png)

You can enter the **Work Area** of a particular task by clicking its name in the list of tasks.

If you don't need the entire file reviewed, you can have a randomized sample created for reviewing. Its size can be set using the **Sample size** field above the table. After entering the desired sample size, click the **Resample randomly** button, and **Perfectionist** will generate a randomized collection of line pairs from the file, close in total wordcount to the **Sample size** value you have set.

![perf5](perfN5.png)

As a **Requestor**, you need to assign a **Reviewer** for each of the project's tasks by submitting their email. The dialog window to do that is called by clicking the **Assign** button in the bottom right of the **Work Area**.

![perf6](perfN6.png)

If there isn't a Cloud account for a submitted email, it is created with **Reviewer** rights automatically.

You will need to choose a metric to use in the review. Currently, we have implemented the **LOGIPEM**, **MQM** and **Holistic** metrics. Any user-defined metrics can be implemented by request.

If a task has already been assigned to a **Reviewer**, upon clicking it in the list, you will see an area with two tabs: **Status** and **Results**.

![perf6](perfN7.png)

In the **Results** tab, you will be able to review the body of the task file, with all the errors the **Reviewer** had found marked in the text and summarized on top of the list.

![perf7](perfN8.png)

From the **Status** tab, by clicking the **Review mistakes** button, you will be able to view each of the errors the **Reviewer** had found in detail, and then comment on them as well as edit or delete them, if necessary. You can access the dialog window for interacting with an error by clicking on that error in the table.

![perf8](perfN9.png)

![perf9](perfN10.png)

When you are ready to complete the task, click on the **Finish Review** button in the bottom left.

### Creating Testing Projects

**Testing Projects** are a feature that we've added to **Perfectionist** recently. They are employed to evaluate the capabilities of linguistic personnel using translation or editing tasks.

Clicking the **Create Testing Project** calls the dialog to input the name of the project, choose one of the premade testing files and set **Translation** or **Editing** as the type of testing that your linguist is to undergo.

![perf10](perfN11.png)

Click on the project name, and then on the **Create** button to enter the email of the test attendee.

![perf11](perfN12.png)

If you've set the task to be a **Translation**, then the **Target** field in the task file will be empty, and the attendee will be required to fill it in. If you've set **Editing**, it will be filled with text for the attendee to edit.

![perf12](perfN13.png)

After the attendee had pressed the **Finish Task** button, the finished task is treated as if it is an LQA project. Clicking on the name of a finished task takes you to a **Work Area**, where you can assign it to a **Reviewer**, as described previously, to find out how the attendee handled their task.

![perf13](perfN14.png)

## Reviewer

After the job is created, the email with the link to new LQA review task is sent to the assigned **Reviewer**. 

As a **Reviewer**, if your account had just been generated, you will be promted to create a new password. Then, the **Review** table will be opened in the browser, with the following columns: **Source**, **Target**, **Errors**, and **Reviewed**. The **Reviewed** checkbox is set automatically each time any translation error is logged in given translation unit, or manually when the unit is fully reviewed. 

![perf6](perf6.png)

You will be required to compare each of the **Source** and **Target** lines. If there is an error,you will need to highlight the erroneous text fragment.

A pop-up window will appear on screen when you highlight a fragment. There, you will be able to suggest a correct translation or enter a comment; but, most importantly, you will need to pick a **Category** and a degree of **Severity** for each error.

![perf1](perf1.png)

A **Reviewer** can mark several errors in each translation unit, and their selections may overlap.

Upon completion of the review, the task should be marked as completed using the **Finish Review** button. A pop-up window will appear for entering a general conclusion on the file, which will be available to the **Requestor**.

![perf2](perf2.png)


## Stakeholder

**Requestor** can assign the **Stakeholder** role to external users to view only the results of LQA tasks.

# Downloading the LQA report

As the review process is finished, the **Reviewer** marks the job as complete. Then, the results become available for **Requestor** to view and download as the **XLSX** scorecard with selected metrics.

![perf3](perf3.png)

