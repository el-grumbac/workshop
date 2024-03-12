

### Steps to setup repository in GitHub:
1. Sign in to your account
2. On the lefthand side of your GitHub Dashboard, click "Create Repository" (if this is a new account) or "New" (if you are using an existing GitHub account).
3. On the repo creation page, be sure to check the "Add a README file" checkbox.

### Deploy GitHub pages
1. Navigate to "Settings" on the menu of your repository page.
2. Navigate to "Pages" on the right-hand site menu.
3. Set your branch to "MAIN" and click "Save".

### Create a configuration file
1. Navigate to the "Code" tab of your repository.
2. Click "Add File," then choose "Create New File" from the dropdown.
3. Name your file "_config.yml" -- make sure that the underscore is there!
4. Put at least the below information in your configuation file:
> title: Your title \
> email: Your email\
> theme: minima
5. Click "Commit Changes" button and type in a commit message that describes the edits you just made.
6. Click "Commit Changes" on the pop-up.

### Edit the content on your main page
1. Click on the "README. md" file in the "Code" tab of your repostory.
2. Using [Markdown] (https://daringfireball.net/projects/markdown/syntax), enter in content.
3. Click "Commit Changes" button and type in a commit message that describes the edits you just made.
6. Click "Commit Changes" on the pop-up.

---

## If you’d like to participate in the advanced hands-on version of this workshop, follow the below instructions to install all dependencies needed to spin up a Jekyll site.
* Open up your command line tool:
 for Mac, this is Terminal
 for PC, this is Command Prompt.
  
### Check if Homebrew is installed. 
* Type into the command line:

> brew help.

  * If you do not get a response, copy/paste the below into the command line:

> /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

### Check if Ruby is installed: 

> ruby -v.

  * If you do not get a response, copy paste the below into the command line:

> brew install ruby

### Check if Bundler is installed: 

> bundle help (type q to exit)

  * If you do not get a response, you might have an outdated version of Ruby installed:

> brew upgrade ruby /
> gem install bundler

#### While we won’t have time today to ensure everyone can connect to GitHub from the command line, you can follow the instructions here to install Git or “brew install git”.

* For Mac: https://git-scm.com/download/mac
* For Windows: https://git-scm.com/download/windows

Then you can follow the instructions [here] (https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)to set up your SSH key in GitHub to connect your local repositories to GitHub.

---

## Installing and Running Jekyll on your local server

1. Install all dependencies (see above section).
2. Install Jekyll and Bundler
> gem install jekyll bundler
3. Navigate to the directory you wish to install your new Jekyll site
> cd directory_name
3. Create a new Jekyll site
> jekyll new ENTER_SITE_NAME_HERE
4. Change into your new directory
> cd SITE_NAME
5. Built the site and make it available on your local server
> bundle exec jekyll serve
6. Access your site at http://localhost:4000 
