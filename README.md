# play-java-ebean
let play2.x support ebean6.x

1、modify play project plugins.sbt
  // Comment to get more information during initialization
  logLevel := Level.Warn
  
  // The Typesafe repository
  resolvers += "Typesafe repository" at "http://repo.typesafe.com/typesafe/releases/"
  
  libraryDependencies ++= Seq("org.avaje.ebeanorm" % "avaje-ebeanorm-agent" % "4.5.3" exclude ("javax.persistence", "persistence-api"))
  
  // Use the Play sbt plugin for Play projects
  addSbtPlugin("com.typesafe.play" % "sbt-plugin" % "2.2.1")

2、change your project ebean dependent to this plugin :play-java-ebean_2.10
3、update your code support ebean6.1.1
