# spring-ai-workshop
Workshop material for Spring AI

The workshop uses the Spring CLI project.  If you are not using GitHub codespaces, [download the Spring CLI](https://github.com/spring-projects-experimental/spring-cli/releases).
You can browse the [Spring CLI Documentation](https://docs.spring.io/spring-cli/reference/0.7-SNAPSHOT/index.html) to learn more about its features.

A quick summary is that the Spring CLI provides a command line application named `spring`

You will create the code for Exercise #1, the "Hello World" AI project,  using the command `spring boot new`.  See below.

The code for additional exercises will use the command `spring boot add`

To access the projects used in these exercises, we first need to add the `ai-azure-catalog`.


You will also need to have the `curl` like tool [httpie](https://httpie.io/docs/cli/installation) installed.

Now, let's get started!

## Add exercises to the spring project catalog

```shell
spring project-catalog add azure-ai https://github.com/rd-1-2022/ai-azure-catalog
```

## Exercise #1 - Create the first Hello World project

Create a new project using the following command.  You can pick a different 

* name:  The following example uses the name `myai` as the project name
* package name:  The following example uses the name `com.xkcd.ai` in honor of [XKCD](https://xkcd.com/).  

```shell
spring boot new myai ai-azure-hello-world --package-name com.xkcd.ai
```

You will now have a project with the structure shown below


```shell
cd myai
```

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

Follow the instuctions in `README.md` to complete the exercise.

## Exercise #2 - Prompt Templating

** MAKE SURE YOU ARE IN THE ROOT OF THE JAVA PROJECT **

Now add the code for Prompt Templating

```shell
spring boot add ai-azure-prompt-templating
```

Look at the `README-ai-azure-prompt-templating.md` file for instructions.

Your directory tree should look like:

```shell
$ tree
.
├── mvnw
├── mvnw.cmd
├── pom.xml
├── README-ai-azure-prompt-templating.md
├── README.md
└── src
    └── main
        ├── java
        │   └── com
        │       └── xkcd
        │           └── ai
        │               ├── Application.java
        │               ├── helloworld
        │               │   ├── Completion.java
        │               │   └── SimpleAiController.java
        │               └── prompttemplate
        │                   └── PromptTemplateController.java
        └── resources
            ├── application.properties
            └── prompts
                └── joke-prompt.st
```

## Exercise #3 - Prompt Roles

Now add the code for the Prompt Roles exercise.

```shell
spring boot add ai-azure-prompt-roles
```

Look at the `README-ai-azure-prompt-roles.md` file for instructions.


## Exercise #4 - Output Parser

Now add the code for Output Parser exercise.

```shell
spring boot add ai-azure-output-parser
```

Look at the `README-ai-azure-output-parser.md` file for instructions.

## Exercise #5 - Chains

Now add the code for Chains exercise.

```shell
spring boot add ai-azure-chains
```

Look at the `README-ai-azure-chains.md` file for instructions.


## Exercise #6 - Stuff the Prompt

Now add the code for the Stuff the Prompt exercise.

```shell
spring boot add ai-azure-stuff-prompt
```
Look at the `README-ai-azure-chains.md` file for instructions.

## Exercise #7 - Retrieval Augmented Generation

Now add the code for the Retrieval Augmented Generation exercise.

```shell
spring boot add ai-azure-rag
```
Look at the `README-ai-azure-retrieval-augmented-generation.md` file for instructions.
