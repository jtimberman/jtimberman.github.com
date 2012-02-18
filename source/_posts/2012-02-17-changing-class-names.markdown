---
layout: post
title: "Changing Class Names"
date: 2012-02-17 09:39
comments: true
categories:
---

Chef mailing list post: http://lists.opscode.com/sympa/arc/chef/2012-02/msg00220.html

Output from bluepill command.

GitHub issue for bluepill: https://github.com/arya/bluepill/issues/132

Daemons gem: http://rubygems.org/gems/daemons

Where's the source? http://rubyforge.org/projects/daemons

Changelog from daemons gem:

    Release 1.1.8: February 7, 2012
    rename to daemonization.rb to daemonize.rb (and Daemonization to Daemonize) to ensure compatibility.

    Release 1.1.7: February 6, 2012
    start_proc: Write out the PID file in the newly created proc to avoid race conditions.
    daemonize.rb: remove to simplify licensing (replaced by daemonization.rb).

    Release 1.1.6: January 18, 2012
    Add the :app_name option for the "call" daemonization mode.

    Release 1.1.5: December 19, 2011
    Catch the case where the pidfile is empty but not deleted and restart
    the app (thanks to Rich Healey)

License issue of daemonize.rb? Why didn't this create a new major version?

http://rubyforge.org/tracker/index.php?func=detail&aid=29516&group_id=524&atid=2084

I added a comment. Hopefully the author does the right thing.
