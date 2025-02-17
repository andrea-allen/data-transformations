# Basic Repo for working with Spark + Scala
The purpose of this repo is to make sure you have everything set up to build and run a spark project locally.

## Pre-requisites
Please make sure you have the following installed
* Java 8
* Scala 2.11
* Sbt 1.1.x
* Apache Spark 2.4 with ability to run spark-submit locally

## Setup for local building and testing
* Clone this repo
* Build: sbt assembly
* Test: sbt test

Please confirm that all of the tests pass.

## Setup for local run with spark-submit
After running ```sbt assembly``` from the root directory run
```
spark-submit target/scala-2.12/data-transformations-assembly-0.1.jar 
```
to run the spark job locally.

Confirm that you see "Hello Spark" in the output.

If all the test passed locally and "Hello Spark" was in the output than your environment is set up and ready for a TW Data Engineering coding interview.

~~*~~*~~*Andy Allen's fork~~*~~*~~*~~*
