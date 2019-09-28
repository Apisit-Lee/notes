Recently I met a problem while creating new projects. I created a local project and wrote something. Then I wanted to push it to git. I created a new git repo, add remote origin, commit & push, and error occured, like bellow:

`fatal: refusing to merge unrelated histories`

It means the local repo and the remote repo has no related history, thus git did not execute my command for the safty reason. In this occasion, I should fix it with: `git pull origin master --allow-unrelated-histories`. This command pulls remote repo to local omitting the related history. Thus remote and local repos are related, I could do push excution freely.

