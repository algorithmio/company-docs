---
description: >-
  This document outlines the standard lifecycle for software engineers at
  Algorithm, from receiving a task to completing a code merge. Adhering to this
  process ensures consistency, quality, and collabor
---

# Algorithm Engineering Workflow Lifecycle

### **Prerequisites**

Before beginning work, ensure the following are in place:

* You have access to **JIRA**.
* You have access to the **codebase** (usually via GitHub or your version control system).
* You have been assigned one or more **development tickets**.

### **Workflow Steps**

#### **1. Update Ticket Status**

When you begin working on a ticket:

* Change its status in JIRA from Todo to Dev In Progress.

#### **2. Create a Feature Branch**

* Create a new branch from the default branch (usually development).
* Use the following naming convention:

\<ticket-name>-\<short-title>

**Example:**

MAK-141-handle-ticket-expiration

#### **3. Commit and Test Frequently**

* Make regular, meaningful commits as you progress.
* When the feature is complete:
  * **Thoroughly test** the feature for functional correctness.
  * **Smoke test** the entire application to ensure your changes don’t break existing functionality.
  * This is especially important since we serve **production clients**.

#### **4. Create a Pull Request (PR)**

* Push your feature branch to the remote repository.
* Create a PR targeting the default branch (e.g., development).
* Use the **same name for the PR** as the branch name.
* Follow the [Pull Request Standards.docx](https://algorithmio-my.sharepoint.com/:w:/g/personal/umair_thealgorithm_io/Eed5m8ZSeb1CuAHUYcgTJiIBydAoktRJrYjWnKE40fWIHw?e=PWUqe1) when writing your pull request description.

#### **5. Request a Review**

* Change the ticket status in JIRA to Ready to Review.
* Notify your team by posting in the **relevant project channel**:

"My PR(s) are ready for review."

This ensures team leads and reviewers are aware and can begin their review process promptly.

#### **6. Handling Code Review Feedback**

If the reviewer requests changes:

* Change the ticket status in JIRA **back to Dev In Progress**.
* Make the necessary updates and **push your changes to the same branch**.
* Once the feedback is addressed, update the ticket status to **Ready to Review** again.
* Notify the team in the project channel that the PR has been updated and is ready for another review.
