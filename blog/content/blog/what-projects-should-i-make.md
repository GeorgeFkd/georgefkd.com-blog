+++
date = 2026-09-26T13:43:30+03:00
draft = true
title = 'What Projects Should I Make'
tags = ['early career']
+++


### TODOS

- Research Hardware stuff
- Find algorithm categories for the mathy stuff section
- Find resources for devops.

### Introduction

This is addressed mostly to beginners/juniors. People with industrial experience can skip to the [domain specific section](#domain-specific-recommendations) for ideas. This article will be expanded the more I learn new things.

### General Advice across domains

- Ideally pick something you would personally use(not something that is necessarily useful to other people).
- Make a smaller version of something open-source or proprietary you use. Choose a subset of features you are going to implement.
- Implement something open source in a different language.
- You can build anything in any programming language you want.
- Implement something simple/something you have already done in a new language you want to learn.
- Find something in a domain you are already interested in and would want your career to revolve around it.
(Personally it is dev-tools and software quality/testing related tooling)
- Set a clear finishing line, this is important. Cross it once you are comfortable.
- Make simplifying assumptions so you can actually finish it.
- Write developer and user-facing docs(Will teach you how to write concisely while targeting a specific demographic).
- How to use AI here.
(As a guidance, write code by hand, do not let it overtake your project, ask it why things are written the way they are, dont use agents or dont let them write the code)

### Domain-specific recommendations

I should point to existing resources/books for each of the domains.(Books can be bought by PDFs for faster and easier access).

I will analyse each of the category to give a bit of the map of each domain as I currently see it,
and the programming languages I would recommend for each(disclaimer you can write everything with anything, pick the language according to where you wanna head towards regarding software domains).
Make small ones from each to discover what you like.

#### Mathy stuff

Leetcode implement generally useful algorithms + Implement algorithms/data-structures specific to a domain you like(I will find some that)
and provide some categories for things. Graph algorithms, advanced tree structures, statistics calculations.

#### Distributed systems

A file syncer teaches lots of fundamentals and can take you as far as you are willing to. There are plenty of features to implement across different software topics(encryption, microservices, versioning in distributed environments).
It is also a great project for really getting comfortable with multithreading and async computations.
A recommended resource to get more advanced and senior is [Designing Data-Intensive Applications by Martin Kleppmann](https://dataintensive.net/). Would suggest it for later, after creating a couple projects or getting far in this project. It helps with system design and understanding problems faced in larger scales and how they are handled.

#### Programming Languages

Before doing an actual project read more on how compilers are structured, what they really do and how(a recommended resource is [this section from crafting interpreters](https://craftinginterpreters.com/a-map-of-the-territory.html)). No need to dive too deep at this point. Then you can implement a simple parser/compiler, as a warming up project you can implement the compiler written in Java from [CraftingInterpreters](https://craftinginterpreters.com/). It is a quality resource for starting the compiler journey with reduced difficulty because the author,Robert Nystrom, introduces and explains code gradually and meticulously. Investigate what part of the compiler mostly interests you.

After learning the basics and having an overview of what components a compiler consists of, you can move to more specific
tooling. If creating tooling around the language and parser is what you prefer, a tool like [Treesitter](https://tree-sitter.github.io/tree-sitter/) can be something interesting to poke around.
It generates the parser for the language you want, and on top of it you can implement the specific things you want to implement(e.g. an imports viewer for Java projects). It is also used in [Neovim](https://neovim.io/) which can help you integrate with an IDE.

If you want to go for lower-level,assembly related stuff there is LLVM which is heavy-duty and needs a significant time
investment to start being productive and creating realistic things.

#### Hardware/Embedded devices and IoT(Internet of things)

#### Web App/Enterprise stuff

Client management system/Something inventory related(for sth you are specifically interested in, e.g. card game collections). Java/C# and a frontend framework(Vue,React,Angular).
In this domain it is valuable to be aware of what the framework offers, because most needed stuff are already semi-implemented there(for example spring boot integrates with probably anything you will ever need when building an Enterprise app).
Learn about architectural patterns such as SOLID, Hexagonal architecture,Domain Driven Design etc. etc. It is favorable to do things in a domain you are practically knowledgable about so you can model things based on how they really are.

#### Mobile Apps Development

It is easy to find something you already want to build. Maybe for a board game or a card game you are playing that could be made easier with an app, maybe for tracking something specific in your life. Maybe an app you find really hard to use and overloaded with features you can make a smaller version that is more focused and appealing to you.

When researching mobile apps development tools and libraries one core decision is whether you will make an app that works unchanged in both Android and iOS(cross-platform tooling) or only target one and use its dedicated tooling for deeper integration with the device(Native tooling).

++language specific stuff I wont write right now, and the iOS problem(you need a mac to develop for it, and a dev subscription to install something on a physical device).

#### Graphics and games

If you want to do more game design(which is less technical software wise) use an engine(Unity,Unreal Engine), otherwise implement some simple rendering yourself, starting with [OpenGL](https://www.opengl.org/), using the tutorials from [learnopengl.com](https://learnopengl.com/). There is also [Vulkan](https://vulkan.org/) for working with GPUs, it is really low-level, really performant and widely used in games and general purpose GPU programming.
Some talk about the different graphics APIs and their difficulty levels. Choose 2D or 3D they are similar in difficulty and there are many methods to choose from.

#### Devops,Linux, System Administration

Self hosting in a home server, Docker/Kubernetes knowledge, Terraform, Cloud platforms. Find resources for such things.Ansible.
Start daily-driving a linux desktop. Make your setup reproducible through ansible.
