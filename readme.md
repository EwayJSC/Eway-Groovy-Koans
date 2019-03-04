## Groovy Koans Project ##

The Groovy Koans project is a collection of small exercises in the form of unit tests, designed to get Java
developers up to speed on Groovy features and common idioms. It starts by teaching you basic Groovy building
blocks, and gradually builds your knowledge towards metaprogramming, slurpers, and all the goodness Groovy has
to offer.

## Getting Started ##
1.  Make sure you have [JDK 1.6+][jdk] installed 
2.  Download and unzip the [Koans][zip] (or clone the GitHub repository with `$ git clone https://github.com/nadavc/groovykoans.git`)
3.  Remove the solutions from the Koans using `$ ./gradlew removeSolutions`
4.  Execute Koan01 with `$ ./gradlew koan01` and fail (or any other Koan using `$ ./gradlew koan##`)
5.  Fix code, and execute again
6.  Keep going until you're fluent at Groovy :)

## Q&A ##

#### I like IntelliJ. How can I use it to debug/edit the Koans? ####

* Download and install [IntelliJ IDEA Community Edition][ideac]
* In IDEA, `File -> Open Project` and open the `build.gradle` file

#### I like Eclipse. How can I use it to debug/edit the Koans? ####

* Execute `./gradlew eclipse`
* Download and install [Eclipise IDE for Java Developers][eclipse]
* In Eclipse, `File -> Import...`, `Existing Projects into Workspace`, and select the project directory

#### I am forced to work behind a proxy. Can I still run the Koans? ####

The `gradlew` script downloads Groovy and Gradle for you, so you don't have to set up anything by yourself.
To allow gradlew to work through your proxy, simply add the following parameters:
```
$ ./gradlew koan01 -Dhttp.proxyHost=[http proxy] -Dhttp.proxyPort=[http proxy port]
```

#### The answers are already there! What's the point?  ####

One of the perks of learning through Koans is that once your Koan is solved, you can compare your solution with
the 'official' solution and perhaps learn from that comparison as well. It is also a way to make sure that the Koans
are indeed solvable by filling in the blanks.

For optimal learning experience, however, you should first try to solve the Koans without those solutions as reference.
To remove the solutions, run `$ ./gradlew removeSolutions` from the root of your unzipped Koans.

#### Are there more Koans planned? How will I know? ####

These are the Koans that are currently planned: 
* Embedding Groovy
* Creating your own DSL
* Creating your own builder
* Transformations
* GPars

Folk from: https://github.com/nadavc/groovykoans