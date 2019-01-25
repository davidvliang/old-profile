---
layout: essay
type: essay
title: How Do I Ask A Question?
# All dates must be YYYY-MM-DD format!
date: 2019-01-24
labels:
  - Smart Questions
  - Problem Solving
---

 <img class="ui small right floated spaced image" src="../images/confused-man.jpg">
 
# The Mindset
Programming is by no means an easy feat. There is guaranteed to be a problem, or problems, that will stump the programmer and leave them dead in their tracks. At that point maybe it’s the best time to get some help from someone of higher knowledge.. or is it? We ask questions to get solutions to our problems, but we must'nt be too eager to obtain this help without first attempting to find the answer ourselves. The philosophy behind "smart" questions and "not smart" questions resides behind the principle of putting in your maximum effort into a problem before invoking someone else.

# What We Should and Shouldn't Do
Eric Steven Raymond had written a rant that shapes itself into a practical guide on how to ask a question the correct and appropriate way. So, what is considered a “smart” question? According to [Raymond’s essay](http://www.catb.org/esr/faqs/smart-questions.html),  An example of this is provided on stack overflow [here](https://stackoverflow.com/questions/1732348/regex-match-open-tags-except-xhtml-self-contained-tags/1732454#1732454) and is shown below.

<blockquote>
  
Topic: RegEx match open tags except XHTML self-contained tags
  
Question: 

I need to match all of these opening tags:
</blockquote>

```
<p>
<a href="foo">
```
<blockquote>
But not these:
</blockquote>
```
<br />
<hr class="foo" />
```
<blockquote>
I came up with this and wanted to make sure I've got it right. I am only capturing the a-z.
</blockquote>
```c
<([a-z]+) *[^/]*?>
```
<blockquote>
I believe it says:

- Find a less-than, then
- Find (and capture) a-z one or more times, then
- Find zero or more spaces, then
- Find any character zero or more times, greedy, except /, then
- Find a greater-than

Do I have that right? And more importantly, what do you think?

</blockquote>

From this post it is evident that the questioner made an attempt to the problem by 

On the contrary, a “not smart” question this [post](https://stackoverflow.com/questions/388470/stacktrace-information-preserving-paths-of-original-source?answertab=votes#tab-top)


 Topic: Stacktrace information preserving paths of original source

 Question:

 I am using C#.net for application development.

 To log and debug exceptions, I use the stacktrace.

 I executed my application on another machine, but when errors occur it refers to the path of my development machine.

 ```
 Ex:   D:\Projects\xyz.CS line no :12 _Error_message_here.
 ```

 Why does it trace to the path on my development machine path even though I am running the application on another machine?




This and yet, there are those that claim there is no such thing as a dumb question.

# But Why?
We must understand that the programmers that answer these questions are people with In fact, they are answering questions <i>voluntarily</i>. The answerer wants to answer the question or else they would not be subscribed to a forum such as Stack Overflow or even bother to respond. It is not their responsibility to serve whatever of your problems you throw at them. The methodology mentioned in Raymond's guide serves to bring more structure to the question and answer system. This structure, of which, is rooted on the fundamentals of good manners and courtesy. This brings up a certain variation to that age old adage, that is, “there are no such thing as dumb questions, only dumb people.”

