# Style Stage WDD331R Assingment
The goal: To create a unique style stage webpage with the base css, adding our own unique style.
## IMPORTANT: Git branching
In order to keep the project organized, git branching is essential. Please create your own branch before writing any code. Name your branch after your name so that it is easy to see who has done what work.
#### Core Concepts:

* **`main` Branch:**
    * This is the primary branch.
    * It **MUST always** hold stable, deployable code.
    * **NEVER work directly on the `main` branch.** All development occurs on separate feature branches.
* **Feature Branches:**
    * These are temporary branches created for every new task, feature, or bug fix.
    * Branch them off `main`, perform your work, and then merge them back into `main`.

---

### Step-by-Step Instructions: Your Branching Workflow

Follow these instructions for each task you begin. Assume your main branch is named `main`.

#### **Step 1: Get Ready for a New Task (Pull the Latest `main`)**

Before you begin any new coding for a task, ensure your local `main` branch is perfectly up-to-date with the remote repository. This prevents you from building on old code.

* **Action:** Switch to the `main` branch.
    ```bash
    git checkout main
    ```
* **Action:** Pull the very latest changes from the remote `main` branch.
    ```bash
    git pull origin main
    ```
    *(**DO THIS** at the beginning of each day, or before starting any new task, to ensure your local `main` is current.)*

#### **Step 2: Create a New Feature Branch for Your Task**

Always create a new, dedicated branch specifically for the task you're about to work on. This isolates your work.

* **Action:** Choose a clear and descriptive name for your branch.
    * **Good Naming Conventions:** In this situation, use your name as the branch name so that we can stay organized.
* **Action:** Use this command to **create** your new branch and **switch** your working directory to it immediately.
    ```bash
    git checkout -b your-branch-name
    ```

#### **Step 3: Work on Your Task & Commit Frequently**

Now you are on your isolated feature branch. Make all your code changes, add new files, and modify existing ones here.

* **Action:** As you complete small, logical parts of your task (e.g., "added button UI," "implemented service function," "fixed a specific bug"), **commit your changes regularly**. Don't wait until the very end. Smaller commits are easier to review and debug.
* **Command:** Stage all your changes (new, modified, deleted files).
    ```bash
    git add .
    ```
* **Command:** Commit your staged changes with a clear, concise message describing what you did.
    ```bash
    git commit -m "descriptive message describing your changes"
    ```

* **Action:** **Push your feature branch to the remote repository often** (e.g., at the end of the day, after significant progress, or before taking a break). This backs up your work and makes it visible for teammates (and review).
    ```bash
    git push origin your-branch-name
    ```
    *(**Note:** The first time you push a new branch, Git might tell you to use `--set-upstream origin feature/your-task-name-here`. Copy and paste that exact command.)*

#### **Step 5: pull request and merge**
When you push your changes, it will often prompt you to open a pull request and merge your changes into main. If you feel confident with the changes you have done, feel free to do this. Make sure to properly resolve any merge requests that may exist. I find that making pull requests is easiest on the github website, but feel free to do it however you feel comfortable.

#### **Step 6: Syncing your branch with main**
For future work, you want to make sure that your branch is fully updated with the code in main. To do so, make sure to run these commands when you have your branch checked out:
* **Action:** Syncs your branch with the `main` branch.
    ```bash
    git pull origin main
    ```
There is probably more than one way to merge everything together, so do what you know best.