# opim5512-dww05002-answers
Dave's solutions to the HW

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
