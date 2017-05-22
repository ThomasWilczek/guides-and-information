# A guide to guide you writing guides

## Introduction

The introduction should contain a short overview, a little sneak peak to what
is about to come. It should only contain the most important points.

## The table of contents

Much like a books table of contents, but more detailed.
The style should look like this:

### 1. Feature/Idea
      1.1 What does it do?
        1.1.1 Why does it do?
      1.2 Variables
      1.3 Functions 
      1.4 Prototype (Can be in an extra file)
### 2. Another Feature
      1.1 Variables
      1.2 Todo

Much like this, it should not contain the real content only links 
to the information you desire, so it's easily reachable.
Try to give it an order that makes sense and mark things as incomplete.
It is okay to bring unfinished things to the table, but remember that none
of us can read minds.

## The content

The content should contain as much information as possible using as few
words as possible. For example:

### 1. Feature

#### What does it do?
     This function sets a ton of ants on fire and returns true if succesfull.

##### Why does it do that?
      The author doesn't like ants, also better working keyboard without ants
      in it.

#### Variables

     `int antAmount;` -- Contains the amount of ants available to burn
     `boolean bar;` -- Is set true if the ants burn correctly and will be
      returned

#### void foo()
     ```
     void foo() {
       if(antAmount !== 0) {
         bar = burnAnts(antAmount);
       }
     
     returns bar 
     }
     ```
## The summary

Sum up what happened and let people think about it. This part shouldn't take a
lot of information into account, only rehash what has been talked about before.
This guide is just meant as a quick overview, which might not suite all needs, 
but you are free to work on it as well.

