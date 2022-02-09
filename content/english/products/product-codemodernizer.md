---
date: "2021-07-14"
draft: false
title: "CodeModernizer"
description: "Longer lasting code"
#icon: "fas fa-users"  # fontawesome icon pack : https://fontawesome.com/icons/


######################### banner #####################
banner:
  title: "CodeModernizer"
  image: "images/undraw/undraw_version_control_re_mg66.svg"
  content : "CodeModernizer is a software tool that employs semi-automated techniques to evolve your Java code over time"
  button:
    enable : true
    label : "Try for Free"
    link : "get-demo/"
  background_class: "bg-light"


######################### about this product #####################
about_this_product:
  enable: true
  title: "The software with consultancy, <br> or on its own with a little bit of work"
  content: "CodeModernizer is available to [buy](pricing/) as a product that can be used without our assistance, but a little work will be necessary to get it fully functioning. If you want our knowledge and experience in combination with CodeModernizer, you can also opt for [consultancy](consulting/) from us."
  background_class: ""

  features:
  - title: "Why buy CM?"
    icon: "fas fa-question"
    content: "Even when your software base is stable, its dependencies continue to evolve. The environment of software runs the language, the JDK, the operating system, the underlying virtualization and hardware, and they all continue to evolve time. However, there are clear dangers that come with freezing your code in time (because, why touch it if it isn’t broken?):

- The older the code becomes, the higher the cost when an eventual refactoring has to happen anyway.

- The older the code becomes, the less coders will be familiar with its dependent libraries and its language constructs.

- At some point, some dependency may break backwards compatibility, and then you’re forced to modernize, usually at an inconvenient time.

With CodeModernizer, your software assets evolve with their environment and the current breed of coders, their knowledge, and their expectations.
    "

  - title: "What does CodeModernizer do?"
    icon: "fas fas fa-project-diagram"
    content: "CodeModernizer modernizes the following aspects of your code:

1. Language constructs, as the language continues to evolve

2. Use of the latest JDK features

3. Use of recent versions of dependent libraries

4. Use of up-to-date build scripts

<br><br>

Before any of the first three can run, the code is regularized. This means that irregular constructs, which can generally be viewed as “sloppy programming”, are transformed to more conventional ones."

      
######################### product_info #####################
product_info:
  enable : true
  title: "Which steps does CodeModernizer follow to update your code?"
  content: ""
  background_class: "bg-light"
  features:
  - image: "images/undraw/undraw_code_inspection_bdl7.svg"
    content : "##### Topic 1: Regularization

      A first round of transformations concerns regularization. None of these change the semantics of the code, obviously, but all of them generally improve the legibility, and make it easer to recognize the statements’ intention for a coder.

      Furthermore, these transformations are critical to the next sets of transformations, as the transformation templates assume regularized code.

      We refer to our page with [technical details](technical-details/) for an overview of the more common regularization steps.

    <br><br>

    ##### Topic 2: Modernize language constructs

      The Java language evolved over its 20+ years of existence, with the introduction of the for-each construct, generics, lambda’s, try-with-resource, records, etc. The target of modernization is to be agreed with the client, but will generally be either Java 8 or Java 16.

      Some examples:

      - for-each should substitute old-style enumerations and for-loops wherever possible

      - introduction of generics in very old style Object+cast usage

      - introduction of try-with-resource where still missing

      - use of streams to replace regular loop operations

      - use of instance-of patterns to avoid costs

      - ...


      Again, we refer to the [technical details](english/technical-details/) for an overview of the more common regularization steps.
    "

  - image: "i"
    content : "##### Topic 3: Use of the latest JDK


    CodeModernizer makes sure your code isn't dependent on an old JDK by making sure the latest JDK is used.

    Some examples include:

    - Phase out any collections framework for the unmodifiable collections in the JDK

    - JDK 16 has introduced a “toList” method on streams, saves a call to “collect”

    - the JDK now includes an HTTP client, which can replace e.g. the Apache HttpCommons library

    - JodaTime has been incorporated as the java.time package

    <br><br>

    ##### Topic 4: Dependent libraries

    There are thousands of open source Java libraries around, hundreds of which enjoy a high popularity. We cannot list all of them here, but chances are that your software is dependent on at least a dozen of these libraries, or more. CodeModernizer will ensure use of the most recent versions of these dependent libraries, so that [.... → throw in example of log4j server crash]

    Typical examples that will recur are

    - Move to SLF4J, the most popular logging framework

    - Move to JUnit 5 from the popular earlier versions JUnit 3 and JUnit 4

    - Move to the latest version of the Spring Framework

    - Some lib [????]
    "




      
