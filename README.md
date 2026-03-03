# Beginner Git & GitHub Activity

Welcome! This activity will guide you through the basic workflow developers use to contribute to a project.

You will:
1. Fork a repository
2. Clone it to your computer
3. Create a branch
4. Make a change
5. Add and commit your change
6. Push your change to GitHub
7. Create a Pull Request

Estimated time: 20–30 minutes.

---

# Overview of What You Are Doing

You will be working in three places during this activity:

1. The original project repository
2. Your fork (your copy of the repository on GitHub)
3. Your local repository (on your computer)

Workflow:

Fork → Clone → Branch → Edit → Commit → Push → Pull Request

---

# Step 1: Fork the Repository

Go to the repository page and click:

Fork

What this does:
- Creates your own copy of the project under your GitHub account
- Allows you to make changes without affecting the original project

After forking, you will work from your copy of the repository.

---

# Step 2: Clone Your Fork to Your Computer

Open a terminal and run:

```bash
git clone https://github.com/YOUR-USERNAME/git-practice-group.git
```

Then move into the project folder:

```bash
cd git-practice-group
```

What just happened:
- The repository was downloaded to your computer
- Git created a local working version of the project
- Your local repo is now connected to your fork on GitHub

Check that everything worked:

```bash
git status
```

---

# Step 3: Create a Branch

Now create a new branch where you will make your change.

```bash
git checkout -b add-my-name
```

What this does:
- Creates a new branch
- Switches you to that branch

Why we do this:
Multiple people can work on the project at the same time without breaking the main branch.

Check your branch:

```bash
git branch
```

Your branch should have a star next to it.

---

# Step 4: Open and Edit the File Using nano

We are going to edit this file:

```
participants.md
```

Open it with nano:

```bash
nano participants.md
```

Nano is a simple editor that runs inside the terminal.

You should now see the contents of the file.

Add your name to the list:

```
- Your Name
```

Example:

```
- Alex
- Jordan
- Taylor
- Your Name
```

---

# How to Save and Exit nano

Save the file:
Press

CTRL + O

Then press Enter.

Exit nano:
Press

CTRL + X

Now you are back in the terminal.

---

# Step 5: Add the File (Stage Your Change)

Now tell Git that you want to include your change in the next commit.

```bash
git add participants.md
```

What this does:
Moves your changes into the staging area.

You can check it worked:

```bash
git status
```

You should see the file listed under:
Changes to be committed

---

# Step 6: Commit the Change

Now create a commit.

```bash
git commit -m "Added my name to the participants list"
```

What a commit is:
A saved snapshot of the project at a specific moment in time.

Each commit has:
- A message
- An author
- A unique ID
- A history connection to previous commits

You just created a new commit on your branch.

---

# Step 7: Push Your Branch to GitHub

Now upload your branch to GitHub.

```bash
git push origin add-my-name
```

What this means:
origin = the remote repository on GitHub  
add-my-name = the branch you created

What happens now:
Your branch and commit are uploaded to GitHub.

Your work is now visible online.

---

# Step 8: Create a Pull Request

Go to your repository on GitHub.

You should see a message like:

Compare & Pull Request

Click it.

Then:
1. Add a title
2. Click Create Pull Request

What a Pull Request is:
A request to merge your changes into the main project.

It allows others to:
- Review your code
- Ask questions
- Suggest improvements
- Merge your work

---

# What Happens After You Submit a Pull Request

The project maintainer can:

Approve your change  
Request changes  
Merge your contribution

When your Pull Request is merged:
Your work becomes part of the project.

Congratulations — you contributed to a repository!

---
