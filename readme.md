
## tools

 * git-todo: A tool for branch summary
 * git-ff: A fetching tool

## git-todo

`git-todo` list branches and tags with author, last commit message, SHA, distances from base branches. you can get a summary for your repository.

### Install

Put `git-todo` in your excutable path:

    cd ~
    git clone https://github.com/dogfeet/git-tles
    echo "export PATH=~/bin:$PATH" >> ~/.bash_profile
    mkdir ~/bin
    cd ~/bin
    ln -s ~/git-tles/git-todo git-todo

### Run

Usage is very simple. Just run:

    git todo

it show your local branches.

![](http://dogfeet.github.com/articles/2012/git-todo/git-todo.png)

* ![](http://dogfeet.github.com/articles/2012/git-todo/checkouted.png) means checkouted branch.
* ![](http://dogfeet.github.com/articles/2012/git-todo/base_branch.png) is base branch(default - master).
* ![](http://dogfeet.github.com/articles/2012/git-todo/ahead.png) is distance. `private-ko-build-ebook` branch has 3 commits base branch does not.
* ![](http://dogfeet.github.com/articles/2012/git-todo/behind.png) is distance. `private-ko-build-ebook` branch does not have 23 commits base branch has.

To change base branch to 'ko' branch, Add 'todo.base' config:

    git config todo.base ko

#### Options

To include remote branches, Add `-r` option

![](http://dogfeet.github.com/articles/2012/git-todo/git-todo-r.png)

To include tags, Add '-t' option

![](http://dogfeet.github.com/articles/2012/git-todo/git-todo-t.png)

To include both of remote brnaches and tags, Add '-a' option

![](http://dogfeet.github.com/articles/2012/git-todo/git-todo-a.png)

## git-ff

It is a git helper like [git-up](https://github.com/aanand/git-up). I will write later.




