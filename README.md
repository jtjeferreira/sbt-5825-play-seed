# Play 2.8

The error is a bit different:
```
[info] welcome to sbt 1.4.0-RC1 (AdoptOpenJDK Java 11.0.6)
[info] loading settings for project global-plugins from idea.sbt,plugins.sbt,sbt-updates.sbt ...
[info] loading global plugins from /home/joao/.sbt/1.0/plugins
[info] loading settings for project sbt-5825-play-seed-build from plugins.sbt ...
[info] loading project definition from /home/joao/git/sbt-5825-play-seed/project
[info] loading settings for project root from build.sbt ...
[info] set current project to sbt-5825-play-seed (in build file:/home/joao/git/sbt-5825-play-seed/)
[info] 
[info] Here are some highlights of this release:
[info]   - Build server protocol (BSP) support
[info]   - sbtn: a native thin client for sbt
[info]   - VirtualFile + RemoteCache: caches build artifacts across different machines
[info]   - ThisBuild / versionScheme to take the guessing out of eviction warning
[info] See http://eed3si9n.com/sbt-1.4.0-beta for full release notes.
[info] Hide the banner for this release by running `skipBanner`.
[info] sbt server started at local:///home/joao/.sbt/1.0/server/6e4b7618f2ae1f9501d8/sock
sbt:sbt-5825-play-seed> run
Starting server

--- (Running the application, auto-reloading is enabled) ---

[info] p.c.s.AkkaHttpServer - Listening for HTTP on /0:0:0:0:0:0:0:0:9000
[success] Total time: 3 s, completed Sep 8, 2020, 9:32:53 PM
[error] a.a.ActorSystemImpl - Internal server error, sending 500 response
akka.http.impl.util.One2OneBidiFlow$OutputTruncationException: Inner flow was completed without producing result elements for 1 outstanding elements
	at akka.http.impl.util.One2OneBidiFlow$OutputTruncationException$.apply(One2OneBidiFlow.scala:22)
	at akka.http.impl.util.One2OneBidiFlow$OutputTruncationException$.apply(One2OneBidiFlow.scala:22)
	at akka.http.impl.util.One2OneBidiFlow$One2OneBidi$$anon$1$$anon$4.onUpstreamFinish(One2OneBidiFlow.scala:97)
	at akka.stream.impl.fusing.GraphInterpreter.processEvent(GraphInterpreter.scala:523)
	at akka.stream.impl.fusing.GraphInterpreter.execute(GraphInterpreter.scala:390)
	at akka.stream.impl.fusing.GraphInterpreterShell.runBatch(ActorGraphInterpreter.scala:625)
	at akka.stream.impl.fusing.GraphInterpreterShell$AsyncInput.execute(ActorGraphInterpreter.scala:502)
	at akka.stream.impl.fusing.GraphInterpreterShell.processEvent(ActorGraphInterpreter.scala:600)
	at akka.stream.impl.fusing.ActorGraphInterpreter.akka$stream$impl$fusing$ActorGraphInterpreter$$processEvent(ActorGraphInterpreter.scala:769)
	at akka.stream.impl.fusing.ActorGraphInterpreter$$anonfun$receive$1.applyOrElse(ActorGraphInterpreter.scala:784)
[error] a.a.ActorSystemImpl - Internal server error, sending 500 response
akka.http.impl.util.One2OneBidiFlow$OutputTruncationException: Inner flow was completed without producing result elements for 1 outstanding elements
	at akka.http.impl.util.One2OneBidiFlow$OutputTruncationException$.apply(One2OneBidiFlow.scala:22)
	at akka.http.impl.util.One2OneBidiFlow$OutputTruncationException$.apply(One2OneBidiFlow.scala:22)
	at akka.http.impl.util.One2OneBidiFlow$One2OneBidi$$anon$1$$anon$4.onUpstreamFinish(One2OneBidiFlow.scala:97)
	at akka.stream.impl.fusing.GraphInterpreter.processEvent(GraphInterpreter.scala:523)
	at akka.stream.impl.fusing.GraphInterpreter.execute(GraphInterpreter.scala:390)
	at akka.stream.impl.fusing.GraphInterpreterShell.runBatch(ActorGraphInterpreter.scala:625)
	at akka.stream.impl.fusing.GraphInterpreterShell$AsyncInput.execute(ActorGraphInterpreter.scala:502)
	at akka.stream.impl.fusing.GraphInterpreterShell.processEvent(ActorGraphInterpreter.scala:600)
	at akka.stream.impl.fusing.ActorGraphInterpreter.akka$stream$impl$fusing$ActorGraphInterpreter$$processEvent(ActorGraphInterpreter.scala:769)
	at akka.stream.impl.fusing.ActorGraphInterpreter$$anonfun$receive$1.applyOrElse(ActorGraphInterpreter.scala:784)
sbt:sbt-5825-play-seed> 
[error] a.a.ActorSystemImpl - Internal server error, sending 500 response
akka.http.impl.util.One2OneBidiFlow$OutputTruncationException: Inner flow was completed without producing result elements for 1 outstanding elements
	at akka.http.impl.util.One2OneBidiFlow$OutputTruncationException$.apply(One2OneBidiFlow.scala:22)
	at akka.http.impl.util.One2OneBidiFlow$OutputTruncationException$.apply(One2OneBidiFlow.scala:22)
	at akka.http.impl.util.One2OneBidiFlow$One2OneBidi$$anon$1$$anon$4.onUpstreamFinish(One2OneBidiFlow.scala:97)
	at akka.stream.impl.fusing.GraphInterpreter.processEvent(GraphInterpreter.scala:523)
	at akka.stream.impl.fusing.GraphInterpreter.execute(GraphInterpreter.scala:390)
	at akka.stream.impl.fusing.GraphInterpreterShell.runBatch(ActorGraphInterpreter.scala:625)
	at akka.stream.impl.fusing.GraphInterpreterShell$AsyncInput.execute(ActorGraphInterpreter.scala:502)
	at akka.stream.impl.fusing.GraphInterpreterShell.processEvent(ActorGraphInterpreter.scala:600)
	at akka.stream.impl.fusing.ActorGraphInterpreter.akka$stream$impl$fusing$ActorGraphInterpreter$$processEvent(ActorGraphInterpreter.scala:769)
	at akka.stream.impl.fusing.ActorGraphInterpreter$$anonfun$receive$1.applyOrElse(ActorGraphInterpreter.scala:784)
sbt:sbt-5825-play-seed> playStop
Stopping server
[info] p.a.i.l.c.CoordinatedShutdownSupport - Starting synchronous coordinated shutdown with ServerStoppedReason reason and 35000 milliseconds timeout
[info] p.c.s.AkkaHttpServer - Stopping Akka HTTP server...
[info] p.c.s.AkkaHttpServer - Terminating server binding for /0:0:0:0:0:0:0:0:9000
[warn] a.a.CoordinatedShutdown - Task [shutdown-application-dev-mode] in phase [service-stop] threw an exception before its future could be constructed: Task java.util.concurrent.ScheduledThreadPoolExecutor$ScheduledFutureTask@1711291d[Not completed, task = java.util.concurrent.Executors$RunnableAdapter@300b27cd[Wrapped task = sbt.internal.TaskProgress$$Lambda$2471/0x0000000100d13040@4958dd1d]] rejected from java.util.concurrent.ScheduledThreadPoolExecutor@15e8e2eb[Terminated, pool size = 0, active threads = 0, queued tasks = 0, completed tasks = 250]
[info] p.c.s.AkkaHttpServer - Running provided shutdown stop hooks
[warn] a.a.CoordinatedShutdown - Task [shutdown-logger] failed in phase [before-actor-system-terminate]: Task java.util.concurrent.ScheduledThreadPoolExecutor$ScheduledFutureTask@4c8e2ed3[Not completed, task = java.util.concurrent.Executors$RunnableAdapter@418a785b[Wrapped task = sbt.internal.TaskProgress$$Lambda$2471/0x0000000100d13040@1ea7d93d]] rejected from java.util.concurrent.ScheduledThreadPoolExecutor@15e8e2eb[Terminated, pool size = 0, active threads = 0, queued tasks = 0, completed tasks = 250]
[success] Total time: 0 s, completed Sep 8, 2020, 9:34:06 PM
sbt:sbt-5825-play-seed> 
```
