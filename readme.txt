git tag -a v1.0 
git tag v1.4-lw

git push origin v1.5
git push origin --tags


Annotated Tags

Creating an annotated tag in Git is simple. The easiest way is to specify -a when you run the tag command:

$ git tag -a v1.4 -m 'my version 1.4'
$ git tag
v0.1
v1.3
v1.4

The -m specifies a tagging message, which is stored with the tag. If you don’t specify a message for an annotated tag, Git launches your editor so you can type it in.

You can see the tag data along with the commit that was tagged by using the git show command:

$ git show v1.4
tag v1.4
Tagger: Scott Chacon <schacon@gee-mail.com>
Date:   Mon Feb 9 14:45:11 2009 -0800

my version 1.4
commit 15027957951b64cf874c3557a0f3547bd83b3ff6
Merge: 4a447f7... a6b4c97...
Author: Scott Chacon <schacon@gee-mail.com>
Date:   Sun Feb 8 19:02:46 2009 -0800

    Merge branch 'experiment'
