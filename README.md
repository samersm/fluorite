# Fluorite

###### The fluorite gemstone’s attributes are predominantly connected with specific area of fortification and stabilization.

# cmd-cheatsheet


## Github

```
* git status

* git add .

* git commit -m "your commit"

* git push

* git push --set-upstream origin master         // To use only git push to github

* git reset --hard HEAD         // To revert to a previous commit, ignoring any changes

* git clean -f -d       // to get rid of untracked files and directories in your working copy

* git commit --amend -m "New commit message"     //To edit your latest commit

* git push -f

* git reflog    //To get a detailed specific

* git revert HEAD   //To undone the latest commit and you can push the new changes normally

* git revert --no-commit HEAD         // To revert two or more commits

* git revert --no-commit <commit id>    // Then You can commit and push normally

* git clone -b <branch> <remote_repo>

* git clone <project path>

* rm -rf .git

* git branch    // To view the list of your branches

* git branch new_branch         // To create a branch

* git checkout -b new_branch    // To create a branch and switch to it

* git checkout branch_name      //To switch branch

* git checkout master   // To merge branche to master

* git pull origin master

* git merge testBranch

* git push origin master        // To Push the changes to master

* git rebase master     // To Take the master codes into different branch

* git rebase --skip     // To skipping the commits already in master

* git remote rename <old> <new>         // To rename a project in git

* heroku domains        //To view all your domains

* heroku rake db:migrate

* git push -f heroku master

* git remote add origin <link>

* git pull / git fetch / git clone

* mkdir <foldername>

* touch <filename>.md

* pwd   // print working directory - shows what directory you are in

* ls    // list the files in this directory

* git log  	//show all commits

* git log —stat 	//Show more details on commits

* git-diff      //Show changes between commits, commit and working tree, etc

* git checkout <commit id>      // To get back and check a specific commit

* git checkout master       // To get back to the head commit

* git stash         // To checkout without commit the changes

* git stash list

* git stash show

* git stash apply   // To get back to the uncommitted changes

* git stash clear   // You should clear your stash after applying it

* git remote add origin <link> 	//To link github to a local machine

* git pull origin master 			//To pull from github to local machine

* git remote add upstream <Github Link URL>         // To Fork a github rebository <Fork from website>

* git remote -v         // Then Clone the repository

* git pull upstream master              // Use upstream to sync

* mv <folder to move> <destination>     // To move folder with git

* mv /home/<user>/South_America /home/<user>/North_America/

* mv ~/workspace/clone/<your_project>/ ~/workspace/projects/           // In C9

* git remote set-url origin git@github.com:username/repo.git    // To wrok whith github repo after cloning

$ c9 ../../folder/file.html   // To open file in c9

$ open file.html  // To open a file in mac os

$ open -a "Atom" file.html  // To open a file in mac os with specific app.
```


## Rails

```
* ruby -v

* brew upgrade ruby     //To update ruby with brew

* rvm list rubies       //Check if rvm is installed

* rvm install ruby-2.4.1  // To update ruby with rvm

* rvm --default use 2.4.1   // To upgrade ruby in c9

* rails -h      // to show all command lines)

* gem install rails

* rails -v

* rails new <name>

* bundle install

* bundle check

* gem list

* gem uninstall <gem name>

* rails routes

* rails db:migrate

* rails db:reset        //Reset-Rebuild database/tables/columns based on migration

* cd rails-projects/saasapp/

* rails s -b $IP -p $PORT

* rails c -h    // for show all command lines)

* rails c       -       rails c -s
        Hirb.enable     // related to hirb gem
        Contact.all
        Contact.create(name: "test", description: "test")

* rails g migrate <UserProfiles>

* rails g controller <Users> <show>

* rails g scaffold <User title:string description:text>

* rails g paperclip <profile> <avatar>

* rails g model <Play title:string description:text director:string>

* rails g controller Plays -s    // -s means that skip the existing files

* RAILS_ENV=production rake db:migrate 	//To run rails in production mode

* rails server -e production
```


