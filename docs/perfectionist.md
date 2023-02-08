# Perfectionist: our cloud-based LQA Tool

**Perfectionist** is a cloud-based tool for measuring translation quality, post editing quality, and raw machine translation quality. 

With this service you can:
- Outsource LQA tasks to internal and third-party experts
- Keep track of reviewes in the LQA reports repository

The service is built in accordance with the most recent proceedings of ASTM International Committee F43 featuring an advanced analytic-holistic LQA methodology.

## Supported File Formats

You can review bilingual files of the following formats: 
- **XLS** (a sample is available on the requestor page)
- **XLIFF**




# User Account and Role

**Perfectionist** uses the same user accounts as the https://cloud.logrusglobal.com/ portal. 

A user will have one of two roles: **Requestor** or **Reviewer**.

## Requestor

A **Requestor** can create review jobs (at https://lqa.logrusglobal.com/requestor-room) by clicking the **New Job** button on the **Requestor tab**.

A **Requestor** can also choose a metric to use in the review: currently we have implemented two metrics, **MQM** and **LOGIPEM**. We intend to also implement the **Interpro** metric in the future.

When you create a LQA job as a **Requestor**, you need to assign a **Reviewer** by submitting their email. If there isn't a Cloud account for a submitted email, it is created with **Reviewer** rights automatically.

## Reviewer

After a job is created, the **Reviewer** is sent an email with the link to new LQA review task. 

As a **Reviewer**, if your account had just been generated, you will be promted to create a new password. Then, the **Review** table will be opened in the browser, with two columns: **Source** and **Target**.

You will be required to compare each of the **Source** and **Target** lines. If there is an error,you will need to highlight the erroreous text fragment.

A pop-up window will appear on screen when you highlight a fragment. There, you will be able to suggest a correct translation or enter a comment; but, most importantly, you will need to pick a **Category** and a degree of **Severity** for each error.

A **Reviewer** can mark several errors in each translation unit, and their selections may overlap.





# Downloading the LQA report

As the review process is finished, the **Reviewer** marks the job as complete. Then, the **Requestor** becomes able to see the results and to download an **XLS** scorecard with the results of the evaluation (according to the  metric selected).