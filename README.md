#  MLCoE GitHub Intro Task — Trainee Onboarding

Welcome to **MLCoE**! This intro task is designed to help you practice the complete **Git & GitHub collaboration workflow** that you'll use throughout your time here — forking, branching, committing, and raising Pull Requests (PRs) the professional way.

Follow this guide carefully and complete each step in order.

---

##  Objective

Every trainee will:
1. Fork the MLCoE repository
2. Create their own folder with a personal introduction
3. Raise a Pull Request to merge their work into the original repository

This simulates a real-world open-source / team contribution workflow.

---

##  Complete Workflow Overview

    Fork → Clone → Create Branch → Create Folder → Create README →
    git status → git diff → git add → git commit → git push →
    Pull Request → Review → Merge

---

##  Step-by-Step Instructions

### 1 Fork the Repository

Go to the original MLCoE repository on GitHub and click the **Fork** button (top-right corner). This creates a copy of the repository under your own GitHub account.

---

### 2 Clone Your Fork Locally

Clone **your fork** (not the original repo) to your local machine:

    git clone https://github.com/<your-username>/<repo-name>.git
    cd <repo-name>

---

### 3 Create Your Own Branch

Never work directly on `main`. Create a new branch using your name:

    git checkout -b Your-Name

**Example:**

    git checkout -b Aman-Verma

---

### 4 Create Your Folder

Inside the **root** of the repository, create a folder with your name.

>  Do **NOT** create a `Trainees/` folder or any parent folder. Your folder must sit directly in the root.

    mkdir Your-Name

**Example:**

    mkdir Aman-Verma

---

### 5 Create Your README.md

Inside your folder, create a `README.md` file:

    cd Your-Name
    touch README.md

Add your personal introduction (see template below), then return to the repository root:

    cd ..

---

### 6 Check Your Changes

Before staging anything, review what you've changed:

    git status

See the exact content changes:

    git diff

---

### 7 Stage Your Changes

    git add Your-Name/README.md

Or, to stage all changes in the repo:

    git add .

---

### 8 Commit Your Changes

Write a clear, meaningful commit message:

    git commit -m "Add introduction README for Your-Name"

**Example:**

    git commit -m "Add introduction README for Aman Verma"

---

### 9 Push Your Branch

Push your branch to **your fork** (not the original repo):

    git push origin Your-Name

**Example:**

    git push origin Aman-Verma

---

### 10 Create a Pull Request

1. Go to your fork on GitHub.
2. You'll see a prompt: **"Compare & pull request"** — click it.
3. Ensure:
   - **Base repository:** original MLCoE repo → `main`
   - **Head repository:** your fork → `Your-Name`
4. Add a clear PR title and description (e.g., *"Add introduction folder for Aman Verma"*).
5. Click **Create Pull Request**.

---

### 11 Review Process

The MLCoE team will review your PR. This may involve:
-  Approval and merge, or
-  Requested changes

**If changes are requested:**

1. Make the required edits locally in your `Your-Name/README.md`.
2. Check status/diff again:

       git status
       git diff

3. Stage, commit, and push the update on the **same branch**:

       git add .
       git commit -m "Update README as per review comments"
       git push origin Your-Name

4. The PR updates automatically — no need to create a new one.

---

### 12 Merge

Once approved, the MLCoE team will merge your PR into `main`. 🎉 Your task is complete!

---

##  Expected Repository Structure

    Repository/
    ├── README.md
    ├── Aman-Verma/
    │   └── README.md
    ├── Adeed-khan/
    │   └── README.md
    ├── Priya-Singh/
    │   └── README.md
    └── ...

---

##  Trainee README Template

Use this structure inside `Your-Name/README.md`:

    # Hi, I'm Your Name 

    ## About Me
    A short paragraph about yourself.

    ##  Education
    - Degree, College Name, Year

    ##  Technical Skills
    - Languages: 
    - Frameworks/Tools: 
    - Other Skills: 

    ##  Areas of Interest
    - e.g., Machine Learning, Web Development, etc.

    ##  Hobbies / Interests
    - e.g., Reading, Gaming, Sketching

    ##  Goals
    - What you aim to achieve during your time at MLCoE

---

##  Important Guidelines & Common Mistakes to Avoid

|  Don't |  Do |
|---|---|
| Work directly on `main` | Always create your own branch |
| Push to the original repository | Push only to your **fork** |
| Create a `Trainees/` parent folder | Place your folder directly in root |
| Modify the main `README.md` | Leave the root README untouched |
| Add extra files in your folder | Only include `README.md` |
| Use vague commit messages like `"update"` | Write clear, meaningful messages |
| Forget to check `git status`/`git diff` before committing | Always review changes first |

---

##  Final Checklist

- [ ] Forked the original repository
- [ ] Cloned my fork locally
- [ ] Created a branch with my name
- [ ] Created a folder with my name in the root directory
- [ ] Added `README.md` inside my folder with all required sections
- [ ] Verified changes with `git status` and `git diff`
- [ ] Staged changes with `git add`
- [ ] Committed with a meaningful message
- [ ] Pushed my branch to my fork
- [ ] Created a Pull Request to `main` of the original repo
- [ ] Addressed review comments (if any)
- [ ] PR merged 

---

##  Final Repository Structure Example

    Repository/
    ├── README.md
    ├── Aman-Verma/
    │   └── README.md
    ├── Adeed-khan/
    │   └── README.md
    ├── Priya-Singh/
    │   └── README.md
    ├── Neha-Gupta/
    │   └── README.md
    └── ...

---

 **That's it!** Completing this task means you now understand the core Git & GitHub workflow used in real-world collaborative projects. Welcome aboard, and happy contributing!