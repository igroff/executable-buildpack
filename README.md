#### Executable Buildpack

This build pack does nothing at all except start something for you.  It looks for
an executable file named server in the root of your repository called server, and runs it.
You'll need to make sure that the executable looks for and honors any variable PORT
in the environment, and binds an HTTP server to that port, other than that the sky's the limit.


#### Really?

Yup, that's all there is to it. So let's say you have a repository called echo in your 
home directory, if you can do this

      15:14:20 ~
      $ cd echo/
      15:14:22 ~/echo
      $ ls -l server

And you see something like this:

      -rwxr-xr-x  1 owner  group  7 Sep 30 13:12 server

You're golden, yes the only thing you need is an executable file called server at the root of your
repository.  That's it, really.


#### What else does it do?

Nothing, really.  All the buildpack does is check for the file you need, the compile step is a no op.
It really desn't do anything other than check for the file, and set things up so it's started at the
appropriate time.

