---
layout: post
title: Hello World!
---

I've chosen to create a blog on things I'm working on. My Hello World blog post will be about my journey to creating a Hello World page using [asciidoctor](https://github.com/asciidoctor/asciidoctor). I'm doing this on my Mac using VSCode, so the instructions will work for that primarily, but should be easily extended to other platforms. This blog is primarily to help me take notes and organize my thoughts. There may be others out there that find it useful. 

The following steps will walk you through my journey of a Hello World asciidoctor site. There is not a guarantee that this is the best way. This is just the way I did it - the first time! Also, Jekyll is only rendering my code block correctly sometimes, which angers me!
1. The first thing you need to do is install asciidoctor via brew -  `brew install asciidoctor` **note:** brew currently doesn't like macOS 11.0 and throws warnings. Hopefully this is fixed by the time anyone else tries this. 
2. I installed the ASCIIDoc 2.8.4 extension for VSCode. This enables an auto preview ability, but of course is not required. 
3. Create a test file in your working directory and name it HelloWorld.adoc. I used this code to create my first file and remember some syntax - feel free to copy it. 
   
~~~
= Hello World!
Ray Blaine <raymond.blaine@dontcall.me 
v1.0

== This is my first Asciidoctor file

TIP: You can find a lot more info on syntax https://asciidoctor.org/docs/asciidoc-syntax-quick-reference/[here!]

=== Things to do
. Get more familiar with syntax
.. that will be fun
. Practice!
. Learn more about css https://asciidoctor.org/docs/produce-custom-themes-using-asciidoctor-stylesheet-factory/[customization]


==== Code looks like this 
[source,python]
----
print(Hello world!)
----
~~~

4. If you want a custon CSS check out this [repository]((https://github.com/darshandsoni/asciidoctor-skins.git)) which I cloned (maybe I should've forked it) for cool ASCIIDoc skins.
   
5. If you put your chosen CSS in the same directory as your .adoc file you can run this code to generate you page `asciidoctor -a linkcss -a stylesheet=boot-cyborg.css  HelloWorld.adoc `. I don't like how this CSS renders the admonition, but that can be played with later. 
6. Now go work on creating somehting more useful! I will too :).

