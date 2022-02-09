---
date: "2021-07-13"
draft: false
title: "Consulting"
description: "Expert knowledge for evolving your codebase"
#icon: "fas fa-dice-d6"  # fontawesome icon pack : https://fontawesome.com/icons/


######################### banner #####################
banner:
  title: "Consulting Services"
  image: "images/products/02.jpg"
  content : "Let us update and evolve your codebase with the use of CodeModernizer and years of experience with software development in Java."
  button:
    enable : true
    label : "Contact us"
    link : "contact/"
  background_class: ""

      
######################### product_info #####################
product_info:
  enable : true
  title: "The process if you opt for colsuntancy"
  content: "The software that can be run on its own in a user-friendly way is still in development. However, with if you opt for consultancy you can already reap the benefits of CodeModernizer for your organization’s code base."
  background_class: "bg-light"
  features:
  - image: "images/products/01.jpg"
    content : "##### Step 1: study round


    1. Signing of an NDA

    2. Offer a view of the code to IBTECH. If dependencies are proprietary, some view on at least the API docs of those dependencies needs to be granted

    3. IBTECH compiles a dependency report

    4. IBTECH makes suggestions on what to modernize
    "

  - image: "images/products/02.jpg"
    content : "##### Step 2: agreement on transformations and cost determination

    1. Agreement on transformation menu

    2. Cost per transformation, in function of the amount of interaction with the library or the number of constructs involved

    3. Determination of a delivery timeline

    4. Determination of a way of how unit tests can be run. Generally IBTECH can run tests that do not require dependent resources such as databases etc. IBTECH may have to be given a way of remotely running tests if these resources cannot be made accessible.

    <br><br>
    
    ##### Step 3: stepwise transformations

    Each of the agreed transformations are carried out, successively.

    The result of each transformation is stored in a separate branch; we can go down to the more granular level of class-file based branches, to facilitate accepting or rejecting (and debugging issues of) individual transformations."

      
######################### content_and_image_ordered #####################
content_and_image_ordered:
  enable : true
  block:
  - title : "Is it safe?"
    background_class : "bg-white"
    images:
    - "images/service-1.png"
    - "images/service-2.png"
    - "images/service-3.png"
    content : "Will my code still run after the transformation? While the transformations are as “safe” as possible, the language is so rich that we cannot rule out occasional problems. This is where your unit tests come in.

    <br><br>

    CodeModernizer will guarantee that any test that it can execute during its quality control process, will remain green. This leaves the situation where your code does not have sufficient unit tests to cover the transformed code. We can automatically identify which transformations took place “untested”.

    <br><br>

    A second set of correctness guarantees are the annotation computed by the [e2immu.org](http://e2immu.org/) static code analyzer. This analyzer determines critical properties of your code’s methods and classes. These properties have to remain invariant."
      
  - title : "Is it secure?"
    background_class : "bg-light"
    images:
    - "images/service-1.png"
    content : "There are generally two components to the CodeModernizer service: a **code transformer and a standard transformation library**, and **custom work for your specific combination of libraries**.

    <br><br>

    Part one you can run using our binary, locally inside your own organization. That means that IBTECH does not have to have a view on your code. The binary writes to a different branch of the source code management system, and we guarantee that the binary does not communicate over the internet, so your code is as secure as it can be.

    <br><br>

    Part two generally requires IBTECH to have a view on those parts of the code that need modernizing. A non-disclosure agreement will be signed if such a view is to be granted."
        

      
######################### CTA #####################
cta:
  enable : true
  title : "Contact us for consulting"
  content : "Get in contact with us to discuss how we can help the codebase of your organization evolve"
  background_class: ""
  button:
    enable : true
    label : "Contact us"
    link : "contact/"

---