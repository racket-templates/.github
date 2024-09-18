# Racket templates

The Racket Templates project provides the `raco new` tool and a collection of templates so you can quickly get started with a new project. 

This is a command line tool! Please remember to configure your command line for Racket. We haven't created support for creating new projects from templates using DrRacket, Vim, or [Racket Mode(https://racket-mode.com) for Emacs, but we would like to do so.

The new command is inspired by the [`dotnet new <TEMPLATE>`](https://learn.microsoft.com/en-us/dotnet/core/tools/dotnet-new) command, but provides the new template capability for the [Racket](https://racket-lang.org) ecosystem.

We currently support templates hosted on GitHub or Gitlab, but we are happy to add others if you prefer to host your template on another service.

## installing the `new` command 
Using existing templates is easy. Just install the package `new`: 
```
raco pkg install new
```

## Select a template
You can view all available templates in this repository in the `templates` directory, or you can 
search them in your command line by doing 
```
raco new --list
```
to see all available templates.


## Install a template and get started

Then you can download any template you want by running 
```
raco new <template-name> <optional-folder-location>
```


# Contribute
The Racket community welcomes all sorts of contributors. And there are many ways to contribute

## Ask questions
Asking questions is welcome - no question is too simple - asking 'so-called' obvious questions help us identify gaps in the documentation and usability of the tools and templates. 

* [Discourse](https://racket.discourse.group/invites/VxkBcXY7yL) and [Discord](https://discord.gg/6Zq8sH5)
* Creating a new issue at [racket-templates/new](https://github.com/racket-templates/new/issues/new)
* Create a new issue on the template repository directly. 

## Answering questions

Yes please! Answering questions on [Discourse](https://racket.discourse.group/invites/VxkBcXY7yL) and [Discord](https://discord.gg/6Zq8sH5) on in issues is most welcome.

## Report a bug

Just like asking a question! Create an issue in  [racket-templates/new](https://github.com/racket-templates/new/issues/new), the template repository where you identified  the bug. If are not sure how to do this or which is the right place, it is fine to let us know via the Racket [Discourse](https://racket.discourse.group/invites/VxkBcXY7yL) or [Discord](https://discord.gg/6Zq8sH5).

## Fix a bug

You are awesome and we love you. Seriously. If you know how to create a pull request that is great, but if you are not sure it is fine to let us know via the Racket [Discourse](https://racket.discourse.group/invites/VxkBcXY7yL) or [Discord](https://discord.gg/6Zq8sH5).


## Submitting a new template

You've created a new template you want to share with the Racket Community? 
Please submit a pull request to add a short configuration file describing 
your template and where to find it to the [racket-templates](https://github.com/racket-templates/racket-templates/tree/main/templates) 
folder in repository [racket-templates](https://github.com/racket-templates/racket-templates/). (I think we need to rename that repository as that name is a little confusing)

Your pull request should contain a single file with the name of 
your template, with the following contents:
```scheme
(name <name of template>
 repo username/repo-name
 from [github|gitlab]
 desc "A short description of your template.")
```

A good example is [Rosette](https://github.com/racket-templates/rosette-template): 
```
(name rosette
 repo "racket-templates/rosette-template"
 from github
 desc "A #lang rosette template for program verification and synthesis.")
```
