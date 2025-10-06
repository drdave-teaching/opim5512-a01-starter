# opim5512-a01-starter
This is the starter repo for students to clone to their own repository. 

## First, make sure you have GitHub CLI installed (should only need to do this once.)
```bash
# Install GitHub CLI (Windows)
winget install GitHub.cli

# Verify
gh --version

# Login (follow the browser flow)
gh auth login
# → GitHub.com → HTTPS → "Login with a web browser"
```

## Now you can clone it!

```bash
cd $HOME\Desktop

# set params
$ORG      = "drdave-teaching"
$ASSIGN   = "a01"        # change to a02 when needed
$NETID    = "dww05002"   # student edits this
$TEMPLATE = "$ORG/opim5512-$ASSIGN-starter"
$NEWNAME  = "$ORG/opim5512-$ASSIGN-$NETID"

# create a new repo from the template and clone it here
gh repo create $NEWNAME --template $TEMPLATE --private --clone

# enter the new repo and start a working branch
cd ".\opim5512-$ASSIGN-$NETID"
git switch -c "$ASSIGN/$NETID-work"
git push -u origin HEAD
```
## After you do the assignment, get the commit message. 
### 1) Make & push your commit
```bash
# from repo root
git add -A
git commit -m "A02: <short, imperative summary>"
git push -u origin HEAD   # pushes your current branch
git log --oneline -1      # copy the 7-char commit hash (e.g., a1b2c3d)
```
### 2) Open a Pull Request (Web UI)

1. Go to your repo → **Compare & pull request** (or **Pull requests → New pull request**).
2. Set **Base**: `main` and **Compare**: *your branch*.
3. **Title**: `[A02] <short title>`.
4. In the PR description, paste:
   - **Latest commit:** `a1b2c3d`
   - **What changed:** 1 sentence
5. On the right side:
   - **Reviewers** → add **drdww** (if allowed)
   - **Assignees** → you (and TA if applicable)
   - **Labels** → `A02`, `review`
6. Click **Create pull request**.
