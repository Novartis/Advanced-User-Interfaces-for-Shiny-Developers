# Advanced-User-Interfaces-for-Shiny-Developers
erum::Conf 2020 workshop session

by the Scientific Computing and Consulting Group, Novartis

-----

:spiral_calendar: May 30, 2020  
:alarm_clock:     09:00 - 17:00 (?)
:hotel:           @ Politecnico

-----


### Workshop Links

- :house: [Workshop Website - Coming soon]()
- :card_file_box: [Github](https://github.com/DivadNojnarg/Advanced-User-Interfaces-for-Shiny-Developers)
- :postbox: [RStudio Community thread - Coming soon](https://community.rstudio.com/)

-----


## Overview

In the past two years, there were various Shiny focused workshops introducing basic as well as advanced topics such as modules and Javascript/R interactions. However, handling advanced user interfaces was never an emphasis.   Clients often desire custom designs, yet this generally exceeds core features of Shiny. We recognized that R App developers lacking a significant background in web development may have found this requirement to be overwhelming. Consequently, the aim of this workshop is to provide participants the necessary knowledge to extend Shiny's layout, input widgets and include the new components in a novel modular framework. The workshop is organized into four parts. We first dive into the {htmltools} package, providing functions to create and manipulate shiny tags as well as manage dependencies. We then go through the basics of JavaScript, especially jQuery. Part 3 homes in on the development of a new template on top of Shiny by demonstrating examples from the [{bs4Dash}](https://github.com/RinteRface/bs4Dash) and [{shinyMobile}](https://github.com/RinteRface/shinyMobile) packages, part of the [RinteRface](https://rinterface.com) project. Finally, we integrate these new components into shiny modules, designed with an object-oriented-based package, namely [{tidymodules}](http://opensource.nibr.com/tidymodules/index.html). This novel approach allows the development of Shiny apps using R6 classes, thereby significantly reducing the burden of modular communication faced by classic shiny modules and their namespace management.


## Learning objectives

- Manipulate Shiny tags with {htmltools}
- Understand how dependencies are handled
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

During this tutorial you will need ... (Work in Progress)

[rstudio-desktop]: https://rstudio.com/products/rstudio/
[chrome]: https://www.google.com/chrome/

We will also set up a [RStudio Cloud](https://rstudio.cloud) dedicated project.


## Schedule

Below is the preliminary program, subject to changes by erum::Conf organisers. The time slots are still undefined since the global program is not available.

| Time          |                        | Activity                           |
| :------------ | ---------------------- | :----------------------            |
| (1h)          | :clapper:              | 1: Introduction to htmltools       |
| (15 min)      | :coffee:               | *Coffee break*                     |
| (1h)          | :nail_care:            | 4: Introduction to JavaScript      |
| (1h)          | :bento:                | *Lunch break*                      |
| (1h)          | :zap:                  | 3: Develop a custom shiny template |
| (15 min)      | :coffee:               | *Coffee break*                     |
| (2h)          | :globe_with_meridians: | 4: tidymodules                     |


### Detailed schedule

  - Introduction to {htmltools}
    * HTML 
    * Shiny's tags: structure (name, class, attributes, children, ...)
    * Manipulate tags: access/modifie/add the class, attributes, children
    * Introduction to HTML dependencies
    
  - Introduction to JavaScript for Shiny (preliminary)
    * Types
    * Functions
    * jQuery
    * Events
    * ...
    
  - Develop a custom shiny template (examples taken from [RinteRface](https://rinterface.com) templates)
    * Reminder on {shiny}'s dependencies (Bootstrap 3, 4, jQuery, ...)
    * Create new CSS/JS dependencies with {hmtltools}
    * Develop the template layout (navbar, sidebar, body, footer, ...)
    * Develop custom input widgets (how to input binding work?)
      * Basic description of the Shiny input binding utils
      * Describe how {shiny} deal with inputs
    * Test the newly created components
      * Unit tests with testthat
      * Testing JavaScript code
      * Other tests
      
  - Introduction to {tidymodules}
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

![](https://i.creativecommons.org/l/by/4.0/88x31.png) This work is
licensed under a [Creative Commons Attribution 4.0 International
License](https://creativecommons.org/licenses/by/4.0/).
