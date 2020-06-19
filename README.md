# Advanced-User-Interfaces-for-Shiny-Developers

by the Scientific Computing and Consulting Group, Novartis

-----

:spiral_calendar: June 20, 2020  
:alarm_clock:     13:30 - 17:00 
:hotel:           @ Remote

-----


## Overview

In the past two years, there were various Shiny focused workshops introducing basic as well as advanced topics such as modules and Javascript/R interactions. However, handling advanced user interfaces was never an emphasis. Clients often desire custom designs, yet this generally exceeds core features of Shiny. We recognized that R App developers lacking a significant background in web development may have found this requirement to be overwhelming. Consequently, the aim of this workshop is to provide participants the necessary knowledge to extend Shiny's layout, input widgets and include the new components in a novel modular framework. The workshop is organized into three parts. We first dive into the {htmltools} package, providing functions to create and manipulate shiny tags as well as manage web dependencies. Part 2 homes in on the development of a new template on top of Shiny by demonstrating examples from the [RinteRface](https://rinterface.com) project. Finally, we show how one may integrate these new components into shiny modules, designed with an object-oriented-based package, namely [{tidymodules}](http://opensource.nibr.com/tidymodules/index.html). This novel approach allows the development of Shiny apps using R6 classes, thereby significantly reducing the burden of modular communication faced by classic shiny modules and their namespace management.


## Learning objectives

- Manipulate Shiny tags with {htmltools}
- Understand how web dependencies are handled
- Discover the steps to create a new template from scratch
- Learn how shiny deals with inputs
- Discover a new framework for robust module development


## Prerequisite

- Be familiar with Shiny, modules
- Basic knowledge in HTML and JavaScript is a plus


## Is this course for me?

You should take this course if you answer yes to at least 2 of the following questions:

  - Do you want to know how to develop outstanding shiny apps?
  - Have you ever wondered how to develop new input widgets?
  - Are you bothered by the cumbersomeness of module communication in vanilla Shiny?
  - How would you manage an app with 150 tightly connected modules?


## Workshop Preparation

- Project: [rstudio-cloud](https://rstudio.cloud/project/1395473)
- Recommanded web browser: [chrome](https://www.google.com/chrome/)
- Resources: [Outstanding User Interfaces for Shiny ](https://divadnojnarg.github.io/outstanding-shiny-ui/)
- tidymodules documentation: [pkgdown website](https://opensource.nibr.com/tidymodules/)

## Schedule

Below is the preliminary program, subject to changes by erum::Conf organisers. The time slots are still undefined since the global program is not available.

| Time          |                        | Activity                           |
| :------------ | ---------------------- | :----------------------            |
| (50min)       | :zap:                  | 1: Shiny: under the hood           |
| (5 min)       | :coffee:               | *Coffee break*                     |
| (1h)          | :zap:                  | 2: Develop a custom shiny template |
| (10 min)      | :coffee:               | *Coffee break*                     |
| (1h)          | :zap:                  | 3: tidymodules                     |


### Detailed schedule

  - Workshop introduction
    * Presentation
    * Quiz: Shiny or not Shiny?
    * Workshop motivations and agenda
  
  - Part 1. Shiny: under the hood
    * Chapter 1: What's behind a Shiny app?
      * Shiny generates HTML from R (Exercise)
      * Shiny dependencies
      * Quick introduction to HTML
        * HTML tags
        * HTML attributes
        * The document object model (DOM)
        
    * Chapter 2: Manage web dependencies with {htmltools}
      * Include CSS and JS, the dirty approach
      * Creating web dependencies
      * Attach web dependencies
      * Exercises
      
    * Chapter 3: From HTML to R
      * Tag structure
      * Exercise 1
      * Add/replace children
      * Tips
      * Exercise 2
  
  - Part 2. Practice: implementation of the Tabler Boostrap 4 dashboard template
    * How do we proceed?
    * Chapter 1: Import web dependencies (exercise step 1)
    * Chapter 2: Create template elements (exercise step 2)
    * Chapter 3: Create new inputs
      * JavaScript
        * Define variables
        * Objects
      * jQuery: "Write less, do more"
        * Selectors
        * Event listeners
        * Exercise
      * Binding Shiny inputs
        * Finding inputs
        * Exercise 
        * Conclusion
      
  - Part 3: Introduction to {tidymodules}
    * Introduction to R6: object oriented programming key concepts
    * Reminders on classic shiny modules: what are the main drawbacks?
    * {tidymodules}
      * Modules definition
        * Inheritance set up
        * Initialize input and output ports
        * Create ui and server methods
        * Other methods
      * Nested modules
      * Module communication
        * Input inheritance (between nested and parent modules)
        * Port forwarding
        * Tidy operations between modules
      * Handle multiple user interfaces
      * Manage module: the ModStore
        * visNetwork representation


## Instructors

Mustapha Larbaoui and David Granjon are respectively, associate director and principal scientist and consultant at [Novartis](https://www.novartis.com) where they use and trains others to use R, Shiny...

[blog]: https://www.novartis.com
[github]: https://github.com/DivadNojnarg
[twitter]: https://twitter.com/divadnojnarg

-----

Copyright 2020 Novartis AG

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
