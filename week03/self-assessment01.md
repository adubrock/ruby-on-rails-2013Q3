*Portland Code School*
#Self-assessment opportunity: Ruby

This is a way for you to find out how much you know about ruby and to learn some new things on your own using personal research techniques.

##How to perform this self-assessment

The essential challenge: Answer the questions below *by yourself*. Do not ask your classmates, your mentor, the IRC channel, a mailing list, or any other human. Look it up and *read* things to find the answers. Unlike the code challenges, this particular aspect of the class is not a team sport. Some aspects of programming are solitary and non-verbal and this is one of them.

You may use any reference book, library, web site, or search engine you like. In fact, most questions require you to support your answer with a reference (book & page or URL). Please do not use videos or screencasts as references. Give me something I can read quickly and I don't have to sit around and watch.

You may not be able to answer all the questions yourself. You aren't being graded by me on this, but you should know all of this by this point in the class. If you don't, think of this as just another homework assignment. After the deadline, we'll discuss the self assessment as a team and you'll be able fill in any gaps.

##How to submit your self-assessment
Make a copy of the markdown source file of this page. Fill in your answers among the questions. Use markdown syntax. Format your answers so that they are easy to distinguish from the questions using indentation, font choice, or some other means. Email the markdown file as text (not as an attachment) to azimmerman@portlandcodeschool.com **before midnight Pacific time, Saturday**. I will review your answers and email you feedback on Sunday and we'll discuss them as a class on next Monday.

##Questions

#### What is the difference between ruby v1.9.3 and v2.0.0?

0. Provide a URL reference to a written description of the changes. Usually, this is on some sort of official site and is called "release notes" but it could also be your favorite article or blog posts that does a good job of describing the changes.

*[https://www.ruby-lang.org/en/news/2013/02/24/ruby-2-0-0-p0-is-released/](https://www.ruby-lang.org/en/news/2013/02/24/ruby-2-0-0-p0-is-released/)*

0. Provide a one or two sentence description of the changes.
 
*There are changes to Language core features, built-in libraries, debug support, and performance improvements. It is reportedly more compatible with 1.9 than 1.9 was with 1.8. It is stable, and apparently has improved documentation over 1.9.3.*

#### What is a patch level? (For example, the p420 in 1.9.3-p420)

0. Provide an overall answer in one or two sentences.

*My understanding is that a patch level is a version of a program updated with a certain set of bug fixes, optimizations, etc. ('patches'). Each time a new set of fixes is integrated into the program, a new patch level is released.*

0. Provide a URL to the official release notes on a particular patch level.

*Here are the release notes for Ruby 2.0.0-p247:*

*[https://www.ruby-lang.org/en/news/2013/06/27/ruby-2-0-0-p247-is-released/](https://www.ruby-lang.org/en/news/2013/06/27/ruby-2-0-0-p247-is-released/)*

#### What is MRI, what are some alternative rubies?

0. Provide an overall answer in one or two sentences.

*MRI stands for "Matz's Ruby Interpreter" and it's considered the 'standard' (or most common) Ruby interpreter. Some alternative rubies (known by my rvm) are GoRuby, Topaz, JRuby, Rubinius, Opal, and others*

0. Provide URLs to the home page or official project page of three alternative rubies and, in one or two sentences each, describe the advantage to each (in the opinion of their adherents).

*[Rubinius](http://rubini.us)--They claim this runs Ruby code fast, and they talk about running on 'all the CPU cores,' that it's 'designed for concurrency,' and built using Ruby. I don't know whether MRI doesn't 'run all the CPU cores,' I'm a little lost when they're talking about 'concurrency,' and not sure whether MRI was or wasn't built with Ruby, but the Rubinius folk make their interpreter sound pretty good.

*[Topaz](http://docs.topazruby.com/en/latest/)--The author of this interpreter claims it's 'high performance' and was written in Python. I put this one on as a representative of the 'less popular' ones (though it looks like it's only been around a little while).*

*[JRuby](http://jruby.org)--On a [linked page](http://confreaks.com/videos/1281-rubyconf2012-why-jruby-works) from the JRuby site, they claim it 'performs better than just about any implementation.' They justify this by claiming it 'has solid, reliable parallel threading' (I have no idea what that means); they say 'its extensions are managed code and won't segfault or interfere with threads or GC' (I'm even more lost here); and they say it gives Ruby access 'to anything that runs on a JVM, even code written in other languages.' (Hm, that might be cool).* 

#### What is a gem? What is "gem"?

0. Provide an overall answer in one or two sentences, including the official name of the package manager. 

*My understanding is that a gem is a set of code called a 'library' that's all rolled into a package that includes the code, documentation, tests, and a 'gemspec' file with information on the gem. The 'gem' command is used to manipulate gem packages from the command line. RubyGems is the package manager.*

0. Provide a URL to a site where all the popular gems are described.

*[RubyGems.org](http://rubygems.org/gems) has a pretty comprehensive list.*

0. Provide three command line examples of
  0. How to get help on gem commands
     *"gem help commands"*
  0. How to search for available gems
     *"gem list --remote"
  0. How to list the gems installed on your system
     *"gem list"

####What are reserved words?

0. Provide an overall answer in one or two sentences

*Reserved words are words used by Ruby that you should not use to create your own variables, methods, etc. For the most part, these seem to be global methods.*

0. Provide a URL to a page where all the reserved words are listed.

*[Tutorialspoint.com](http://www.tutorialspoint.com/ruby/ruby_quick_guide.htm) has them listed on that link.

0. In one or two sentences, tell me what why you can't use reserved words for your own variable and method names.

*These words are already used by Ruby for global methods, etc. so you can't use them for your own methods. We did change a global method (+) in our code challenge, so that makes me wonder whether you might actually be able to do this (though + is not a reserved word), but I haven't been able to find an answer, and it seems like it's best to just come up with your own method names.*

####What is a "class"? What is an "object"?

0. Provide an overall answer in one or two sentences, highlighting the differences between the two concepts.

*It seems like 'everything' is supposed to be an object in Ruby, but my understanding is that a "Class" is where you essentially define a template for an object--a place from which you can generate an instance of the class (an 'object') that can use all of that class's methods.*

0. Provide a short snippet of code that defines a ruby class with a class variable, an instance variable, a class method, and two instance methods - one public and one private. The methods don't have to do anything, but the variables have to be accessible for both get and set from other objects. Make sure all names comply with ruby naming conventions.

*class 
*
*  def public_method
*    puts "This is a public instance method."
*  end
*
*private
*
*  def private_method
*    puts "This is a private instance method."
*  end

0. Provide a short snippet of code that instantiates an object of the class you just defined, calls the methods, and gets and sets the variables.

0. Provide URLs or references to where you learned how to do the prior two snippets.

####As far as ruby is concerned, what is truthiness? 

0. Provide an overall answer in one or two sentences.

0. Provide a list of things in ruby that evaluate to false.

0. Provide a list of things in ruby that evaluate to true.

####  = vs == vs ===

0. Answer the question: Does ruby have a === operator? Why or why not?

0. Compare the different operators and provide examples of how the are used.

#### Many happy returns

0. Describe the "return" statement. What does it do? Why is it useful? 

0. Compare "return", "break", and "next" in one or two sentences.

0. Answer the question: If a method doesn't have a return statement, what gets returned?

0. Offer an opinion on the following: Is using a final return statement idiomatic ruby? Why or why not? What effect does this have on readability? Limit your opinion to a paragraph, but feel free to provide code snippets to support your claim.

<hr />
Copyright © 2013 Alan Zimmerman <br />
Used by permission by Portland Code School

