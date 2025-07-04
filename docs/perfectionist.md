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
- **XLIFF**, **XLF**, **MXLIFF**, **MQXLIFF** **SDLXLIFF**, **TSV**

# User Account and Role

**Perfectionist** uses the same user accounts as the https://cloud.logrusglobal.com/ portal. 

A user will have one of three roles: **Requestor**, **Reviewer** or **Stakeholder**.

## Requestor

A **Requestor** operates the **Requestor Room** page at https://lqa.logrusglobal.com/requestor-room. This user role has the capability of creating new LQA projects and new testing projects for evaluating personnel.

### Creating New Projects

This is done by using the **Create Project** button on the top right of the screen. 

![perf0](perfnew1.png)

This button calls a simple dialog window where you can name the new project.

![perf1](perfN1.png)

After you have named the new project, it will appear in the **Requestor Room**'s table of projects. Each line in the table represents a different project, lists its type and number of tasks (files) in in, as well as enables the **Reviewer** to download its results, delete it or rename the project.

Clicking on a name of a new project with zero tasks brings you to the **New Job** window, where you can set the project up with tasks. The sample.xlsx file is also available there.

Clicking the **Create** button calls up a special dialog box where you can drag and drop suitable bilingual files; you can also click on the box itself to call up a standard Explorer interface to look for the files you need.

![perf2](perfnew4.png)

Any duplicate translation units are excluded from the file when it is uploaded to **Perfectionist**. If you need to still include the duplicates, check the **Do not remove duplicates** box.

If a project has already had files assigned to it, clicking on its name in the list will take you to the project page, where each uploaded file is represented as a task. You can add more tasks with the **Create Task** button. Tasks can be deleted, renamed, or transfered to a different project by clicking the icons at the end of the task's line in the table.

![perf3](perfnew5.png)

You can also invite other users to be the the project's **Stakeholders** with the **Add User** button. It calls a simple dialog window where you can enter another user's email address to add them to the list of **Stakeholders**.

![perf4](perfN4.png)

You can enter the **Work Area** of a particular task by clicking its name in the list of tasks.

![perf3](perfnew6.png)

If you don't need the entire file reviewed, you can have a randomized sample created for reviewing. This is done in the **Sampling** screen, which you can access with the **Sampling** button. The size of the sample - either in **words**, or in **translation units** - can be set using the **Sample size** field and the adjacent drop-down menu; you can also set the sample to consist of either **random**, or **consecutive** translation units with the appropriate radio button. 

![perf3](perfnew7.png)

When the **Sample** button is clicked, **Perfectionist** will generate a randomized collection of translation units from the file, close in total wordcount to the **Sample size** value you have set, and display the results. You can then click either the **Confirm** button to have this task presented as the generated sample, or the **Don't sample request** button to cancel.

![perf3](perfnew8.png)

As a **Requestor**, you need to assign a **Reviewer** for each of the project's tasks by submitting their email. The dialog window to do that is called by clicking the **Assign** button in the bottom right of the **Work Area**. Optionally, you can also assign a **Translator** for the task.

![perf3](perfnew9.png)

If there isn't a **Cloud** account for a submitted email, it is created with **Reviewer** rights automatically.

You will need to choose a metric to use in the review. Currently, we have implemented the **LOGIPEM**, **MQM** and **Holistic** metrics. Any user-defined metrics can be implemented by request.

If a task has already been assigned to a **Reviewer**, upon clicking it in the list, you will see an area with two tabs: **Status** and **Results**.

![perf7](perfN7.png)

In the **Results** tab, you will be able to review the body of the task file, with all the errors the **Reviewer** had found marked in the text and summarized on top of the list using by-segment and by-wordcount diagrams.

![perf3](perfnew10.png)

From the **Status** tab, by clicking the **Review mistakes** button, you will be able to view each of the errors the **Reviewer** had found in detail, and comment on them as well as edit or delete them, or propose your own full translation for the **Fixed Target** field, if necessary. You can access the **Error Review** dialog window for interacting with an error by double-clicking on that error in the table.

![perf3](perfnew11.png)

![perf3](perfnew12.png)

When you consider the task to be complete, click on the **Finish Review** button on the bottom right.

### Creating Testing Projects

**Testing Projects** are employed to evaluate the capabilities of linguistic personnel using translation or editing tasks.

Clicking the **Create Testing Project** button calls the **New Testing Project** dialog. Here, you need to input the name of the project, choose one of the premade testing files and set **Translation** or **Editing** as the type of test that your linguist is to attend.

![perf11](perfN11.png)

Click on the project name, and then on the **Create** button to enter the email of the test attendee.

![perf12](perfN12.png)

Emails are not sent automatically. Links to testing tasks are available to the **Requestor**, and they are required to email/message them manually to the **Translator** which is to be tested. This is because such a **Translator**, at that time, only gets one-time access to the testing task; we don’t need them as a full user of our **Cloud** yet because we may never see them again. By the same token, the link to the testing project is only needed once, and for a limited period of time. We left it up to the **Requestor** to determine the best way to deliver the project link to the **Translator**, instead of using automatic emails.

