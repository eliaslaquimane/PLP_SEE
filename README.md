I was tranning github command and I found an issues when I trying to push my file to this repo, the message that was appear on my terminal was: remote: Permission to eliaslaquimane/PLP_SEE.git denied to ohayatech.
fatal: unable to access 'https://github.com/eliaslaquimane/PLP_SEE.git/': The requested URL returned error: 403

to solve this error I used the following command:

# first a verify the github authentication status to see the user or account that I being used:
gh auth status

# secund  I logout other account that was using with:
gh auth logout

# third I login with the account that I have the repo to push
gh auth login

# And Then I make a push, it work good.

git push -u origin main

