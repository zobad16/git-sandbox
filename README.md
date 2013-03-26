# Welcome to the Git Sandbox

This is a simple repo to help people play with git for the first time, this README will attempt to walk you through the various steps to making a modifications to the repo and pushing them back to github.

If the previous statement was about as clear as mud don't worry! Read the next section, it will give you a starting place. If however you've come the world of SVN or even mercurial you may want to skip the next section.

# I have no idea what anything you said means....

Well, first let me welcome you to the wonderful world of (distributed) version control. A software paradigm that allows multiple developers to work on the same code base at the same time and maintain versions. It can do this by maintaining changes you've made to files and then merging those changes together with others changes. To give you the most insanely brief history of version control I'm going to refer to the following list (note: I don't include preprietary solutions like MS source safe or the precursor to git itself, sorry):

1. In the beginning there was CSV ( http://en.wikipedia.org/wiki/Concurrent_Versions_System )
2. It was followed by SVN ( http://en.wikipedia.org/wiki/Apache_Subversion )
3. Soon after came Mercurial http://en.wikipedia.org/wiki/Mercurial and Git ( http://en.wikipedia.org/wiki/Git_(software) )

If you're that interested in the history of things you're going to have to read up on the history of it all, the combined history of all of them would be far, far, beyond the scope of this README, and, let's be honest, I'm lazy.

Suffice it to say that we started with a simple server-client architecture and ended up in a world that we call distributed version control systems. The idea behind this new generation of version control systems (VCS) was that code "features" shouldn't be so hard to manage. In the past when they wanted to split off from the trunk (think a tree) and make vast changes to the source they would create branches the problem with the older generation of VCS's really sucked at this operation. Specifically when it came to bringing all those changes from that new branch back into the trunk.

Newer systems such as git and mercurial took a different approach, instead of creating these nearly immutable branches they decided that branching should be a light and common affair. To do this they made it so branches could be relocated to different points in the history of the repository, in git terms this is called rebasing but more on that later.

Such is the state of things, git made managing branches, and sub-branches less of a pain which made things awesome!

# OK, so I have some idea of what that meant, but what is all this pushing stuff? Is it like svn pull?

No, well, kind of, but not really. You see modern DVCS's have a concept of a local repoistory and a remote repository. The idea being that you'd perform all of your work in your local repository and not push those changes to the remote (public area where other developers can see them) until they were ready. Gone are the days where you maintain a lock on a file or where you're forced to push out incomplete code.

It's best to think of it this way, your local repo is your desk where you keep your stationary, you're free to write what ever you want and you won't effect anyone else. But then you walk downstairs to your apartments lobby and pin it to the board. Now your changes are in a remote place and free for all to see and copy.

# Awesome! So where do I begin?

Well this entire repo is inteded to be a safe play ground for you to futz around in. I would suggest that you fork this repo via githubs fork functionality and then clone the repository.

## Fork wha now? Clonning? Like sheep?

Forking is where you create a completely independent copy of a repository. Though I think you're awesome for reading this document I'm not going to let you commit changes to this repository all willy nilly like.

Cloning is where you create a local copy of your repository. It's somewhat in a vague sort of way related to svn checkout. Anyhow let's get started

After you've forked the repo you should clone it (note: be sure to replace $USER$ with your github user name):

<code>git clone https://github.com/$USER$/git-sandbox.git</code>



