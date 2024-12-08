# 2025 Python & HTMX Learning Journal

---

> [!IMPORTANT] Rules for 2025
> 1. Write Python every day
> 2. Journal after playing with any new concept
> 3. At the end of each chapter, write a full blog post explaining the concepts covered in the chapter as if you were teaching them to a child
> 4. Never commit any code without being able to fully explain what it's doing
> 5. Every month, reread and work through one previous chapter from the year
> 6. Detours must remain detours and must not take more than 8 hours of your time a week
> 7. Don't stray from this plan.

---

## December 7, 2024

Topic: `origin` in Git
Resource: [Pro Git - 2.5 - Working with Remotes](https://git-scm.com/book/ms/v2/Git-Basics-Working-with-Remotes)

What I learned:
- `origin` is just a default term to describe a remote repository's URL
- When using `git clone <url>`, a remote will be created with an `origin` representing the given URL
- When initializing a repo locally with `git init`, you will typically add a remote URL where the local code will be pushed. That remote URL is conventially called `origin` though it could be called anything.

Experiments:
- I didn't do anything 😬

Curiosities evoked:
- What is the utility of using multiple remotes?
- Why is `git push -u origin main` necessary after adding a remote and then `git push` works as a standalone therafter?

---

## December 7, 2024

Topic: Tracking relationships between local and remote branches
Resource: [Pro Git - 2.5 - Working with Remotes](https://git-scm.com/book/ms/v2/Git-Basics-Working-with-Remotes)

What I learned:
- `-u` is used to create a tracking relationship between local and remote branches
- When a remote has been added, but the code in the local branch hasn't been pushed to the remote repo, using something like `git push -u origin main` will create a tracking relationship between the local `main` branch and the remote `origin` repo, creating a remote `main` branch at `origin` and pushing the local code to that branch. Thereafter, Git will already be tracking the relationship between the two branches so when you simply `git push`, Git will push the local code to the related remote branch.
- `--set-upstream` is the longhand form of `-u`

Experiments:
- *In progress*

Curiosities evoked:
- *In progress*