######################### content_and_image_ordered #####################
content_and_image_ordered:
  enable : true
  block:
  - title : "For whom?"
    background_class : "bg-white"
    images:
    - "images/service-1.png"
    - "images/service-2.png"
    - "images/service-3.png"
    content : "Those who will gain the most benefit out of using CodeModernizer are companies who own a Java software base that is valuable to them, one they intend to continue to use for many years to come.

    The service is especially interesting to those who cannot afford or do not want to assign programmers to do regular maintenance on the code. In a time where coders are in high demand, you would rather have them implement new features instead of keeping the Java software base modern and up-to-date."
      
  - title : "What is not?"
    background_class : "bg-light"
    images:
    - "images/service-1.png"
    content : "CodeModernizer will not set out to structurally improve your code. Its transformations may recognize some dangerous constructs and replace them with better choices, but as a general rule, the semantics and organization of the code remain untouched.

    Neither does CodeModernizer act as a service or consultancy to add unit tests, do bug fixing, improve performance, or extend the application with new features."
      
  - title : "Is it safe?"
    background_class : "bg-white"
    images:
    - "images/service-2.png"
    content : "Will my code still run after the transformation? While the transformations are as “safe” as possible, the language is so rich that we cannot rule out occasional problems. This is where your unit tests come in.

    <br><br>

    CodeModernizer will guarantee that any test that it can execute during its quality control process, will remain green. This leaves the situation where your code does not have sufficient unit tests to cover the transformed code. We can automatically identify which transformations took place “untested”.

    <br><br>

    A second set of correctness guarantees are the annotation computed by the [e2immu.org](http://e2immu.org/) static code analyzer. This analyzer determines critical properties of your code’s methods and classes. These properties have to remain invariant."
      
  - title : "Is it secure?"
    background_class : "bg-light"
    images:
    - "images/service-3.png"
    content : "There are generally two components to the CodeModernizer service: a **code transformer and a standard transformation library**, and **custom work for your specific combination of libraries**.

    <br><br>

    Part one you can run using our binary, locally inside your own organization. That means that IBTECH does not have to have a view on your code. The binary writes to a different branch of the source code management system, and we guarantee that the binary does not communicate over the internet, so your code is as secure as it can be.

    <br><br>

    Part two generally requires IBTECH to have a view on those parts of the code that need modernizing. A non-disclosure agreement will be signed if such a view is to be granted."

  - title: "Will I still recognize the code?"
    background_class: "bg-white"
    images:
    - "images/service-2.png"
    content: "An important topic in source code transformations is formatting.

    Transformers generally mess up existing formatting; comments in the code may go missing, become irrelevant, move to the wrong place, etc. CodeModernizer does a best effort here; generally, though, the effect is greater standardization, a benefit to your code base."

  - title: "The process with just the software or consulting?"
    background_class: "bg-light"
    images: 
    - "images/service-1.png"
    content: "CoderModernizer is a downloadable product, that can be used independently However, if you and/or your company feel like consultancy from IBTECH would be beneficial, you can get in contact with us."
    button:
      enable : true
      label : "Contact us"
      link : "contact/"

      
######################### CTA #####################
cta:
  enable : true
  title : "Start using CodeModernizer to keep your Java codebase up to date, today."
  content : "Try CodeModernizer for free or choose the pricing plan that best applies to you!"
  background_class: ""
  button:
    enable : true
    label : "Pricing plans"
    link : "pricing/"

---

######################### Intro Video #####################
intro_video:
  enable: true
  title: "Check out our video preview"
  content: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi egestas Werat viverra id et aliquet. vulputate egestas sollicitudin."
  video_url: "https://www.youtube.com/embed/dyZcRRWiuuw"
  video_thumbnail: "images/products/02.jpg"
  background_class: ""