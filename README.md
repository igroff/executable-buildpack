#### Executable Buildpack

This build pack does nothing at all except start something for you.  It looks for
an executable file 'server' in the root of your repository called server, and runs it.
You'll need to make sure that the executable looks for and honors any variable PORT
in the environment, and binds an HTTP server to that port, other than that the sky's the limit.
