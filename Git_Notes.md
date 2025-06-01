###### List of commands and tricks usually used

1. Setting the git configs locally.
- <pre>
    git config user.name __name__
    git config user.email __email__
    git config core.autocrlf
    git config core.commentchar ";"
  </pre>

2. Special sequence for git 
- This sequence is used when you want to make changes to some old commits
  <pre>
    git add __files_you_want__
    git commit --fixup=__OLD_COMMIT__
    git rebase --interactive --autosquash __OLD_COMMIT__^
  </pre>
  Please make sure you include "^" and the end of the commit
- Tricks can be used in git fetching
  <pre>
    git fetch origin refs/heads/__remote_branch_name__
  </pre>
  Same approach can be used for pull as well.
