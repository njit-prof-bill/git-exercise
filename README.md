# Git and GitHub Excercise
This is a simple exercise to get familiar with using Git and GitHub. Students will collaborate to create a "Class Roster" where each person contributes their personal information. This will demonstrate branching, cloning, creating a PR, reviewing, and merging.

This assignment is due Sunday 9/10 at midnight.

### Tools Required
- A computer with Git installed.
- A GitHub account.

### Step 1: Getting Started
- Instructor created a new public repository on GitHub called `git-exercise`.
- The repo has a README.md that explains the project: "This is a collaborative roster. Each contributor should add their personal information."
- The repository is available at https://github.com/njit-prof-bill/git-exercise.
- The instructor will send an invite to this repository that will allow you to push your branch to GitHub. In order for him to send the invite, you must post your GitHub id in the Discord #General channel.

### Step 2: Cloning the Repository
1. Each student clones the repository to their local machine using:
```
git clone https://github.com/njit-prof-bill/git-exercise
```

Student may use the GitHub website for cloning, or may also use GitHub Desktop.

### Step 3: Creating a New Branch
Each student creates a new branch to work on their information, replacing [student_name] with their own name:
```
git checkout -b add-info-[student_name]
```
**Important** You will get a zero for the assignment if you commit directly to the main branch!!

### Step 4: Adding your Information
1. Each student creates a new .md file named after themselves (e.g., bill-mccann.md).
2. Inside the file, they add their personal information using markdown formatting.
3. Commit the changes:
```
git add [your file_name].md
git commit -m "Added the information for [student_name]"
```

Make sure your document contains:
- Your name
- Your favorite programming language
- Your preferred IDE
- Your hobbies
- Your favorite cartoon from your childhood
- A favorite movie, book, music, or video game
- Your discord id
- Your GitHub id

You get an extra credit point if the information is formatted in a table (using markdown).

### Step 5: Pushing the Branch and Creating a Pull Request (PR)
1. Student pushes their branch to GitHub:
```
git push origin add-info-[student_name]
```
2. Go to the git-exercise repository on GitHub, where you'll see a message about your recently pushed branch. Click "Compare & pull request."
3. Fill out the PR details, explaining your addition, and then create the pull request.

### Step 6: Reviewing the Pull Request
1. Paired up review each other's PRs.
2. Reviewer looks over the info file in the PR, checking for any mistakes or suggestions. Type a message in the General channel use the @discord_name to tag the person.
3. Reviewer checks to make sure that all the questions have been answered. Request changes if there are unaswered questions.
4. Reviewer can leave comments on specific lines of code or on the PR as a whole.
5. Once the review is complete, if changes are suggested, the author makes the necessary modifications in their local branch and then pushes the updates to the same branch. The PR will be updated automatically.

### Step 7: Merging the Pull Request
1. Once the reviewer is satisfied with the changes and approves the PR, they merge the PR into the main branch.
2. Ensure that information gets merged properly without any conflicts.

### Step 8: Pulling Merged Changes
After their PRs have been merged, students should update their local main branch to have the latest changes:
```
git checkout main
git pull origin main
