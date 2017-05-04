## Available Projects for Scala 2.13.0-M1

Library maintainers, library users, please [edit this page](https://github.com/scala/make-release-notes/edit/2.13.x/projects-2.13.md) and let the world know what libraries are available.

<!--
### Scaladex

Scaladex, the index of Scala libraries, now offers searching by target version:

********** THESE LINKS WON'T DISTINGUISH M1 FROM M2 ONCE M2 COMES OUT
********** reported upstream: https://github.com/scalacenter/scaladex/issues/411

* [Scala modules for 2.13.0-M1](https://index.scala-lang.org/search?scalaVersions=2.13&q=*+AND+organization%3Ascala)
* [Testing frameworks for 2.13.0-M1](https://index.scala-lang.org/search?scalaVersions=2.13&keywords=testing)
* [Other libraries for 2.13.0-M1](https://index.scala-lang.org/search?scalaVersions=2.13)
* [Compiler plugins for 2.13.0-M1](https://index.scala-lang.org/search?scalaVersions=2.13&keywords=compiler-plugin)
* [Sbt plugins for 2.13.0-M1](https://index.scala-lang.org/search?scalaVersions=2.13&keywords=sbt-plugin)
-->

### Scala modules

Add in sbt using `libraryDependencies += ...`:

    "org.scala-lang.modules"           %% "scala-parallel-collections" % "0.1.2"
    "org.scala-lang.modules"           %% "scala-parser-combinators"   % "1.0.6"
    "org.scala-lang.modules"           %% "scala-swing"                % "2.0.0"
    "org.scala-lang.modules"           %% "scala-xml"                  % "1.0.6"

The remaining modules (scala-java8-compat, scala-async) will be published shortly.

### Testing frameworks

Add in sbt using `libraryDependencies += ... % "test"`:

    "org.scalacheck"                   %% "scalacheck"                % "1.12.6"          % "test"
    "org.scalacheck"                   %% "scalacheck"                % "1.13.4"          % "test"
    "org.scalacheck"                   %% "scalacheck"                % "1.13.5"          % "test"
    "org.scalatest"                    %% "scalatest"                 % "3.0.3"           % "test"

### Other libraries

Add in sbt using `libraryDependencies += ...`:

    "com.chuusai"                      %% "shapeless"                 % "2.3.2"
    "org.scalactic"                    %% "scalactic"                 % "3.0.3"           % "test"
    "org.scalaz"                       %% "scalaz-core"               % "7.2.11"
    "org.typelevel"                    %% "macro-compat"              % "1.1.1"

### Compiler plugins

Add in sbt using `addCompilerPlugin(...)`:

    "org.scala-lang.plugins"           %% "scala-continuations-plugin" % "1.0.3"  cross CrossVersion.full
    "org.scalamacros"                  %% "paradise"                   % "2.1.0"  cross CrossVersion.full
    "com.typesafe.genjavadoc"          %% "genjavadoc-plugin"          % "0.10"   cross CrossVersion.full

### sbt plugins

Most plugins do not need to be re-published for 2.13, but certain plugins did require changes.

Add using `addSbtPlugin(...)`:

    "org.scala-js"                     % "sbt-scalajs"                % "0.6.16"

### Pending

You can subscribe to these tickets to find out when a library you want becomes available:

* [cats](https://github.com/typelevel/cats/issues/1648)
* [kind-projector](https://github.com/non/kind-projector/issues/50)
* [machinist](https://github.com/typelevel/machinist/pull/16)
* [pcplod](https://github.com/ensime/pcplod/issues/22)
* [specs2](https://github.com/etorreborre/specs2/issues/573)