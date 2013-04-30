Fork benchmark
==============

Fork benchmark is a primitive benchmark that measures the time that is required to fork, exec and destroy x processes, where you can define x as the command line argument.

I created it because I was wondering why SysVinit is so slow.  Hint: It's not because forks are slow, but but because init runs the services scripts sequantially, not in parallel.