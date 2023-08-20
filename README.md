# spring-ai-workshop
Workshop material for Spring AI

## Create an alias

```shell
source .devcontainer/scripts/postCreateCommand.sh
```

## Add exercises to the spring project catalog

```shell
spring project-catalog add azure-ai https://github.com/rd-1-2022/ai-azure-catalog
```

## Exercise #1 - Create the first Hello World project

```shell
spring boot new myai ai-azure-hello-world --package-name com.xkcd.ai
```

You will now have a project with the structure shown below

```shell
$ tree
.
├── mvnw
├── mvnw.cmd
├── pom.xml
├── README.md
└── src
    └── main
        ├── java
        │   └── com
        │       └── xkcd
        │           └── ai
        │               ├── Application.java
        │               └── helloworld
        │                   ├── Completion.java
        │                   └── SimpleAiController.java
        └── resources
            └── application.properties
```

## Exercise #2 - Prompt Templating

First clean up your build directory.

Now add the code for Prompt Templating

```shell
spring boot add ai-azure-prompt-templating
```

Now you will have the code added to your project for the Prompt Templating exercise.

Look at the `README-ai-azure-prompt-templating.md` file for instructions.

## Exercise #3 - ...

rinse, lather, repeat.




Follow the instructions in the `README.md` file for the exercise.