## NodeJS

```
* npm init      // To start a new npm project

* npm install   // To install all the dependencies in package.json file

* npm install -g <package>        // To install npm package globally

* npm install -s <package>        // To install npm and save it to a package.json file

* npm install --save-dev @angular/cli@latest    // To install packcage in dev dependencies with latest version

* npm start

* npm list      // To view all the npm list

* npm list --depth=0         // To view all installed npm list in the project/dir

* npm list -g --depth=0         // To view all globally installed npm list 

* npm outdated          //To check witch packages need to update

* npm update    // To update all packages in the same directory as the package.json

* npm update <package>    // To update one installed package in the same directory

* npm outdated -g --depth=0     //To find out which global packages need to be updated

* npm update -g         //To update all global packages

* npm update -g <package>         //To update one global package

* npm cache clean

* npm cache verify              // Cache clean for the new node version

* npm prune     // Allow you to delete Nodejs project (u need to clear package.json first)

* npm uninstall -s <package>

* npm uninstall -g <package>

* brew upgrade node     //To update node with brew

* nvm install 6.0.0  	//To update nodejs to the latest version with nvm

* nvm install node

* nvm use 7.4.0

* nvm alias default v7.4.0

* npm install -g npm    // Update npm
```


## Angular

```
* npm install -g @angular/cli

* ng new <appName>      //To create a new angular project

* ng new <appName> --directory ./       //To create new app in the same dir/

* ng generate component views/heroes

* ng generate component pages/dashboard

* ng generate module config/app-routing --flat --module=app

* ng g service services/hero --module=app

* ng serve --host 0.0.0.0 --port $IP  	//to run angular 2 app

* ng serve --host 0.0.0.0 --port 8080 --live-reload-port 8081

* ng serve --host 0.0.0.0 --public-host <workspace>-<username>.c9users.io //To run updated angular 2
```

## React
```
* npm install -g create-react-app

* create-react-app <appName>
```

## MongoDB
```
* brew update

* brew install mongodb

* brew services start mongodb

* mongo
        // Inside the console shell
        * show dbs
        * use <DB Name>         // To create new db
        * show collections      // To view tables
        * db.createCollection('tablename')
        * db.tablename.insert((name:'data', title:'data'))       // To Insert data to the database
        * db.tablename.find()   // To View inserted data
```

## python

```
* python —version
* python	 //to go to the python console
        >>> help('modules')  	// to see a list of your installed packages

* python <filename>.py

* sudo easy_install markdown 	//to install new package
```


## django

```
* mysql-ctl start

* python -m django --version

* django-admin startproject <project name>

* python manage.py startapp <page name>

* python manage.py migrate

* python manage.py runserver $IP:$PORT
```


## PHP

```
// setting up phpmyadmin for c9
$ mysql-ctl install
$ phpmyadmin-ctl install
$ mysql-ctl start

// php c9 updates commands
$ sudo apt-get update
$ sudo apt-get install libmcrypt-dev

$ curl -L -O https://github.com/phpbrew/phpbrew/raw/master/phpbrew
$ chmod +x phpbrew
$ sudo mv phpbrew /usr/local/bin/
$ phpbrew init

$ [[ -e ~/.phpbrew/bashrc ]] && source ~/.phpbrew/bashrc

$ phpbrew lookup-prefix ubuntu

$ phpbrew install 7.1.9 +default
$ phpbrew switch php-7.1.9
$ phpbrew use php-7.1.9
$ php -v

// Works Fine!

// To unzip file from c9
$ unzip <my_arch>.zip
```


## Homebew

```
* brew list

* brew update

* brew install <packagename>

* brew upgrade <packagename>    //To update single package

* brew link --overwrite <packagename>

* brew postinstall <packagename>

* brew uninstall <packagename>

* brew cleanup

* brew services list    //Check for serveces Running/Stopped

* sudo chown -R $(whoami) /usr/local 
* sudo chown “whoami” /data/db

* brew services start mongodb
        * mongo
```