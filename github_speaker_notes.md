## Today's Itinerary

Hi everyone, we'd like to go over today's itinerary.  We have 90 minutes and we have no break scheduled.  Everything we do today can be done in the browser, so you don't need any special software installed.  We're also going to make sure you know where to go to get our materials so if you want to go back over what we talked about, you have access to the materials later.

We're going to start of talking about GitHub.  Joy Payton will lead that effort.  

Then Elizabeth Drellich will take on the topic of Markdown.

Finally, _______________ will present Liascript.  Liascript, by the way, is what you see here on your screen.

##  Logging into GitHub

First step: go to <https://github.com> and either:

* login (if you have an account)
* create an account (it's free!)

GitHub is a website that provides storage for git repositories (we'll explain this a bit more) as well as some helpful add-ons that are often used by software developers.  You may or may not use these helpful add-ons such as issues, pull requests, projects, etc.

## Your Account Homepage

Let's take a look at some of what you might see on your Git account homepage.  Here is my GitHub account homepage!

![](media/github_account_home.png)

* In the yellow highlighted area, you can see biographical information, which you can optionally add if you want.
* In the purple box, here are some of my pinned repositories, which are the ones I want easily visible for fast access.  A repository is a directory of files all related to a single project.  
* In green, at the top, we see the "Repositories" tab, where I can see all 59 of my repositories.
* And finally, if you follow the orange arrow on the right side, you can see a plus button which will allow me to add a new repository.

If you think of the word *hub* as referring to a central place for something, you might realize that "GitHub" is a central place for "git".  But... what's git?  Before we start diving into this website, what is it all about?

### Git is Version Control

Git is the technical industry standard for version control.  Version control exists in order to give you access to any version of a text file (usually code or configuration files) at any time, with helpful messages that tell you why things changed and by whom. Often, a scientist’s first form of version control is something like this first image:

![](media/primitive_version_control.png)

If you have a file system that looks like this, with clues embedded in file names, you have a crude (and large, and hard to work with) version control system already. You probably have to say things like “no, it’s the one with the time stamp in March, remember, because in April that was the one that says ‘final’ but it’s not really …”. Maybe you’re afraid to throw any of the files away because you’re not 100% sure you remember exactly why you made that particular version, but you’re a little chagrined that you have 10 versions of (mostly) the same .csv. If your files are large, you might have a storage problem as well!

And what about your clinical or research collaborators? Are you sending these files back and forth over email for each member to make changes? What if someone accidentally works on a version that doesn’t include the changes of another collaborator? Working by committee is hard when you rely on local copies. Maybe you have just one copy on a server that everyone has access to, which is better. But while you have the file open, your assistant or co-PI can’t make changes. Frustrating!

Good news! There is a better way to do version control. While there are several methods out there (e.g. Subversion), Git has won the market.

Git helps you track changes in your text (more on this later) files.  Specifically, Git will help you track the version of your files and keep records of:

* What changed
* When it changed
* Who changed it
* Why they changed it

Not only does Git keep a record of this, but it allows you to go back in time and recapture things you deleted or changed and now have second thoughts about.  This is great because it keeps you from hoarding multiple versions of a file, which fill up your hard drive and also give you heartburn when you have to comb through them to find that one thing you are looking for.

Now, earlier, we said that Git helps track changes in **text** files.  What did we mean by that?


#### Text files

Git does its best work when you track changes in your **text** files.  By "text" here we mean files that are encoded in plain text, like .txt files, computer code like Python files, configuration files, data files like .json and markdown/markup files like .xml or .yaml.  Specially formatted "word processing" documents like Microsoft Word or .pdf documents aren't encoded in plain text and aren't "text files" in this sense.  Why does this matter?

Because while Git can tell exactly what line and what characters changed in a text file, and highlight those changes so you can see easily what changed, Git cannot do that level of specificity for non-text files.  If you have an image or a PowerPoint slide deck, and you put that in a Git repository, it can only tell you *that* it changed, and by whom, and their message for why it changed.  It can't tell you, say, that you added two extra slides, or that the image now is in black and white instead of color.

### Git in GitHub

“git” is a command line tool, a program that uses a set of rules that governs how the Git version control system works. You can use it by itself and do everything you need to, if you’re comfortable working on the command line. Lots of people do just that!

While Git by itself is great at version control and keeping track of your changes, GitHub wraps all of the sometimes complex inner workings of Git into a visually pleasing, easy to understand user interface.   GitHub is a company that has done a good job of making tools that work with git, but GitHub and git are distinct products, maintained by different organizations.  You may want to learn more about git itself, or you might want to investigate other products that are GitHub competitors, like BitBucket.  That being said, we're going to teach you some things about GitHub today, because we think that's a good way to start thinking about these ideas for the first time.

Instead of having to learn a bunch of command line tools, GitHub (both the website as well as the client software you can run on your computer) allows you to see things like version history, file change summaries, etc., very simply. It’s fairly intuitive for most day-to-day uses.

GitHub (the website) is a also place for your files to live with version control applied to them, so you can think of it as a souped-up remote server. That means it’s great not only for version control (which you could just do on your local computer using a git-enabled product like GitHub Desktop), but also having a central hub for all your files that you and your collaborators can use as the canonical source of the best, most up-to-date files.

## Creating a Repository in GitHub

![](media/new_repository_button.png)<!-- style = "border: 1px solid;" -->

![](media/new_repository_form.png)<!-- style = "border: 1px solid;" -->

### Examine Repository

![](media/repository_view.png)<!-- style = "border: 1px solid;" -->

### README.md

### Editing Files in Browser

### Preview

### Saving Files and Committing

### Uploading an External File