If you've set the task to be a **Translation**, then the **Your Input** field in the task file will be empty, and the attendee will be required to fill it in. If you've set **Editing**, it will be filled with text for the attendee to edit.

![perf13](perfN13.png)

After the attendee had pressed the **Finish Task** button, the finished task is treated as if it is an LQA project. Clicking on the name of a finished task takes you to a **Work Area**, where you can assign it to a **Reviewer**, as described previously, to find out how the attendee handled their task.

![perf14](perfN14.png)

### Arbitrating

The **Requestor** sees a window with the **Status** and **Results** tabs upon opening a task:

![perf3](perfnew13.png)

The **Status** tab shows basic information about the task, with a button for switching to reviewing errors.

Below are the workflow buttons: the **Complete Task** button completes the task, and the **Assign Task** button enables either sending the task for review to a translator, and/or sending it for second review to a reviewer, or sending it to an arbiter. With the third option, you may start the arbitration cycle and design it as you wish. When sending a task for review, the same email is sent as when issuing an initial task.

The error reviewing screen looks much the same as a normal review, but without the ability to add new errors by highlighting text. You can click on an error that's already present, and a screen with data on it. The data can't be changed directly, but at the bottom there are the buttons to **Accept**, **Reject**, **Propose Edit**:

![perf3](perfnew14.png)

**Accept** marks the error as closed.

**Reject** requires a comment and marks the error as rejected.

**Propose Edit** enables you to edit the Category, Severity, Screenshot and Fixed Target fields. Adding a comment will be required:

![perf3](perfnew15.png)

The buttons may differ depending on the error status. For example, if the **Translator** selects **Reject**, then at the next stage of the review there will be a button to **Accept Rejection**, which will remove the error.

Arbiters have different buttons; they can simply change any fields and close the error.

Also on this screen there is the **View history** button for viewing the history of changes to the error:

![perf_arb_4](perf_arb_4_1.png)

### Analytics

The **Requestor** can access the **Analytics** page using the **Analytics** button. Here, you can filter out the list of accessible files using one or more of a wide variety of applicable filter conditions:

![perf_arb_4](perfnew2.png)

The **Analytics** window will display filtered results as a table:

![perf_arb_4](perfnew3.png)

Using the **Export** button, these results may be exported as an XLSX file.

## Reviewer

When a **Requestor** assigns an LQA task, an email with the link is sent to the **Reviewer**.

If there isn't a **Cloud** account connected with the assigned email address, it is created automatically with a prompt to create a new password.

![perf17](perfN17.png)

As a **Reviewer**, you operate the **Reviewer Room** page at https://lqa.logrusglobal.com/reviewer-room. There, you can see the list of tasks that have been assigned to you by **Requestors**.

![perf_arb_4](perfnew16.png)

The **Work Area** of a task can be opened by clicking its name in the **Reviewer Room**'s list. This page represents the task's file using the following columns: **Source**, **Target**, **Errors**, **Fixed Target** and **Reviewed**. The **Reviewed** checkbox is set automatically each time any translation error is logged in a given translation unit, or manually by the **Reviewer** after the unit has been fully reviewed. 

![perf15](perfN15.png)

You will be required to compare the **Source** and **Target** fields in each of the translation units. If there is an error, you will need to highlight the erroneous text fragment.

Highlighting any part of the **Target** field brings up the **Error Annotation, Suggestion and Comments** dialog window. There, you will need to set the **Category** and the degree of **Severity** of this particular error; optionally, you are also enabled to leave a comment or to offer your own variant of the full translated sentence for the **Fixed Target** field.

![perf16](perfN16.png)

Multiple errors may be marked in each translation unit, and their highlighted text fragments may overlap.

Having reviewed the entire file, you will need to mark the task as finished by clicking the **Finish Review** button. A dialog window with a text box for entering a general conclusion on the file will be called; the **Requestor** will be able to view that conclusion later.

![perf2](perf2.png)


## Stakeholder

As a **Stakeholder**, you operate the **Stakeholder Room** page at https://lqa.logrusglobal.com/stakeholder-room. There, you can see the list of projects which you have been invited to as a **Stakeholder** by the project's **Requestor**. Stakeholders supervise the performance of their company requestors and reviewers, monitor the overall translation quality level, and catch any pitfalls.

![perf19](perfN19.png)

You can go into a project's own page by clicking its name in the list. For **Stakeholders**, only the tasks that have already been assigned to **Reviewers** are visible on the project page.

![perf20](perfN20.png)

As a **Stakeholder**, you can view the in-progress task similarly to how the **Requestor** does it on the **Results** tab.

# Downloading the LQA report

While the review process is ongoing (or after it has been finished) in any given task, the **Requestor** as well as any invited **Stakeholders** may download the score card in the form of an **XLSX** file. This option is available in the form of the download symbol next to each assigned task in the project's list of tasks.

The **XLSX** file will be composed according to the metric chosen by the **Requestor** when assigning the task.