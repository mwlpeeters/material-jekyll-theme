---
layout: post
title: Building a Visual Studio Extension
description: Some basic prerequisites for building a Visual Studio extension
---

## End state

When you read this article you will end up with an Visual Studio solution that can be used to develop Visual Studio Extensions. Furthermore it will give you some tips of tools you might find useful during development.


## Introduction
In the next couple of months I will try to create some blog posts on this site about building Visual Studio Extensions for Visual Studio 2015.

So why would you create a Visual Studio extension? Well good question, I can only tell you why I would create an extension:

- To add features I'm missing (or simply cannot find)
- To automate anything that is repetitive
- Just because it can be done 


## Prerequisites

Here is a simple shopping list:

- Visual Studio 2015 with the ''Visual Studio Extensibility Tools''

This SDK is available in all Visual Studio editions except Express and since Visual Studio 2015 it can only be installed during the installation of Visual Studio itself.

![alt text][vs-setup]{: .small}

> Already installed Visual Studio? 
> Well you can alter it from the Apps & Features page in the Configuration Panel.

- A Visual Studio Extension called `Reset Experimental Instance`, you can find it [here](https://visualstudiogallery.msdn.microsoft.com/ca73dffb-0ab4-4b94-a45a-f288112120a3).
- ILSpy, for inspecting assemblies. Grab your copy from [here](http://ilspy.net/).
- LINQPad (optional), I really love this tool! For quick code snippets and inspecting objects this tool is a must! You'll find it [over here](https://www.linqpad.net/) 
- A lot of patience because sometimes not everything is documented that well or it's hard to find on the internet.


## Setting up the solution

1. Create a new project
2. In the template tree navigate to *Templates > Visual Studio C# > Extensibility*
![alt text][template-tree]{: .small}  
3. Select the `VSIX Project`
![alt text][project-type]{: .small}
4. Give the project (and solution) a name

You should now have a project which can be used to create Visual Studio Extensions.

![alt text][sample-solution]{: .small}



> TODO: I'm still working on this article, stay tuned


## See also
[Installing the SDK](https://msdn.microsoft.com/en-us/library/mt683786.aspx)

[vs-setup]: /images/2016-10-01-Building-A-Visual-Studio-Extension/setup.png "Visual Studio Setup"
[template-tree]: /images/2016-10-01-Building-A-Visual-Studio-Extension/template-tree.png "Template tree"
[project-type]: /images/2016-10-01-Building-A-Visual-Studio-Extension/project-type.png "VSIX Project Type"
[sample-solution]: /images/2016-10-01-Building-A-Visual-Studio-Extension/sample-solution.png "Sample solution"
