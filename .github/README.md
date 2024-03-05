# Tech Business Brain - Notes on Startups, SaaS, Entrepreneurship, Funding, etc

By Weng Fei Fung.

Collection of SaaS tech entrepreneur notes. The goal is to record what I learn as I start tech businesses, read business books, talk to business persons, etc. I want to leverage what I know from software development into my own startups.

### Mac workflow Obsidian to Terminal: 
I am authoring the curriculum separately inside an Obsidian MD vault. I can manage the git repository by right clicking the curriculum folder in Obsidian -> Reveal in Finder -> New Terminal at Folder (on the highlighted folder in Finder). Now I can run git and other terminal commands.

### Server pipelines
My apache server has a script I can trigger from my local machine. ~~When triggering from my local machine, it tunnels SSH then runs a script at the server to fetch then reset hard to origin/main.~~ I created a npm script called `deploy` to streamline the server pipeline and it works by staging and committing most recent files changes, pushing to Github repository, then opening a PHP file with the secret token to have the remote server perform a git fetch and git reset. There is no pulling or merging because I'm not editing from the server and want to prevent the pipeline from being broken when there's a chance of merge conflicts that require manual interaction from the user.

In order for the server pipeline to work, I made sure there is good file permissions at SSH by going to the directory containing the app which contains the curriculum. Then I ran `sudo chown -R user:user 3dbrain-front`. The `-R` performed the chown recursively. I made sure the `user` is the user shown by server-update.php's debugging information. If this were not done, when the npm script `deploy` opens the php file, you will see the error about file permissions making it impossible to unlink or link your new files as part of the fetch/reset. Finally, I ran `sudo chmod -R u+w 3dbrain-front`.
