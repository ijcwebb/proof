---
title: "An Introduction to Mathematical Proof"
author: "Iain Webb"
date: "2021-04-16"
site: bookdown::bookdown_site
documentclass: book
bibliography: [book.bib]
biblio-style: apalike
link-citations: yes
description: "Description"
---
# Introduction



Welcome! It's lovely to have you here!

<img src="figures/head1.png" width="332" />

## About this course

This book accompanies the course "Reason and Argue Better: Logic in Proof and Argument", which was written between 2018-2019 and has been taught every semester since.

This is the third semester that this course has been taught online or partly online. The course has been adapted for online teaching, with some elements simplified and others expanded. Completing this course online offers some challenges, but also opportunities for things not possible when offline. 

## About this book

This book contains the material we will study as well as exercises (see the next section) and links for further reading. Most weeks I will assign you a chapter to read, and you should complete both the reading and the exercises within the chapter before our next class. 

This textbook may be updated during the course. Therefore you are advised to access the book at the link at https://ijcwebb.github.io/proof, rather than printing or downloading it. Also, even though you *can* read ahead of the set chapter, you are advised that later chapters might change as the course procedes.

Part I of this book (chapters 2-5) covers the terminology surrounding mathematical proof, part II (chapters 6-9) covers the basics of proof, and chapters 10-16 in part III each cover a different method of proof. Chapter 17 covers mathematical completeness.

## How to use this book

When completing the week's reading, you will encounter some exercises. I will indicate which of these you should attempt.

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-2"><strong>(\#exr:unnamed-chunk-2) </strong></span>Regular exercises look like this...
  
a. ...with subparts...
b. ...like this.
</div>\EndKnitrBlock{exercise}
</div>

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}Solutions might be included underneath exercises, in which case you should aim to complete the exercise before checking the solution. If the solution is not included, then we will probably discuss it in class.
</div>\EndKnitrBlock{solution}

<div class="alert alert-danger" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-4"><strong>(\#exr:unnamed-chunk-4) </strong></span>Extension exercises look like this. These are exercises that require a little more thought. 

Solutions won't be given in the book for these exercises, but we may discuss these in class. You can also book one-to-one consultations to discuss.
</div>\EndKnitrBlock{exercise}
</div>

There are a couple of other coloured boxes used in this book:

<div class="alert alert-warning" role="alert">
<strong>Careful!
</strong> This is where I alert you to mistakes commonly made by students in this course. Read these warnings carefully to avoid these mistakes yourself.
</div>


<div class="alert alert-success" role="alert">
<strong>What we've learnt </strong> 
These boxes are found at the end of each chapter, and recap the main things we have covered in the chapter. You can view these as key takeaways from the chapter. These often set us up for the next chapter too. 
</div>

That's it. You're ready to begin!

<!--chapter:end:index.Rmd-->

# Statements

A statement is a **remark** or **declaration**. Here are some examples:

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-5"><strong>(\#exm:unnamed-chunk-5) </strong></span>Life is pain.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-6"><strong>(\#exm:unnamed-chunk-6) </strong></span>I am 19 years old.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-7"><strong>(\#exm:unnamed-chunk-7) </strong></span>I like your hat.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-8"><strong>(\#exm:unnamed-chunk-8) </strong></span>London is the capital of Great Britain.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-9"><strong>(\#exm:unnamed-chunk-9) </strong></span>Four people are traveling to different places on different types of transport.
</div>\EndKnitrBlock{example}

## Non-statements    

So what is *not* a statement? I've listed four types of non-statements below. Can you think of any other types?

### Fragments

Fragments are incomplete sentences, and are not statements.

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-10"><strong>(\#exm:unnamed-chunk-10) </strong></span>Fish.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-11"><strong>(\#exm:unnamed-chunk-11) </strong></span>I am.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-12"><strong>(\#exm:unnamed-chunk-12) </strong></span>Bro!
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-13"><strong>(\#exm:unnamed-chunk-13) </strong></span>Okurrr.
</div>\EndKnitrBlock{example}

### Questions

Anything that ends with a question mark is not a statement; it's a question.

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-14"><strong>(\#exm:unnamed-chunk-14) </strong></span>What is $2 \cdot 2$?
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-15"><strong>(\#exm:unnamed-chunk-15) </strong></span>Are you going to eat that?
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-16"><strong>(\#exm:unnamed-chunk-16) </strong></span>What is this life if full of care?
</div>\EndKnitrBlock{example}

### Implicit answers

Anything that answers a question, **without explicitly referencing the question**, is not a statement. Or at least, not one that we can work with.

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-17"><strong>(\#exm:unnamed-chunk-17) </strong></span>$162.5$
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-18"><strong>(\#exm:unnamed-chunk-18) </strong></span>Yes it is.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-19"><strong>(\#exm:unnamed-chunk-19) </strong></span>The day after tomorrow.
</div>\EndKnitrBlock{example}

### Exclamations

These are like fragments, and are not complete sentences.

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-20"><strong>(\#exm:unnamed-chunk-20) </strong></span>Dang!
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-21"><strong>(\#exm:unnamed-chunk-21) </strong></span>Ura!!
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-22"><strong>(\#exm:unnamed-chunk-22) </strong></span>Phew!
</div>\EndKnitrBlock{example}

## What makes a *good* statement?

Not all statements are equally good! Some are better than others. Follow the rules below for high-quality statements:
    
### All the words should be clear and understandable

All the words in a statement should *either* already be understood by the reader, or should be easy to Google. Let's look at some examples:

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-23"><strong>(\#exm:unnamed-chunk-23) </strong></span>**Bishkek** is the **capital** of the **Kyrgyz Republic**.
</div>\EndKnitrBlock{example}

This is nice and clear. We know what the Kyrgyz Republic is, we know what Bishkek is, and we know what a capital is.

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-24"><strong>(\#exm:unnamed-chunk-24) </strong></span>The **human foot** is comprised of 26 **bones**.
</div>\EndKnitrBlock{example}

Again, this statement is nice and clear. We know what each term means.
    
\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-25"><strong>(\#exm:unnamed-chunk-25) </strong></span>An **atom** of **uranium** has one more **electron** than an **atom** of **protactinium**.
</div>\EndKnitrBlock{example}

We might not understand every term here, but we could use Google to find out more.
    
\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-26"><strong>(\#exm:unnamed-chunk-26) </strong></span>The **candidate** won the **popular vote** but lost the **election**.
    </div>\EndKnitrBlock{example}

This isn't clear, and no matter how much Googling we do, we won't be able to clarify the details. We need to ask the author of the statement: Which election? Which year? Which candidate?
    
\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-27"><strong>(\#exm:unnamed-chunk-27) </strong></span>**I love you**.
</div>\EndKnitrBlock{example}

On its own, this statement isn't clear enough. Who is speaking, and to whom?

Once we understand that, we need to ask whether **love** is clearly defined? Are we talking about something from the soul? Something biological? Familiar love? Friendship?
    
\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-28"><strong>(\#exm:unnamed-chunk-28) </strong></span>1000 is a **large** number.
</div>\EndKnitrBlock{example}

There's only one word here which is not clear: large. It's not clear how the author is defining large. Maybe the author could change the statement to compare it with something:

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-29"><strong>(\#exm:unnamed-chunk-29) </strong></span>1000 is larger (higher) than 500.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-30"><strong>(\#exm:unnamed-chunk-30) </strong></span>1000 people died of **Covid-19** today in the U.S., the largest **daily total** since the **global pandemic** began.
</div>\EndKnitrBlock{example}
        
\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-31"><strong>(\#exm:unnamed-chunk-31) </strong></span>1000 is the largest number for which the **Romans** had a **symbol**.
</div>\EndKnitrBlock{example}

In all three of these statements, the word "large" has now  been given clear meaning.

### No paradoxes!

Paradoxes contradict themselves. They are statements which are built on tricks of language:
    
\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-32"><strong>(\#exm:unnamed-chunk-32) </strong></span>This sentence is not clear.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-33"><strong>(\#exm:unnamed-chunk-33) </strong></span>This sentence is false.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-34"><strong>(\#exm:unnamed-chunk-34) </strong></span>The next sentence is not true. The previous sentence is true.
</div>\EndKnitrBlock{example}
            
Because paradoxes are built to contradict themselves, they aren't much use to us. Therefore we'll avoid them in this course.^[They are good for keeping our brains busy though!]

<div class="alert alert-danger" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-35"><strong>(\#exr:unnamed-chunk-35) </strong></span>Can you find any other paradoxical statements? What makes them paradoxical?
</div>\EndKnitrBlock{exercise}
</div>

### Statements should stand on their own

Don't you hate that feeling when you start watching a film but nothing makes sense because you didn't watch the previous films in the series?^[I had watched *none* of the previous Marvel movies before watching *Avengers: Endgame*. I understood nothing and had to spend an hour afterwards quizzing my boyfriend on the Tesseract, the Ancient One, and what Robert Downey Jr. was doing stranded in space. I *think* I got it.]
    
A good statement should stand on its own, and not rely on the reader knowing previous statements. If it *does* assume knowledge of previous statements, they should be referenced or restated, like including a plot synopsis for the previous movies!

Now it's your turn. Bring your answers to our next class. 

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-36"><strong>(\#exr:unnamed-chunk-36) </strong></span>Take a look at the statements below. Are all the terms clear? Do you understand all the terms? If not, do you think you could find out their meaning on your own? Do any of the statements need more explanation by the author?
    
a. It is hot today.
b. It is hotter today than it was yesterday.
c. The highest temperature on record, 54.4$^{\circ}$C or 130$^{\circ}$F, was measured on 16th August 2020 at the Death Valley National Park in California.
d. The explosion in Beirut in August 2020 could have been avoided.
e. 24 is a nice number.
f. 28 is a perfect number.
g. Two negatives make a positive.
h. Aman has a twin sister.
i. Ariana Grande was the most streamed artist of the year.
j. On average it rains more in Wales than it does in Kyrgyzstan.
</div>\EndKnitrBlock{exercise}
</div>

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}Here are a few solutions to the above exercise.

a. It is not clear what hot means. Definitions of hot will vary around the world and from person to person. It's also not clear which day the statement is talking about (i.e. when the statement was written).

b. This is clearer than the previous statement, however we could benefit from knowing where this statement is talking about. Bishkek? New York? Night time? Day time? And again, it's not clear which day the statement is talking about (i.e. when the statement was written).

c. This is pefectly clear. We know where and when the statement is talking about, that it is referring to a peak temperature, and that it is not claiming that this was indeed the highest temperature ever on Earth, merely that it is the highest on record.
</div>\EndKnitrBlock{solution}

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-38"><strong>(\#exr:unnamed-chunk-38) </strong></span>Using the three rules given above, which of the following statements are good? What is wrong with the others?
    
a. The cyrillic alphabet contains 33 letters.
b. Gunnar Garfors has visited every country in the world.
c. People find it harder to concentrate on one task than they used to.
d. Mobile phones have gotten more powerful over time.
e. Video games help people relax.
f. The US is larger than China.
g. The last word of this sentence is.
h. This sentence contains four e's.
i. This sentence contains 3 1's, 1 2 and 2 3's.
j. The longest word in this sentence is "complementary".
</div>\EndKnitrBlock{exercise}
</div>

<div class="alert alert-success" role="alert">
<strong> What have we learnt? </strong> 

- We know what *isn't* a statement.
- We know what makes a *bad* statement.
- We know what makes a *good* statement.

</div>

In this course, we will only work with good, high-quality statements. You should ensure that any statement *you* write obeys the above rules.
        
Next, let's look at whether good statements are true or not. 

<!--chapter:end:02-test.Rmd-->

# Truth values

## What is the truth value of a statement?  

Simply, the *truth value* of a statement is whether the statement is true or false. 
    
- The truth value of the statement "Bishkek is the capital of the Kyrgyz Republic" is true. 
- The truth value of the statement "Osh is the capital of the Kyrgyz Republic" is false.

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-39"><strong>(\#exr:unnamed-chunk-39) </strong></span>What are the truth values of the following statements?
  
a. $4 + 4 = 9$
b. $3 \cdot 6 = 18$
c. Ice melts above $0^{\circ}$C on Earth.
d. $11,118$ is the largest number in existence.
e. The Earth is closer to the Sun than Jupiter.
f. $a^2+b^2=c^2$, where $a$, $b$, $c = 1$.
g. $a = b+c$.
h. $1000$ is a large number.

See below for the answers.
</div>\EndKnitrBlock{exercise}
</div>

## Statements with clearly defined truth values

Look back up at **Exercise 3.1**. The first 6 statements all have **clearly defined** truth values: they are either true (b, c and e) or false (a, d and f).
    
What do we mean when we say a statement has a clearly defined truth value? 

- **Completeness** - The statement contains enough information for its truth value to be decided. Terms are clearly defined or easily researchable.
- **Objectivity** - The truth value of the statement is not based on personal opinion or experience.
- **Mutual exclusivity** - If a statement is true, it can't also be false. If a statement is false, it can't also be true.
- **Universality** - If the statement is true today, it will be true tomorrow, and it was true yesterday.

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-40"><strong>(\#exr:unnamed-chunk-40) </strong></span>Write:

a. a statement which has a clearly defined truth value of **true**.  
b. a statement which has a clearly defined truth value of **false**.
c. a statement which has a clearly defined truth value that *only you* know.
</div>\EndKnitrBlock{exercise}
</div>
    
## Statements without clearly defined truth values
 
Look again at **Exercise 3.1**. Statements g and h *don't* have clearly defined truth values? Why not?
    
Let's look at g: 

<center>

$a = b + c$

</center>

This statement doesn't contain enough information for us to be able to decide on its truth value. Aidai can make this statement true, by choosing the numbers $a = 5$, $b = 2$ and $c = 3$. But Patime can make this statement false, by choosing the numbers $a$, $b$, $c = 1$. When two people can come to different conclusions about the truth value of a statement, its truth value is not clearly defined.
    
Next we'll look at h: 

<center>

$1000$ is a large number.

</center> 

This statement doesn't have a clearly defined truth value because it depends on personal opinion. Younger members of your family might say the truth value of this statement is true, because they are used to using smaller numbers. However an economist or an astrophysicist or a paleontologist (or you) might disagree, because they are used to dealing with numbers much larger than 1000.
    
Let's look at two more examples: 

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-41"><strong>(\#exm:unnamed-chunk-41) </strong></span>$4x>0$
</div>\EndKnitrBlock{example}

Why is the truth value of this statement not clearly defined? It's because there is not enough information. Its truth value depends entirely on the value of $x$, about which we know nothing. If we choose $x$ to be 10, this statement is true, but if we choose $x$ to be $-5$, the statement is false. 

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-42"><strong>(\#exm:unnamed-chunk-42) </strong></span>Bishkek is a big city.
</div>\EndKnitrBlock{example}

We've already said that good statements are clear and specific. The reason for this is so that we can decide their truth value. 
    
In this statement, "big" is a very vague term. The units of measurement aren't clear. Is it referring to area, to the number of people in Bishkek, to the number of buildings, to the size of those buildings? Also, big compared to what? Compared to Karakol? Compared to Osh? Compared to Almaty? Compared to Seoul? Or maybe compared to 100 years ago? Again, it's not clear.

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-43"><strong>(\#exr:unnamed-chunk-43) </strong></span>The following statements **do not** have clearly defined truth values. Why not?

a. This math problem is difficult.
b. Damascus is an old city.
c. The largest city in my country is also my capital city.
d. The world is in a bad state.
e. $3.14$.
f. $x$ is positive.
g. $ab > cd$
h. Tomorrow is Wednesday.
i. $4$ is an unlucky number.
j. Nur-Sultan is the capital of Kazakhstan.
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-44"><strong>(\#exr:unnamed-chunk-44) </strong></span>Amend each of the ten statements in **Exercise 3.3** to give a statement with a clearly define truth value.
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-45"><strong>(\#exr:unnamed-chunk-45) </strong></span>Write a statement which does not have clearly defined truth value. For what reason(s) does your statement not have a clearly defined truth value?
</div>\EndKnitrBlock{exercise}
</div>

## Unknown truth values

What if you don't know the truth value of a statement? Does that mean it is not clearly defined?
 
Let's consider the following statement:  

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-46"><strong>(\#exm:unnamed-chunk-46) </strong></span>$29,999$ is a prime number.^[Go googling if you're not sure what *prime* means!]
</div>\EndKnitrBlock{example}

You probably don't know whether this statement is true or false. I certainly didn't know when I wrote it! However, it's clear that this statement *will* have a clearly defined truth value, even if we don't know what it is:
    
- **Completeness** - The statement contains enough information, and the terms are clear.
- **Objectivity** - The primeness of numbers is not a matter of personal opinion.
- **Mutual exclusivity** - This statement is either true or it is false: 29,999 can't be both prime and not prime. 
- **Universality** - If 29,999 is prime today, it will be prime tomorrow, and it was prime yesterday.

Here's another example:  

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-47"><strong>(\#exm:unnamed-chunk-47) </strong></span>Earth is the only planet in the entire universe with life.
</div>\EndKnitrBlock{example}
    
- **Completeness** - The statement contains enough information, and the terms are clear (as long as life is clearly defined^[It is possible that people might disagree on what constitutes life, see https://www.theguardian.com/books/2020/aug/06/lyfe-a-new-word-for-aliens-that-takes-a-leaf-out-of-life. However, as long as we agree on a definition of life, this statement will have a clearly defined truth value.]).
- **Objectivity** - The existence (or not) of life on other planets won't be a personal opinion: it either exists or it doesn't.
- **Mutual exclusivity** - This statement is either true or it is false.
- **Universality** - This statement is universal to a point. For example, the truth value of this statement *could* change over time, for example if life appears on a planet sometime in the future. However, considering the huge amounts of time that is required for life to appear, for our purposes this statement has universality.

Despite not knowing the truth value of this statement, it will have a clearly defined truth value. Either Earth *is* the only planet with life (statement's truth value: true) or there are other planets with life somewhere in the universe (statement's truth value: false).
    
However, unlike **Example 3.1**, this statement's truth value is less easy to find out. Googling ``is there life out there?'' isn't going to help, as the answer is not yet known, and might never be known. 

<div class="alert alert-warning" role="alert">
<strong>Careful!</strong> 

Just because we don't know the truth value of a statement, that doesn't mean it doesn't have one!

It's also possible that a statement has a clearly defined truth value that we will *never* know.
</div>

<div class="alert alert-danger" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-48"><strong>(\#exr:unnamed-chunk-48) </strong></span>Do you know (or can find out about) any statements which will have a clearly defined truth value but which no one in the world knows? Do people who know a lot about this statement think the truth value *will* one day be known, do they know it can never be known, or are they not sure? 
</div>\EndKnitrBlock{exercise}
</div>

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-49"><strong>(\#exr:unnamed-chunk-49) </strong></span>Which of the following are important for a statement's truth value to be clearly defined?

  - The statement contains enough information to assess its truth value.
  - The statement is written in English.
  - The statement is about mathematics.
  - Any terms new to the reader are easy to look up using Google or in a book. 
  - The statement is objectively true or false, not personal opinion.
  - The statement contains numbers.
  - The statement is universally true or false, not just locally.
  - The statement is short.
  - All terms are clear.
  - The statement is not a paradox.
  - Someone else wrote the statement, not me.
  - The statement is typed, not handwritten.
  </div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-50"><strong>(\#exr:unnamed-chunk-50) </strong></span>Which of the following statements will have clearly defined truth values? Which *won't* have clearly defined truth values? Why not?

a. No UN member state has a flag which contains purple.
b. SZA is taller than The Weeknd.
c. People find me funnier than you.
d. There is a largest number.
e. $x > 0$.
f. $|x|$ is never negative.
g. All odd numbers end with $1$, $3$, $5$, $7$ or $9$.
h. All even numbers end with $2$, $4$, $6$, $8$ or $0$.
i. $100$ is prime.
j. Poetry is difficult to understand.
k. Earth is the only planet in the universe which contains life.
l. All square numbers are even.
m. There are no solutions to the equation $a^2 + b^2 = c^2$.
n. There are no solutions to the equation $a^3 + b^3 = c^3$.
o. All perfect numbers are even.
p. Eating vegetables is good for people's health.
q. All men are created equal.
r. It rained in Bishkek on 01/01/2021.
s. All people have black hair.
t. Most people are good.
u. Max is tall.
v. The identity of the oldest person alive is known.
w. $30\mod 7 = 2$.
x. $29\mod 4 = 3$.
y. Japanese is the hardest language for non-native speakers to learn.
z. Japanese is difficult for non-native speakers to learn.
</div>\EndKnitrBlock{exercise}
</div>

<div class="alert alert-success" role="alert">
<strong> What have we learnt? </strong> 

In the previous chapter, we learnt what makes a good statement. In this chapter, we have learnt about truth values, and what it means for a statement to have a clearly defined truth value.

</div>


In our next chapter, we define a new term...

<!--chapter:end:03-test.Rmd-->

# Mathematical statements

## Definition

Quite simply, if a statement is good (clear and non-paradoxical) and has a clearly-defined truth value (even if you don't know what that truth value is), it is described as a **mathematical statement**.

Statements which fail to qualify as mathematical statements are called **non-mathematical statements**.

## Mathematical statements don't need to be about mathematics!

Before we move on, we need to address a really important point. When we say something is a mathematical statement, it does not have to be about mathematics!!

Let's look at some examples of mathematical and non-mathematical statements:

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-51"><strong>(\#exm:unnamed-chunk-51) </strong></span>Bishkek is the capital of the Kyrgyz Republic.

This is a mathematical statement, even though it's not talking about mathematics! It is mathematical because it is clear, all terms are defined, and it will have a clearly-defined truth value.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-52"><strong>(\#exm:unnamed-chunk-52) </strong></span>Malta is the largest country in the world

This is also a mathematical statement, despite not being about mathematics. It is clear, all terms are defined, and it will have a clearly-defined truth value. 
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-53"><strong>(\#exm:unnamed-chunk-53) </strong></span>$356$ and $989$ have no common divisors.

This is a mathematical statement - it will have a clearly-defined truth value.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-54"><strong>(\#exm:unnamed-chunk-54) </strong></span>There is a smallest elementary particle, one that can't be divided into smaller particles.

This is a mathematical statement. All terms are easy to Google, and the statement will have a clearly-defined truth value (though it's currently unknown^[See https://www.youtube.com/watch?v=ZorRPAD32i4 for what might be smaller than leptons and quarks, and https://www.youtube.com/watch?v=ehHoOYqAT\_U for a nice introduction to elementary particles.]).
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-55"><strong>(\#exm:unnamed-chunk-55) </strong></span>Pears are the best fruit.

This is not a mathematical statement because it is an opinion.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-56"><strong>(\#exm:unnamed-chunk-56) </strong></span>$8$ is better than $14$.

This statement is not mathematical because it is an opinion, and because "better" is not defined, and therefore will not have a clearly-defined truth value.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-57"><strong>(\#exm:unnamed-chunk-57) </strong></span>The Earth is big.

This is also not mathematical because it is vague and therefore will not have a clearly-defined truth value.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-58"><strong>(\#exm:unnamed-chunk-58) </strong></span>Poetry is difficult to understand.

'Understand' is not clearly defined (do we mean to get a personal understanding; to understand other people's interpretation of the poem; to grasp the poet's meaning; or just to understand what the words mean?). 'Difficult' will have a subjectivity to it which means different people might come to different conclusions about the truth value of this statement. It's also not clear which type of poetry, or which poet, the statement is referring to. Therefore the truth value of this statement will not be clearly defined, and so the statement is not mathematical.
</div>\EndKnitrBlock{example}

## Statements containing mathematics aren't necessarily mathematical!

We should also be clear on another point: Just because a statement contains mathematics, that doesn't mean it's mathematical! 

The statement "8 is a better number than 14" might be about numbers, but it's not mathematical because it doesn't have a clearly-defined truth value.

Equally, the statement "$ab = cd$" is definitely mathematical in its content, but it is not classified a mathematical statement because it doesn't contain enough information to decide on its truth value.

<div class="alert alert-warning" role="alert">
<strong>Careful!</strong> 

Mathematical statements don't have to be about mathematics. They just have to be good, clear statements with a clearly-defined (though possibly unknown) truth value. We use the word mathematical here to describe the *nature* of the statement, rather than its *content*.
</div>

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-59"><strong>(\#exr:unnamed-chunk-59) </strong></span>For this exercise, you should write:
  
a. A mathematical statement that is *not* about mathematics.
b. A mathematical statement that *is* about mathematics.
c. A non-mathematical statement that *is* about mathematics.
d. A non-mathematical statement that is *not* about mathematics.
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-60"><strong>(\#exr:unnamed-chunk-60) </strong></span>Do you know the truth values of the two mathematical statements you wrote in the previous question? If not, do you think you could find out?
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-61"><strong>(\#exr:unnamed-chunk-61) </strong></span>Look back at the twenty-six statements in Exercise 3.8. 

a. How many of them are mathematical statements?
b. How many are non-mathematical statements?
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-62"><strong>(\#exr:unnamed-chunk-62) </strong></span>Of those statements in Exercise 3.8 which *are* mathematical statements:

a. Which of them do you know are true?
b. Which do you know are false?
c. Which don't you know the truth value of but you think *someone* in the world does?
d. Do you think there are any to which *no one* in the world knows the answer to?
</div>\EndKnitrBlock{exercise}
</div>

<div class="alert alert-danger" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-63"><strong>(\#exr:unnamed-chunk-63) </strong></span>From Exercise 4.4, part d, we know that there are mathematical statements to which no one can *ever* know the answer? Can you think of any others? Remember, they don't have to be about mathematics!
  </div>\EndKnitrBlock{exercise}
</div>

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-64"><strong>(\#exr:unnamed-chunk-64) </strong></span>Below are four more statements. Repeat Exercises 4.3 and 4.4 for these statements.
  
a. There are infinitely many square numbers.
b. There are infinitely many prime numbers.^[Watch from 12:30 in this video: https://www.youtube.com/watch?v=OihQPf4mJH4.]
c. There are infinitely many perfect numbers.
d. There is no set^[A set is a collection of items.] whose cardinality^[Cardinality tells you the number of items in a set.] is strictly between that of the integers^[Integers are the whole numbers: ...-3, -2, -1, 0, 1, 2, 3...] and the real numbers^[Real number include both whole and non-whole numbers.].    
</div>\EndKnitrBlock{exercise}
</div>

<div class="alert alert-success" role="alert">
<strong> What have we learnt? </strong> 

- We've learnt to consider the *nature* of the statement, not its subject, when deciding if it is "mathematical" or not: the phrase 'mathematical statement' refers to a statement with a clearly-defined truth value, but not necessarily about mathematics.

- Therefore, the statement "C is the eighth letter of the Latin alphabet", "Nur-Sultan is further North than Bishkek" and "10 > 8" are all mathematical statements, but neither "$a > b$" nor  "$a^2 + b^2 = c^2$" nor "Bishkek is a green city" are mathematical statements, because they don't have a clearly-defined truth value.

</div>

<!--chapter:end:04-test.Rmd-->

# Axioms and definitions

Now that we fully understand what makes a statement "mathematical", we should discuss **axioms** and **definitions**. 

## Axioms are a special kind of mathematical statement

Axioms are mathematical statements which are true, and are *self-evidently* so and therefore cannot be proved. They should be things so obviously true or so universally accepted, that when you read them, you say to yourself, "*Duh, of course!*"^[https://www.merriam-webster.com/dictionary/duh]. Axioms should be so obvious, that when asked to prove them, you end up scratching your head and shouting "C'MON, IT JUST *IS* TRUE!!!!".

Axioms are the building blocks of mathematics. There is no complete list of them all, as we can always add more of them to the list. This chapter contains the axioms which we may use in this course. Tell me if you find a statement which you believe is an axiom but which I've forgotten, and I'll add it to the list below.

### Rules of axioms

- Axioms describe a property of a mathematical object or operation.
- Axioms should never cover more than one property.
- The property each axiom describes is not necessarily unique to the mathematical object, for example the *commutativity* property is true for both multiplication, "$ab = ba$", and addition, "$a+b=b+a$". Similarly "There are infinitely many ways to cut a circle into two equal halves" is also true for spheres: "There are infinitely many ways to cut a spheres into two equal halves".
- Axioms are mathematical statements which are true, elementary and universally accepted, but which don't have proofs (because they are so fundamental).
- Axioms should not be derived from other axioms.

### Axioms about algebra

Here are a few axioms about algebra. Note that $a, b, c$ and $d$ can be *any* numbers.^[See https://www.aaamath.com/ac11.htm.]

- If $a = c$ then $c = a$.
- If $a = c$ and $b = c$, then $a = b$.
- If $a = b$ and $b = c$, then $a = c$.
- If $a = b$ and $c = d$, then $a + c = b + d$.
- $a \cdot b = b \cdot a$.
- If $a = b$ and $c = d$, then $ac = bd$.

### Axioms about geometry

Here are a few axioms about geometry.^[See https://en.wikipedia.org/wiki/Foundations_of_geometry, http://web.mit.edu/wwmath/vectorc/3d/old/axioms.html, https://www.ams.org/journals/tran/1904-005-03/S0002-9947-1904-1500678-X/S0002-9947-1904-1500678-X.pdf, and http://www.mrc.uidaho.edu/~rwells/Critical%20Philosophy%20and%20Mind/Chapter%2023.pdf.] Look up any words you don't understand.

- If you have two points, you can draw a straight line which connects them.
- If you have two points, you can always draw a circle with one of the points at the circle's centre and the other on its edge.
- There are infinitely many ways to cut a circle into two equal halves.
- A straight line can be extended in either direction forever.
- Three points can be arranged in such a way that they don't all lie on the same straight line.
- Four points can be arranged in such a way that they don't all lie on the same flat plane.

**Note:** All of these axioms above can be written in even briefer terms, though I haven't done so, in order to ensure clarity. 

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-65"><strong>(\#exr:unnamed-chunk-65) </strong></span>Illustrate each of the six geometric axioms above with a pictorial example.
</div>\EndKnitrBlock{exercise}
</div>

<div class="alert alert-danger" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-66"><strong>(\#exr:unnamed-chunk-66) </strong></span>Can you think of any more algebraic or geometric statements which you believe are *so* obviously true that they are in fact axioms. Suggest them to me and if they're axioms, I'll add them to this chapter.

It's possible that *you* might consider a statement to be an axiom (something so obviously true that no proof is needed), but someone else might believe it is not self-evident and that a proof is needed. 

That's fine...if challenged to prove something that you believe is an axiom, rise to that challenge!
</div>\EndKnitrBlock{exercise}
</div>

## Definitions are a special kind of axiom

Where axioms describe a property of a mathematical object or operation, **definitions** describe mathematical objects or operations themselves. If axioms form the *rulebook* of mathematics, then definitions form the *dictionary* of mathematics.

### Rules of definitions

- Definitions describe a mathematical object or operation.
- Definitions should never cover more than one object or operation.
- Mathematical objects or operations don't have to have just one possible definition (e.g. the meaning of multiplication changes if we're talking about scalars, vectors, matrices, etc.).
- Definitions answer the question, "What is a ...?", for example "What is a square" or "What is an even number?" or "What is multiplication?"
- Definitions can't be proved, they are just accepted by all people doing mathematics.
- Definitions allow us to all agree on key terms in mathematics.
- Definitions can refer to other definitions.

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-67"><strong>(\#exr:unnamed-chunk-67) </strong></span>Write definitions for the following objects or operations.

a. A **square number** (or **perfect square**).
b. A **whole number** (or **integer**).
c. A **non-whole number**.
d. **Consecutive** whole numbers.
e. One number **divides** another. (Careful here, I don't simply mean division. Consider that 4 *divides* 12 but that 5 *does not divide* 12.)
f. An **even number**.
g. An **odd number**.
h. The **absolute** (or **modulus**) operation.
i. A **point**.
j. A **line**.
</div>\EndKnitrBlock{exercise}
</div>

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}These are *my* definitions, but these are not perfect. Different people might choose different words to describe these things, and your definitions might look different to mine. This isn't a problem as long as our definitions are both clear, and we both mean the same thing!

a. A **square number** (or **perfect square**) is the square of a whole number.
b. **Whole numbers** (or **integers**) are numbers with digits only to the left of the decimal point.
c. **Non-whole numbers** are numbers which have value to the right of the decimal point (and possibly to the left too).
d. Two whole numbers $a$ and $b$ are **consecutive** if either $b = a + 1$ or $a = b + 1$.
e. $a$ **divides** $b$ if $b \div a$ leaves no remainder.
f. **Even numbers** are whole numbers which can be written in the form $2n$, where $n$ is a whole number.
g. **Odd numbers** are whole numbers which *cannot* be written in the form $2n$, where $n$ is a whole number.^[Alternatively: **Odd numbers** are whole numbers which can be written in the form $2n + 1$, where $n$ is a whole number.]
h. The **absolute** (or **modulus**) of a negative number is the positive version of that number.
i. A **point** has no length, width or height.
j. A **line** has length but no width or height.
</div>\EndKnitrBlock{solution}

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-69"><strong>(\#exr:unnamed-chunk-69) </strong></span>Below are three mathematical statements (i.e. they have clearly-defined truth values). One of them is an axiom, one is a definition and one is just a regular statement. Which is which?
    
a. The sum of the digits of any number divisible by $9$ is itself divisible by $9$.
b. The product of two negative numbers is positive.
c. For two positive numbers $a$ and $b$, $a$ is larger that $b$ if $a - b > 0$.
</div>\EndKnitrBlock{exercise}
</div>

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-70"><strong>(\#exr:unnamed-chunk-70) </strong></span>Come up with definitions of the following terms. Try to be concise, but sufficiently clear.

a. A **rectangle**.
b. A **square**.
c. A **straight line**.
d. A **circle**.
e. A **3D shape**.
f. A **rational number**.
g. **Consecutive even numbers**.
h. **Consecutive odd numbers**.
i. **MAX**(   ).
j. **MIN**(   ).
k. An **acute angle**.
l. A **circle's circumference**.
m. A **tangent** to a circle.
n. The **sum** of two numbers.
o. The **difference** of two numbers.
p. The **product** of two numbers.
q. The **ratio** of two numbers.
r. A **cube number** (or **perfect cube**).^[Unlike perfect squares, perfect cubes do not have a small number of possibilities for the last two digits. Except for cubes divisible by $5$, where only $25$, $75$ and $00$ are allowed.]
s. A **triangle**.
t. A **cuboid**.
u. **Adjacent** sides of a triangle.
v. A **multiple** of a number.
w. An **octagon**.
x. Two **perpendicular** lines.
y. A **prime number**.
z. The **proper divisors** (or **proper factors**) of a whole number.
</div>\EndKnitrBlock{exercise}

</div>

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}^[See https://studymaths.co.uk/glossary.php, http://www.mrc.uidaho.edu/~rwells/Critical%20Philosophy%20and%20Mind/Chapter%2023.pdf, https://www.quora.com/Is-there-a-comprehensive-list-of-axioms-and-math-principles-to-make-learning-math-easier, https://sites.math.washington.edu/~aloveles/Math300Summer2011/Math300Axioms.pdf.]

A square number (or perfect square) is the square of a whole number.

Whole numbers (or integers) are numbers with digits only to the left of the decimal point.

Non-whole numbers are numbers which have value to the right of the decimal point (and possibly to the left too).

Two whole numbers a and b are consecutive if either $b = a + 1$ or $a = b + 1$.

$a$ divides $b$ if $b ÷ a$ leaves no remainder.

Even numbers are whole numbers which can be written in the form $2n$, where $n$ is a whole number.

Odd numbers are whole numbers which cannot be written in the form $2n$, where $n$ is a whole number.

The absolute (or modulus) of a negativenumber is the positive version of that num-ber.

A point has no length, width or height.

A line has length but no width or height.

A rectangle: A 2D shape with four straight sides and four right angles

A straight line:  a line with unchanging slope

A circle:  a shape representing all the points equidistant from a single point

A 3D shape: a shape with width, length and height

A rational number: a number that be expressed at the ratio of two integers

Consecutive even numbers: If a is an even number $2n$, and $b = a+2$, then $a$ and $b$ are consecutive even numbers.

Consecutive odd numbers: If $a$ is an odd number $2n + 1$, and $b = a + 2$, then $a$ and $b$ are consecutive odd numbers.

MAX(  ): Returns the largest of a set of numbers.

MIN(  ):  Returns the smallest of a set of numbers.

An acute angle: An angle measuring between $0$ and $90$ degrees.

A circle's circumference: The distant around the edge of a circle.

A tangent to a circle: A straight line which intercepts a circle only once.

The sum of two numbers: For two numbers $a$ and $b$, their sum is $a + b$.

The difference of two numbers: For two numbers $a$ and $b$, their difference is $a - b$.

The product of two numbers: For two numbers $a$ and $b$, their product is $a \cdot b$.

The ratio of two numbers: For two numbers $a$ and $b$, their ratio is $a / b$.

A cube number (or perfect cube): A perfect cube is the cube of an integer.

A triangle: A three-sided 2D shape.^[According to this song, https://www.youtube.com/watch?v=gHjnGbNBuAw, "three points were two lines meet".]

A cuboid: A 3D shape which has six rectangular faces at right angles to each other.

Adjacent sides of a triangle: Two sides which meet at a common point.

A multiple of a number: The number multiplied by any integer.

An octagon: An eight-sided 2D shape.

Two perpendicular lines: Two straight lines which meet at a right-angle.

A prime number: An integer whose only two unique divisors are $1$ and itself.

The proper divisors (or proper factors) of a whole number: Integers which divide into another integer, excluding the number itself.
</div>\EndKnitrBlock{solution}

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-72"><strong>(\#exr:unnamed-chunk-72) </strong></span>Use the following questions to check your understanding of some key definitions.

a. Is zero even?
b. Is a square a rectangle?
c. Does $12$ have five or six divisors?
d. How many proper divisors does $25$ have?
e. If a triangle is a "$3$-gon", a pentagon is a "$5$-gon", and an octagon is an "$8$-gon", what is a "$4$-gon"?
f. What's a "$6$-gon"? What's a "$2$-gon"?
g. Is $87$ prime?
h. How many multiples of $7$ are two-digit numbers?
i. How many pairs of adjacent sides does a triangle have?
j. How many of the following are *not* lengths?

  - circumference of a circle
  - perimeter of a rectangle
  - distance between two points
  - width of a cuboid
  - height of a cylinder
</div>\EndKnitrBlock{exercise}

</div>

<div class="alert alert-success" role="alert">
<strong> What have we learnt? </strong> 

- Axioms are special kinds of mathematical statements; they are ones which are self-evidently true. They are the building blocks of mathematics.
    
- We've also learnt that *really* fundamental axioms are called definitions. They are how we guarantee that you, your fellow mathematicians and your reader all understand what you're talking about!^[See https://en.wikipedia.org/wiki/Vacuous_truth.]

</div>

## Types of real numbers

In section 5.4, we will meet some axioms about **inequalities**. Inequalities describe the *ordering of real numbers*. In this section, we will check we know what real numbers are.

Real numbers are any numbers on the number line which stretches from $-\infty$ to $\infty$:

<div class="figure" style="text-align: center">
<img src="figures/numberline.png" alt="The number line." width="90%" />
<p class="caption">(\#fig:unnamed-chunk-73)The number line.</p>
</div>

\begin{center}
\begin{tikzpicture}
\draw[latex-latex] (-5.5,0) -- (5.5,0) ; %edit here for the axis
\foreach \x in  {-5,-4, -3,-2,-1,0,1,2,3,4,5} % edit here for the vertical lines
\draw[shift={(\x,0)},color=black] (0pt,3pt) -- (0pt,-3pt);
\foreach \x in {,, -3,-2,-1,0,1,2,3,,} % edit here for the numbers
\draw[shift={(\x,0)},color=black] (0pt,0pt) -- (0pt,-3pt) node[below] 
{$\x$};
\end{tikzpicture}
\end{center}

*Any* number that a calculator can display is a real number:

(A) Whole numbers (integers)
(B) *Terminating* decimals (0.1, -0.5, 68.25)
(C) *Recurring* decimals ($\frac{1}{3} = 0.3333...$, $-\frac{11}{9} = -1.2222...$, $\frac{1}{7} = 0.142857142857...$. In the last example, notice that the sequence $142857$ repeats.)
(D) Non-recurring decimals ($\pi = 3.1415926...,$ $e = 2.7182818284590$, $\sqrt{2} = 1.41421356237...$)

We split the four types of real number above into two groups: 

### Rational real numbers
(A), (B) and (C) are **rational real numbers**, because they can be expressed as the *ratio* of two integers.

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-74"><strong>(\#exr:unnamed-chunk-74) </strong></span>Pick an example of a number of type (A), (B) and (C) above. Show for each of your choices that the number can be written as the ratio of two integers.
</div>\EndKnitrBlock{exercise}
</div>

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}Answers will vary. An example of type (A) is $4$, which can be written as $\frac{4}{1}$, which is the ratio of two integers. Similarly, $-3$ can be written as $\frac{-3}{1}$, which is the ratio of two integers. An example of type (B) is $0.5$, which can be written as $\frac{1}{2}, which is the ratio of two integers. Similarly, $-0.1$ can be written as $\frac{-1}{10}$, which is the ratio of two integers. Or $1.875$, which can be written as $\frac{15}{8}$, and $19.5$ which can be written as $\frac{29}{2}$. An example of type (C) is $-0.1111...$ which can be written as $\frac{-1}{9}$, or 1.166666... which can be written as $\frac{7}{6}$.</div>\EndKnitrBlock{solution}

### Irrational real numbers

Type (D) are **irrational real numbers**, because they *can't* be written as the ratio of two whole numbers.

<div class="alert alert-danger" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-76"><strong>(\#exr:unnamed-chunk-76) </strong></span>Later in the course, we'll see why $\pi$, $e$, $\sqrt{2}$ and $\sqrt{3}$ are all irrational numbers. Do you know a way to show this?^[Rational and irrational numbers have very different properties. The digits of rational numbers (including non-terminating decimal numbers) are fully known. The digits of irrational numbers can't be fully known because they follow no pattern and don't repeat. Just because you know the first 12 million decimal digits of $\pi$, it doesn't mean you can predict the 12-million-and-first digit!] ^[Whilst $\pi$ and $e$ are both known to be irrational, no one knows if $\pi + e$, $\pi e$, $\dfrac{\pi}{e}$, $\pi^e$, $\pi^\pi$, $e^e$, $e^\pi$, $2^e$ or ln$\pi$ are rational or irrational. See https://math.ou.edu/\char`\~jalbert/courses/openprob2.pdf.]
</div>\EndKnitrBlock{exercise}
</div>

### Symbols

We use the symbol $\mathbb{R}$ to mean ALL real numbers, for example $a \in \mathbb{R}$ means that the number $a$ is a real number (and $a \not\in \mathbb{R}$ means that the number $a$ is not a real number^[We won't deal with "non-real" numbers (called imaginary or complex numbers) in this course.]).

We use the symbol $\mathbb{Q}$ for just the rational real numbers, and $\mathbb{Q}'$ for the non-rational real numbers. For those rational numbers which are integers (whole numbers), we use the symbol $\mathbb{Z}$.

<div class="figure" style="text-align: center">
<img src="figures/numbertypes.png" alt="The real numbers are divided into two groups." width="90%" />
<p class="caption">(\#fig:unnamed-chunk-77)The real numbers are divided into two groups.</p>
</div>

How to use these symbols? As mentioned above, to tell your reader that you're talking about a general real number, you write $a \in \mathbb{R}$, where $\in$ means "belongs to" or "is".

<div class="alert alert-warning" role="alert">
<strong>Careful!</strong> 

The symbol $\in$ is very powerful: it covers ALL possible values of the type of number given. For example, if you write $a \in \mathbb{Z}$, you are saying that $a$ could be *any* integer in the world, and if you write $a \in \mathbb{Q}$, you're saying that $a$ can be *any* rational number. Similarly, writing $a \in \mathbb{Q'}$ means that $a$ is *any* irrational number (so not just $\pi$ or $\sqrt{2}$). 

</div>


Add $^{+}$ to any symbol to specify you're only talking about the positive numbers from the set. Similarly, add $^{-}$ to specify you're only talking about the negative numbers from the set.

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-78"><strong>(\#exr:unnamed-chunk-78) </strong></span>Give a couple of examples of $a$ in each of the cases below.

a. $a \in \mathbb{Z}^{+}$
b. $a \in \mathbb{Q}'$
c. $a \in \mathbb{Q}^{+}$
d. $a \in \mathbb{Z}^{*}$
e. $a \in \mathbb{Z}^{-}$
f. $a \in \mathbb{R}$
g. $a \in \mathbb{C}$
h. $a \in \mathbb{Z}$
i. $a \in \mathbb{R}^{+}$

Part d might be more challenging!
</div>\EndKnitrBlock{exercise}
</div>

### Further dividing up the integers

Within the integers, there are lots of sets of special numbers, for example *even* numbers, *odd* numbers, *prime* numbers, *triangle* numbers, *Fibonacci* numbers, and *perfect* numbers. Some of these sets overlap (i.e. there are some numbers which are in more than one set).^[Within these sets, there are even smaller subsets of numbers. For example, the Mersenne primes are special examples of primes.]

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-79"><strong>(\#exr:unnamed-chunk-79) </strong></span>Can you find:

a. A number which is both prime *and* triangular?
b. A number which is both prime *and* perfect?
c. A number which is both triangular *and* perfect?
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-80"><strong>(\#exr:unnamed-chunk-80) </strong></span>Are there any prime Fibonacci numbers?
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-81"><strong>(\#exr:unnamed-chunk-81) </strong></span> 

a. Is 1 perfect? Triangular? Prime? A Fibonacci number?
b. Is 2 perfect? Triangular? Prime? A Fibonacci number?
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-82"><strong>(\#exr:unnamed-chunk-82) </strong></span>What's the smallest positive integer that is neither prime nor triangular nor perfect nor Fibonacci? 
</div>\EndKnitrBlock{exercise}
</div>

## Inequalities

Inequalities compare numbers^[Or expressions], in terms of their size. Earlier in this chapter we defined "greater than" and "less than". One number is "greater than" another if it appears further to the right on the number line:

<div class="figure" style="text-align: center">
<img src="figures/numberline.png" alt="The number line. The further to the right a number is, the 'greater' it is." width="90%" />
<p class="caption">(\#fig:unnamed-chunk-83)The number line. The further to the right a number is, the 'greater' it is.</p>
</div>

So $11$ is greater than $10$ (or $11 > 10$), and $10$ is greater than $0$ (or $10 > 0$), and $2 > -5$ and $-5 > -10$. If we write $a > 5$, we mean that $a$ is a number greater than $5$ (for example $6$ or $20$ or $5.1$). If we write $a \geq 5$ we mean $a$ is either greater than $5$ or equal to $5$. The symbols $<$ and $\leq$ apply for less than, and less than or equal to.

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-84"><strong>(\#exr:unnamed-chunk-84) </strong></span>Here are three axioms about inequalities:

a. If $a>0$ and $b>0$, then $a+b>0$.
b. If $a>0$ and $b>0$, then $ab>0$.
c. If $a>0$ and $b>0$, then $a + b > a$ and $a + b > b$.

Because these are axioms, we can't prove them (they are *too* fundamental). However, we can illustrate them with examples. Find examples of each of the axioms above, in order to illustrate them.
</div>\EndKnitrBlock{exercise}
</div>

<div class="alert alert-danger" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-85"><strong>(\#exr:unnamed-chunk-85) </strong></span>Aida says that, mathematically, $-10$ is greater than $-50$. Murat says that $-50$ *could* be considered as greater than $-10$, in certain circumstances. How could you argue Murat's case? Give specific example(s) how he could be seen as right. ^[Note, in this course, we will ALWAYS use "greater than" to mean "further to the right on the number line" (despite what Murat says!).]
</div>\EndKnitrBlock{exercise}
</div>

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-86"><strong>(\#exr:unnamed-chunk-86) </strong></span>Below are five more axioms about inequalities. Again, illustrate each of these axioms with an example.
    
- If $a > b$ and $k$ is any real number, then $a + k > b + k$.
- If $a > b$ and $b > c$, then $a > c$.
- If $a > b$ and $k > 0$ then $ak > bk$.
- If $a > b$ and $k < 0$, then  $ak < bk$.
- For any real number $a$, $a^2 \geq 0$.   
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-87"><strong>(\#exr:unnamed-chunk-87) </strong></span>Below are four conjectures about inequalities. Find *counterexamples* which disprove them:
    
- If $a>0$ and $b>0$, then $ab > a$ and $ab > b$.
- If $a^2 < b^2$ then $a < b$.
- If $a < b$ and $k < l$ then $ak < bl$.
- If $\dfrac{a}{b} > cd$ then $ad > bc$. 

You only need to find one counterexample for each. *Hint: Negative numbers will be useful here!*
</div>\EndKnitrBlock{exercise}
</div>

<!--chapter:end:05-test.Rmd-->

# Mathematical proof

## Mathematics versus other fields

Mathematical proof is different to proof in other fields. Let's look at how.

### Terminology

Mathematics has a different set of terms when talking about proofs.

In mathematics, once we have identified a statement which we would like to try to prove or disprove, we rename it a **conjecture**.

If we are successful in proving it, the conjecture is renamed a **theorem**. If it is disproved, it is called a **disproved conjecture**. Only statements that have been proved true can be called theorems.

<div class="figure" style="text-align: center">
<img src="figures/statementjourney.png" alt="The journey of a statement." width="65%" />
<p class="caption">(\#fig:unnamed-chunk-88)The journey of a statement.</p>
</div>

\* A mathematical statement obviously!

<div class="alert alert-danger" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-89"><strong>(\#exr:unnamed-chunk-89) </strong></span>How many mathematical theorems can you name?
  </div>\EndKnitrBlock{exercise}
</div>

### Methodology

In mathematics we talk about theorems. In other sciences, they talk about theories. What's the difference? It all about how the proof is constructed.

**A proof in mathematics must be built DEDUCTIVELY**

We say therefore that a theorem in mathematics is deductively true. In other words, you should be able to provide a list of steps which someone else could follow and arrive at the same conclusions. 

**A proof in science is built on EVIDENCE**

We say therefore that a scientific theory is empirically (or "verifiably") true, based on observations made or evidence collected. To verify it, someone would need to either trust your evidence, or be able to recreate the evidence themselves.^[Something known as reproducibility.] The Oxford English Dictionary defines a theory as "A statement of what are held to be general laws, principles or causes of something known or observed".

That's the difference between a theorem in mathematics and a theory in science.

### Trial and improvement

In mathematics, once a conjecture's truth value has been discovered, it remains this way forever. However in other sciences (both natural sciences and social sciences), theories are always being improved upon and added to as more research is done and more discoveries made.

This is a key principle of modern science - it doesn't claim to know all the answers, but its aim is the truth, and it chooses as its foundations those theories which have the most compelling evidence.^[This approach provides a stable platform for further exploration. Just because science can't definitively say whether a statement is 100\% true, its chosen approach is better than throwing our hands up and saying "who knows!" or "no one can be sure!". Considering that we have science to thank for iPhones, vaccinations against deadly diseases, increased food yields, an understanding of how all life on Earth is connected, space exploration, and a great many other things, it's a pretty good approach!]

The **theory of gravity**, the **theory of relativity**, the **theory of evolution** and even the current form of **the periodic table** are all examples of theories which are constantly being changed and updated as new evidence is revealed.

Some scientific theories have even been shown to be completely wrong. Here's a short list of some theories previously believed true but later disproven: https://www.famousscientists.org/10-most-famous-scientific-theories-that-were-later-debunked.

### An ever-changing world

Statements about world geography, international politics, currency markets, individual people, the state of technology and a lot else besides are all likely to all be time-dependent. Countries fall, empires collapse, capitals change, phones get faster, people and animals evolve.

For example, the statement "Nur-Sultan is the capital of Kazakhstan" has a built-in time limit. It won't be true forever. We don't know how long it will be true for, but it won't be true forever. Sure, it is true at the moment, but what if the capital is renamed in future years? The truth value of the statement would change. 

"The capital of Kazakhstan is located in the north of the country" is also currently true. This statement is definitely more general, but is still time-dependent: the capital of Kazakhstan used to be located in the south of the country; what's stopping the location of the capital city shifting again in the future? 

And how long will Kazakhstan exist? All countries change over time. Eventually there won't be a Kazakhstan, or a France or a Benin or a Britain.

## So what does this all mean?

It means that the study of mathematics is different to other sciences, to economics, to philosophy, psychology, evolutionary biology, and all other fields of study. If something is proved in mathematics, its truth value won't change over time. Prove something is true in mathematics and you know that it has always been true and that it will remain true forever.^[For example, proving Pythagoras' Theorem (https://www.pinterest.com/pin/300122762659059179/) tells us this theorem is true for all time.] In 5 years or 100 years or 1000 years or a million years, the truth value will be unchanged. 

The axioms laid down by the Greek mathematician **Euclid of Alexandria** over two thousand years ago, some of which you met in Chapter 5, are as true now as they were then.^[See https://plus.maths.org/content/maths-minute-euclids-axioms.]

The mathematical proofs of the mathematician **Muhammad ibn Musa al-Khwarizmi**, born near Khiva in Central Asia, which he presented in his book *The Compendious Book on Calculation by Completion and Balancing*,^[The title of this book gave the us the word *algebra*, from the Arabic word *al-jabr* meaning "restoration", "the reunion of broken parts" or sometimes "bone-setting".] have not had their truth values changed in the hundreds of years since. The many proofs of French mathematician **Sophie Germain** are as valid now as they were in the 18th and 19th century when she wrote them. The mathematics of American mathematician **Katherine Johnson** in the 1960s or the Iranian mathematician **Maryam Mirzakhani** in the 2000s and 2010s will remain relevant forever. 

Anything **You** prove true in this course will be true forever. Anything you show is false will be false forever. Get ready to make your mark on history!

<div class="alert alert-danger" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-90"><strong>(\#exr:unnamed-chunk-90) </strong></span>How many theories in *your* major do you know? How are theories in your major proved true?
  </div>\EndKnitrBlock{exercise}
</div>

<div class="alert alert-success" role="alert">
<strong> What have we learnt? </strong> 

- As discussed in Chapter 4, a good mathematical statement has an unchanging truth value. In many fields, the truth value of statements can change over time, but in mathematics, once the truth value of a mathematical statement has been established, it will remain this way forever.

</div>

<!--chapter:end:06-test.Rmd-->

# Disproving a conjecture

We've discussed truth values a lot already, and we've agreed that *mathematical* statements must be either true or they are false.  Once we've decided that we're interested in finding out the truth value of a mathematical statement, we rename it a conjecture and get to work...

To **prove a conjecture**  means to show that its truth value is "true". To **disprove a conjecture** means to show that its truth value is "false".

In this chapter we'll discuss disproving conjectures. There's two ways to show a conjecture is false.

## Finding a counterexample

Disproving false conjectures is generally easier than proving true conjectures. This is because all false conjectures have **counterexamples**.

Take a look at the following two conjectures:

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-91"><strong>(\#exm:unnamed-chunk-91) </strong></span>No Chinese citizen has green eyes.</div>\EndKnitrBlock{example}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-92"><strong>(\#exm:unnamed-chunk-92) </strong></span>All Irish citizens have a vowel in their surname.</div>\EndKnitrBlock{example}

How you would prove, or disprove, these conjectures?

- To prove this first one, we would need to check the eye colour of *all* Chinese citizens. That's because this is a conjecture about all Chinese citizens. How long is that going to take!?! Is it even possible?!?
But to disprove this conjecture, we just need to find one Chinese citizen with green eyes. Much easier! This single green-eyed Chinese citizen would be our counterexample.
    
- To prove the second conjecture, we would need to consult a database of the surnames of all Irish citizens. We would then set up a computer to check that each of them contain a vowel (a, e, i, o or u).
To disprove the conjecture, we would just need to identify just one Irish citizen whose surname did not contain a vowel. This could be done using the database approach as well, or maybe we know of a famous Irish person whose surname is vowel-less. This one person would be our counterexample.

Just one counterexample is needed to disprove a false conjecture. Of course, we might find lots of counterexamples, i.e. many Chinese citizens who have green eyes, or many Irish citizens without vowels in their surname. This would be great - it would probably make our job of finding a counterexample easier! But even if there is only one Chinese citizen with green eyes, or one Irish citizen with a surname devoid of vowels, that is enough to show the conjecture is false.

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-93"><strong>(\#exr:unnamed-chunk-93) </strong></span>The following conjectures are all false. Find a single counterexample which shows this.

a. All prime numbers are odd.
b. $(a + b)^2 = a^2 + b^2$ for any numbers $a$ and $b$.
c. All sheep in South Africa are white. (Good luck Googling!)
d. The national flags of all UN members are rectangular.
e. All numbers are either positive or negative.
f. $a^2 > a$, where $a$ is a whole number.
g. If $a$ is a whole number and $a^2$ is divisible by $4$, then $a$ is divisible by 4.
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-94"><strong>(\#exr:unnamed-chunk-94) </strong></span>In the last exercise, you found counterexamples which disproved the conjectures.

a. Which of the conjectures above have just **one** counterexample? 
b. Which of the conjectures above have **a few** counterexamples? 
c. Which of the conjectures above have **an infinite number** of counterexamples?
</div>\EndKnitrBlock{exercise}
</div>

## Finding a disproof

Finding a counterexample is the most common and popular way of disproving a conjecture. It's also possible to disprove a conjecture without finding a counterexample. This is called finding a disproof, and often happens when you set out looking for a proof and it goes wrong! We'll look at this a bit later. 

<div class="alert alert-success" role="alert">
<strong> What have we learnt? </strong> 

- Finding a counterexample (or a few) is the most popular and common way to disprove a conjecture.
   
- Whilst there may be many counterexamples for a particular conjecture, just one is enough to disprove a conjecture.
   
- True conjectures don't have counterexamples, because they're true! Only conjectures which are false will have counterexamples.

</div>

<!--chapter:end:07-test.Rmd-->

# Getting started with a new conjecture

Let's take a moment to review what we've learnt over the past couple of chapters. In Chapter 5 we saw that axioms are statements which can't be proved, because they are so fundamental. Axioms (and the even more fundamental definitions) are statements which allow us to talk about and do mathematics.

<div class="alert alert-danger" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-95"><strong>(\#exr:unnamed-chunk-95) </strong></span>Here are four more axioms, all of which are about probability. How many of these have you heard about or used before?
  
- The probability of something happening is a non-negative, real number.
- The probability of something happening is never greater than 1.
- The sum of the probabilities of all possible events is 1.
- The probability that at least one of the possible events will happen is 1.
</div>\EndKnitrBlock{exercise}
</div>

In Chapter 6 we learnt that any mathematical statement^[Which is not an axiom or a definition.] that we're interested in proving or disproving can be reclassified a "conjecture". We can then attempt to prove it or disprove it. In Chapter 7 we saw that the most common way of disproving a conjecture is to hunt for a counterexample. 

In this chapter, we'll formalise the steps you should follow upon meeting (or creating) a new conjecture, of whose truth value you don't yet know. The steps are:

1. Look for a counterexample.

2. Attempt a proof:
- Rewrite the statement in the form "If...then..."
- If needed, draw the conjecture's map.
- Select the method(s) of proof.

## Step 1: Start by looking for a counterexample

When beginning with a new conjecture, you (probably) don't know whether it's true or false. Therefore, your first step should always be to look for a counterexample. We saw in the last chapter that to disprove a false statement, we just need to find a single counterexample to disprove it.

If you find one, then you have disproved the conjecture, and don't need to worry about trying to prove it (as you know it's false!). If you don't find one, it doesn't mean there isn't one, but at least you tried!

Looking for a counterexample is a good place to begin with a new conjecture because it helps you to understand what the conjecture is saying.

<div class="alert alert-warning" role="alert">
<strong>Tips for looking for a counterexample</strong> 

- How long should you look for a counterexample? I would suggest trying out four or five examples to see if any of them are counterexamples.

- Being creative when trying to find a counterexample will increase your chance of finding a one (if it exists). For example, with the second conjecture in **Exercise 8.2** below, you could experiment with $a$ and $b$ both positive, then with $a$ and $b$ both negative, then with $a$ and $b$ having different signs, then with either or both $a$ and $b$ equal to zero, etc. The more varied your attempts are, the more likely you're find a counterexample (if it exists).

- Keeping going until you think you've tried all possible "types" of example.

- Stop if you find a counterexample, or if you think you've tried enough and are ready to try a proof.
</div>

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-96"><strong>(\#exr:unnamed-chunk-96) </strong></span>Try to find a counterexample of the following conjectures. I'm not promising that they are all false so it might be that a counterexample doesn't exist for some of them.

(\#cnj:oxygen): Multiples of $4$ are divisible by $8$.

(\#cnj:oxen): For two real numbers $a$ and $b$, $|a||b| = |ab|$.

(\#cnj:oops): Every whole number greater than $2$ can be written as the difference of two perfect squares. (For example, $11 = 36 - 25, 12 = 16 - 4, 13 = 49 - 36$.)
  
(\#cnj:oodles): Every positive odd number can be written as the difference of two perfect squares.
  
(\#cnj:only): All triangles contain at least one angle measuring $\geq 60^{\circ}$.

(\#cnj:osh): All triangles contain at most one angle measuring $\geq 60^{\circ}$.
</div>\EndKnitrBlock{exercise}
</div>

If you fail to find a counterexample, maybe the conjecture is true. Or maybe you just weren't able to find a counterexample, even though one (or more) exists.^[This could be for a number of reasons, such as the the counterexample(s) are really really big, or maybe because you forgot to check all types of examples. Also, maybe you were just unlucky.] Because we don't know which, we move onto Step 2...

## Step 2: Try to build a proof

We don't know if the conjecture is true or false, but our attempts to disprove it by finding a counterexample failed. Our next step is to attempt to build a proof.

If the conjecture is true, we should be able to construct a proof to show this. If it is actually false, then as we build our proof we will find it breaks somehow. This would be called a disproof. Whilst finding a disproof is sufficient in showing the conjecture to be false, the disproof might make it easier to find a counterexample to the conjecture.

<div class="alert alert-warning" role="alert">
<strong>Note</strong> 

When trying to build a proof, be optimistic and believe that the conjecture *is* true.

Expecting the proof to fail is not a good mindset for effective proof building!

</div>

There are many different methods of proof we could build, and our choice will depend on the type of conjecture. We might have to try out several of the methods before we find the one that works. Also, different people might use different methods for the same conjecture. That's fine. As long as they both come to the same conclusion about the conjecture's truth value, the method used isn't important.

### If...then...
No matter what method you decide to start with, make sure the conjecture is in the form **If ... then ...**. If the conjecture is not in this form, rewrite it so that it is.

Why is the **If ... then ...**. form so important? The 'if' part signals the conjecture's starting point, and the 'then' part signals the conjecture's destination. It means we know where to begin our proof, and where we're headed whilst we're building the proof.

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-97"><strong>(\#exm:unnamed-chunk-97) </strong></span>Multiples of even numbers are even.

Rewritten in the  **If ... then ...** form, this conjecture becomes "**If** $a$ is an even number, **then** $ka$ is even, where $k \in \mathbb{Z}$".
</div>\EndKnitrBlock{example}

We use the letter $P$ to indicate the starting point of a conjecture, and the letter $Q$ to indicate the destination. So for the above conjecture:

Here are some more examples, taken from Exercise 6.1.1. The original conjecture is on the left, and the **If ... then ...** form on the right:

$P$: $a$ is an even number

$Q$: $ka$ is even, where $k \in \mathbb{Z}$

**Original conjecture** | **If ... then ...**
------------- | -------------
All prime numbers are odd | If $p$ is prime, then $p$ is odd
$(a + b)^2 = a^2 + b^2$ for any numbers $a$ and $b$ | If $a$ and $b \in \mathbb{R}$, then $(a + b)^2 = a^2 + b^2$ 
All sheep in South Africa are white | If a sheep lives in South Africa, then it is white
The national flags of all UN members are rectangular | If a country is a UN member, then its flag is rectangular
All numbers are either positive or negative | If $a \in \mathbb{R}$, then $a$ is either positive or negative
$a^2 > a$, where $a$ is a whole number | If $a \in \mathbb{Z}$, then $a^2 > a$

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-98"><strong>(\#exr:unnamed-chunk-98) </strong></span>For each example above, what is $P$? What is $Q$?
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-99"><strong>(\#exr:unnamed-chunk-99) </strong></span>For each of the six conjectures from Exercise 8.2:
  
a. Rewrite them in the **If ... then ...** form.
b. What is $P$ for each? And $Q$?
</div>\EndKnitrBlock{exercise}
</div> 

### Draw the map

Once the conjecture is in the form **If ... then ...**, you should attempt to draw the conjecture's **map**.

It's not always possible to draw a conjecture's map, but if you're able to it can *really* help you choose the most appropriate method of proof for that conjecture.

Here's the format of a conjecture map:

<img src="figures/maps1.png" width="45%" style="display: block; margin: auto;" />

Notice we start on the left side of the picture and finish on the right.

Next, we add $P$ and $Q$. We'll use the conjecture from above, "If $a$ is an even number, then $ka$ is even, where $k \in \mathbb{Z}$".

<img src="figures/maps2.png" width="50%" style="display: block; margin: auto;" />

You can see that $P$ has been added to the left side of the map and $Q$ to the right side. Above the map we write what type of number we're considering, in this case integers. Below the map, we write details of any variables (e.g. $k$) that the conjecture uses.

Next we add the **opposite of $P$** and the **opposite of $Q$** to the map.

What does the opposite mean? Well, in the example above, the numbers we're considering are the integers. We put the even ones in $P$, and all those which are not even (so odd) in $S$ (see below).

Similarly, if you multiply an integer $a$ (even or odd) by another integer ($k$), the result will be another integer. The even $ka$ we're storing in $Q$, and the odd $ka$ will go into $T$.

<img src="figures/maps3.png" width="50%" style="display: block; margin: auto;" />

Finally, we add **arrows** to the map to represent what the conjecture is saying. Arrows can only go from the left side of the map to the right side.

Therefore, the conjecture map of the statement 
"multiples of even numbers are even" is:

<img src="figures/maps4.png" width="50%" style="display: block; margin: auto;" />

This can all seem really confusing, but trying to draw a couple of conjecture maps yourself will really help.

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-104"><strong>(\#exr:unnamed-chunk-104) </strong></span>Draw the conjecture map for the following conjectures.

a. The square of a prime number is also prime.
b. Integers retain their parity when squared.
c. The sum of two consecutive integers is odd.
d. Numbers retain their sign when cubed.
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-105"><strong>(\#exr:unnamed-chunk-105) </strong></span>Draw the conjecture map of the conjecture from Exercise 8.2 (a), (c) and (d).
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-106"><strong>(\#exr:unnamed-chunk-106) </strong></span>Why is it difficult to draw a conjecture map for Exercise 8.2 (b), (e) and (f)?
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-107"><strong>(\#exr:unnamed-chunk-107) </strong></span>In class, we met the concept of dividing up a group of items into two smaller groups. If ALL the elements in the original groups are contained in one (or both) of the two smaller groups, we say the smaller groups are 'complete'. And if the two smaller groups don't share any elements, we say they are 'disjoint' from one another.
a. Our class.
b. The integer
</div>\EndKnitrBlock{exercise}
</div>

### Choose your method

Once you have written the conjecture in the form "If ... then ..." and have attempted (hopefully successfully) in drawing its map, you are ready to begin to try building a proof.

We have lots of choices of methods of proof available. In this course, we'll look at:

- proof by **exhaustion**, 
- **direct proof**, 
- proof by **cases**, 
- proof using **previously proved or disproved conjectures**, 
- proof via the **contrapositive**, 
- proof by **contradiction**, and 
- proof by **induction**.

Each of chapters 10 - 16 will cover one of these methods, and give you some examples to practice on.

At the end of each chapter there will be some more conjectures to work on. These conjectures might be true or might be false. To prove the true ones, you will be expected not just to rely on the method introduced in that chapter, but all previous methods too. This is because the challenge (and fun) of proving conjectures comes from not knowing where to start and feeling your own way to a proof. It's a very satisfying experience!^[Also, when presented with a set of conjectures and told to "Prove using a direct proof..." or "Prove by induction...", like a robot you will switch your brain off and switch on your autopilot, which we don't want!]

Chapter 17 is a bonus chapter, and covers the incompleteness of mathematics.

The next chapter, chapter 9, looks at what makes a good proof. 

<!--chapter:end:08-test.Rmd-->

# Before we start...

Prior to beginning to prove some conjectures, there are several questions which students always have, or difficulties that seem to arise. This chapter will address some of them.

## Why prove something?

We should ask ourselves why we should care about mathematical proof. (Hopefully you asked yourself this prior to taking this course!) Why are mathematics proofs important? This is a *big* question, which we won't pretend to be able to answer in just a few short paragraphs, but I'll mention a couple of my main reasons for caring about mathematical proof:

- A proof of a mathematical statement is absolute; there is no exception to the rule. They cannot be argued this way or that way, and no two people can come to different conclusions upon reading a mathematical proof. There is no "fake news", "alternative facts", or lies in mathematics. Such absolute statements are wonderful and do not exist in any other field of study

- Mathematics is EVERYWHERE! From music to the economy, from demographics to nature, from business to space travel, mathematics is used to help us reason about the world we live in. If we weren't able to apply mathematical theorems that we have proved to be true, we would not know much about the world around us.

- It is possible to know when you can not do better; for example, a cartographer wishing to use as few colours as possible to colour her maps can be told by a mathematician that four different colours will suffice to ensure no two adjacent areas are the same colour (this theorem is called the *Four Colour Theorem*}. Similarly mathematicians have been able to tell chemists when certain crystal structures have no mathematical obstructions (which led chemists to search for, and successfully produce, new crystal structures). There are numerous other examples of this kind.

- Mathematics isn't done simply to serve a purpose, however, or to support other fields. A mathematical proof precisely captures an idea, ideas which as well as being fundamental are often beautiful and elegant. These beautiful ideas deserve to be written down correctly.

## How do I write a good proof?

Here are some things to remember when writing proofs:

- Always use English (or Kyrgyz, Spanish, Russian, Arabic or whichever language you're writing your proof in) to clearly convey what you mean; good mathematical arguments should read like an essay. Whenever you write a proof, you should read through your answer and check to see if it could be read aloud and still be understood. 

- Label lines of work that you need to refer back to with reference numbers. In this course, you should also label the conjecture with the reference number from the textbook. End the proof with the $\square$ symbol to show you're done.

- Always clearly state your assumptions. This becomes extra important with the method proof by contradiction, and is key with the method proof by cases.

- Use words or symbols to correctly connect the mathematical statements which make up your proof (See the section below on the difference between the symbols $=$, $\Rightarrow$ and $\Leftrightarrow$.)

- Take pride in the mathematics you write; when you write a piece of mathematics, you are showing people *exactly* how you think. So, you should try to write as elegantly and beautifully as you can!

- Good mathematical proofs written by one person should be understandable by another. All terms should be clearly defined, and any variables used too.

- Proofs should be watertight, meaning that it shouldn't contain any holes - no one should be able to criticise you for not considering something. For example, if the conjecture concerns all whole numbers, your proof would not be valid if it only covers positive numbers. If the statement concerns all polygons, your proof would not be valid if it only covers triangles and squares.

- Proofs should always be as short and efficient as possible, whilst still being complete.

## How do I check my proof is correct?

Mathematicians can't check their own proofs, mainly because *they* wrote it. Have you ever tried to spot a mistake you've made in your own work? It can be really difficult to do! 

For a proof to be declared valid, it should be shared with your peers to check it. Germain did this, Mirzakhani did this, Euclid did this. In this course, you'll share your answers with me and with each other. 

Once your peers have approved it, you then can publish your proof as a piece of mathematics. It's at *this* point that you enter the history books and your mathematical proof remains valid for ever!

Note however, that as you move through the rest of this course, you will start to get a sense of when you have finished a proof. Knowing when a proof is finished, and when it is *not* finished, is a valuable skill you will develop.

## Common mistakes in proof

Here are some of the most common mistakes when writing proofs, all of which make your proof *invalid:

- **Arguing from examples:** Looking at examples is one of the most helpful practices a conjecture-prover can engage in. We discussed how useful it is to start with examples as a "way-in" to a new conjecture. However, it is a mistake to think that general statement can be proved by showing it to be true for some cases. For example, finding five right-angled triangles where Pythagoras' Theorem is true does not prove that the theorem is true for all right-angled triangles.
- **Using the same letter to mean two different things:** Often beginner conjecture provers give a new variable quantity the same letter name as a previously introduced variable. This will confuse your reader.
- **Assuming the thing to be proved is true:** If you are trying to prove something is true, you can’t assume it is true at the beginning of the proof. The reason for this is because assuming it true at the beginning might encourage you to use it as an established fact during your proof.^[A lawyer in court trying to prove a defendant guilty is not allowed to say, "Because we know the defendant is guilty, we know he can't have been where he says he was on the night of the crime. Because we know he is guilty, we know he was at the scene of the crime that night". No one in the jury is going to be convinced by this argument! The lawyer must find explicit evidence that the defendant was at the scene of the crime that night.]
- **Claiming something is true without having justified it:**. This is also called “jumping to a conclusion”.
<!-- - **Using “any” when you mean “some” -->
<!-- - For example, *any* multiple of 5 ends with 5 versus *some* multiples of 5 end with 5. -->
<!-- **Using “if” when you mean “because”** -->

The first of these means you haven't actually started a proof. The second is not too much of a problem and is easily rectified. The last two would mean you have started a proof but that it contains fundamental problems. Both of these two are a headache to mathematicians and conjecture-provers around the world!

## $=$, $\Rightarrow$ and $\Leftrightarrow$

Finally, we discuss the important mathematical symbols "$\Rightarrow$", "$\Leftrightarrow$" and "$=$", and how they should be used in proofs.

### The equals sign

The equals sign, "$=$", is used to denote an equality between mathematics expressions (not statements). So for example, 

\begin{align}
  1+1=2
\end{align}

or

\begin{align}
  \sin^2 \theta + \cos^2 \theta = 1
\end{align}

### The implies sign

The implies sign, "$\Rightarrow$", is used to denote when one mathematical statement follows directly from another. For example

\begin{align}
  x &= 3 \Rightarrow x^2 = 9
\end{align}

which is read "if $x$ equals three then $x$ squared equals nine". Note that it would be wrong to write

\begin{align}
  x^2 = 9 \Rightarrow x &= 3
\end{align}

as $x^2 = 9$ doesn't mean that $x$ is definitely $3$ (it could be $-3$).

### The equivalence sign

The equivalence sign, "$\Leftrightarrow$", is used to denote the equivalence of two mathematical statements. If $A$ and $B$ are mathematical statements, then writing $A \Leftrightarrow B$ means that both $A \Rightarrow B$ and $B \Rightarrow A$ are true. For example,

\begin{align}
    x - 1 &= 0 \Leftrightarrow x = 1
\end{align}

Note that it would be wrong to write

\begin{align}
    x^2 &= 9 \Leftrightarrow x = 3
\end{align}

but correct to write

\begin{align}
    x^2 &= 9 \Leftrightarrow x = \pm 3
\end{align}

## Example

Let's look at an example of a good proof and a bad proof. Both are trying to prove the following conjecture:

(\#cnj:red): If $a$ and $c$ are positive real numbers and $x = \pm \sqrt{\frac{c}{a}}$, then $ax^2-c=0$.

A couple of observations first. Note that $a, c >0$ implies that $a \neq 0$, which is important as it's the denominator of the fraction $\frac{c}{a}$. This means that $\frac{c}{a}$ is defined. Also note that $a, c > 0$ implies that $\frac{c}{a} > 0$ which is important as it is under a square root. This means that $\sqrt{\frac{c}{a}}$ is defined.

### A good proof

First, the good proof.

\BeginKnitrBlock{proof}<div class="proof">\iffalse{} <span class="proof"><em>Proof. </em></span>  \fi{}Our starting point $P$ is $x = \pm \sqrt{\frac{c}{a}}$, with $a, c \in \mathbb R^+$.
  If
\begin{align}
  x &= \pm \sqrt{\frac{c}{a}}(\#eq:abe)
\end{align}
  then squaring both sides, meaning both sides are positive and equivalent, gives
\begin{align}
  x^2 &= \left(\pm \sqrt{\frac{c}{a}} \right)^2 (\#eq:chick) \\
  &= \frac{c}{a} (\#eq:maybe)
\end{align}
  Multiplying both sides by $a$, which we can do as $a\neq 0$, we get
\begin{align}
  ax^2 &= c (\#eq:load) \\
  ax^2 - c &= 0 (\#eq:neigh)
\end{align}
  We have shown that $x = \pm \sqrt{\frac{c}{a}}\Rightarrow ax^2 - c = 0$ as required.
</div>\EndKnitrBlock{proof}

Here are a couple of things to notice:

- This conjecture was not difficult to prove, so the proof shouldn't be overly complicated. The presentation above demonstrates how to write a clear, comprehensive, cohesive and rigorous (watertight) argument.

- We label the conjecture with its reference number from the textbook, in this case "Conjecture \@ref(cnj:red)", so that if we need to we can refer back to it and its proof/disproof later. As we'll see in a later chapter, we often use work we've done previously, and having a quick way to refer back to previous conjectures and their proofs/disproof can speed this up for us!
    
- Every line in the proof above is labelled with a reference number: \@ref(eq:abe), \@ref(eq:chick), \@ref(eq:maybe), \@ref(eq:load), \@ref(eq:neigh). In your proofs, you probably won't need or want to label every line of work, but you should label important lines, ones which you use later in the proof (or even later in proofs of other conjectures!)

- Notice that we used the $\square$ symbol to indicate that we consider the proof is finished.

### A bad proof

Now for the bad proof.

\BeginKnitrBlock{proof}<div class="proof">\iffalse{} <span class="proof"><em>Proof. </em></span>  \fi{}
\begin{align}
  ax^2 + c &= x^2 + \frac{c}{a} = 0 (\#eq:water) \\
  &= x \Rightarrow \pm \sqrt{\frac{c}{a}} (\#eq:fire)
\end{align}
which completes the proof.
</div>\EndKnitrBlock{proof}

You can probably see very easily that this second proof is far from perfect. However, you might argue that the person who wrote the answer more or less knew what they meant. For example, they know "why" $x = \pm \sqrt{\frac{c}{a}}\Rightarrow ax^2 - c = 0$. The question then is, what's wrong with this proof? 

- Firstly, it is really hard for the reader to follow. 

- Secondly, when you, the author, are not absolutely clear about what your assumptions are, or don't properly justify implications, it is easy to run into trouble. 

Here's another example which demonstrates this:

Let
\begin{align}
  x=y
\end{align}
  As $x=y$,
\begin{align}
    y(x-y) &= x(x-y) (\#eq:noone)
\end{align}
  Also,
\begin{align}
    & x(x-y) = x^2 - xy - x^2 - y^2 = (x+y)(x-y) = 2y(x-y) (\#eq:reign)
\end{align}
  So,
\begin{align}
  y(x-y) &= 2y(x-y) (\#eq:rain)
\end{align}
  and so
\begin{align}
  1 &= 2 (\#eq:decide)
\end{align}

<!-- ## Exercises -->

<div class="alert alert-danger" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-110"><strong>(\#exr:unnamed-chunk-110) </strong></span>Look back at the "bad proof" above. Based on everything you've read in this chapter, how many things can you find to criticise about this proof?
</div>\EndKnitrBlock{exercise}
</div>


<!-- <div class="alert alert-info" role="alert"> -->
<!-- ```{exercise} -->
<!-- Prove the following conjecture using the good proof practices outlined above. -->
<!-- ```  -->


<!-- (\#cnj:blue): If $a, b, c \in \mathbb R$, with $a\neq 0$, $b^2 - 4ac > 0$ and $x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$, then $ax^2 + bx + c = 0$. -->

<!-- ```{exercise} -->
<!-- What is wrong with the following argument? -->

<!-- *Proof:* Let -->
<!-- \begin{align} -->
<!--   x &= 1 + 1 + ... + 1 \text{ (so there are $x$ 1's)} (\#eq:last)  -->
<!-- \end{align} -->
<!--   Multiplying both sides of equality \@ref(eq:last) by $x$ we get: -->
<!-- \begin{align} -->
<!--   x^2 &= x + x + ... + x (\#eq:yellow)  -->
<!-- \end{align} -->
<!--   Differentiating both sides of equality \@ref(eq:yellow) with respect to $x$ we get -->
<!-- \begin{align} -->
<!--   2x &= 1 + 1 + ... + 1 (\#eq:knew) \\ -->
<!--   &= x (\#eq:pepper)  -->
<!-- \end{align} -->
<!--   Divide both sides of equality \@ref(eq:knew) by $x$, we conclude that -->
<!-- \begin{align} -->
<!--   2 &= 1  (\#eq:salt) -->
<!-- \end{align} -->

<!-- ```  -->

<!-- </div> -->

<!-- And proof by smallest counterexample: https://math.libretexts.org/Bookshelves/Mathematical_Logic_and_Proof/Book%3A_Book_of_Proof_(Hammack)/10%3A__Mathematical_Induction/10.03%3A_Proof_by_Smallest_Counterexample -->

<!-- Select text, then Shift Ctrl and C to comment it out. -->

<!--chapter:end:09-test.Rmd-->

# The flowchart of proof

The picture below summarises everything we've covered in the first nine chapters. You should follow this flowchart to set up and conduct mathematical proof.


<div class="figure" style="text-align: center">
<img src="figures/flowchart_for_proof.png" alt="The flowchart of proof." width="100%" />
<p class="caption">(\#fig:unnamed-chunk-111)The flowchart of proof.</p>
</div>

<!--chapter:end:10-test.Rmd-->

# Proof by exhaustion

<div class="alert alert-warning" role="alert">
<strong>Note: You should be familiar with the flowchart of proof in Chapter 10 before reading this chapter.
</strong> 
</div>

Welcome to our first method of proving conjectures! The method is called **Proof by Exhaustion**. 

This doesn't mean you do it until *you* are exhausted. Rather, you do it until all possibilities are exhausted. It is closely related to the method presented in Chapter 14 called Proof by Cases.

Part of the skill of mathematical proof is identifying the most appropriate method for any specific conjecture. Considering this, let's look at some conjectures for which proof by exhaustion *is* appropriate, and some for which it is *not*.


**Conjecture** | **If true, how to prove by exhaustion?** | **Practical?**
------------- | ------------- | -------------
No Chinese citizen has green eyes | Check eye colour of every Chinese citizen | No, as there's too many
All Irish citizens have a vowel in their surname | Check a database of Irish citizens | Possibly
There is no integer $a$ such that $a^2 + a^3 = 100$ | Check possible integers | Yes, as there are only so many integers which could work here.
The sum of the digits of a multiple of $9$ is itself a multiple of $9$ | Check all multiples of $9$ | No, as there's infinite number of them
For any right-angle triangle with hypotenuse $a$ and legs $b$ and $c$, $a^2 = b^2 + c^2$ | Check every possible right-angle triangle | No, as there's infinite number of them

Using this method when there are too many cases, as in (1) and (4), will take far too long, unless you've got a quick or systematic way to carry out the check, as in (2). This method works best for conjectures where the number of possibilities is low, as in (3).^[Unless we could prove that there exist only a limited (and small) number of "families" of right-angled triangles. We'll return to this example later, but for now it seems unlikely to be suitable for a proof by exhaustion.]

## Steps

1. Identify and list all possibilities.
2. Prove that your list definitely contains all possibilities (i.e. you haven't forgotten any).
3. Show that the conjecture is true for each of the possibilities on your list.

## Formal definition

To prove "If $P$ then $Q$" by exhaustion, show that

<center>

If $P_1$ then $Q$.

If $P_2$ then $Q$.

$\vdots$

If $P_n$ then $Q$.

</center>

where $P_1$, $P_2$, ..., $P_n$ are all possible (finitely many) values of $P$.

## Conjectures

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-112"><strong>(\#exr:unnamed-chunk-112) </strong></span>Use the following examples to practise.

* In our next class, you'll be given a new set of conjectures to prove using this method.

* Follow the flowchart in Chapter 10 (for example, if the conjecture is not in the form **If ... then ...**, make sure you rewrite it before starting the proof). 

* Solutions are included underneath the exercise. Attempt the proof before checking the solutions.
  
(\#cnj:nigh): If $2 \leq a \leq 7$ and $a \in{\mathbb Z}^+$, then $4 \nmid a^2 + 2$.

(\#cnj:thru): There is a prime number between $8$ and $12$.

(\#cnj:exit): No square number ends in $8$.

(\#cnj:send): $97$ is a prime number.
</div>\EndKnitrBlock{exercise}
</div> 

***

***Solutions:***

***

Conjecture \@ref(cnj:nigh): See
https://www.youtube.com/watch?v=ifMZt4l5JIM. Alternatively https://www.youtube.com/watch?v=YmbTI91TUp4.

***

Conjecture \@ref(cnj:thru): See
https://www.youtube.com/watch?v=eQM778zoB14.

***

Conjecture \@ref(cnj:exit): Watch 0:00-4:20 of https://www.youtube.com/watch?v=k0f7w4xTp1I.

***

Conjecture \@ref(cnj:send): See https://www.youtube.com/watch?v=1amtOenZEwU.

***

<!-- There is no integer $a$ such that $a^2 + a^3 = 100$. -->

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-113"><strong>(\#exr:unnamed-chunk-113) </strong></span>Some of these conjectures below are false; **disprove them by finding a counterexample**. Some of them are true; **prove them by exhaustion**. Follow the flowchart in Chapter 10 to help you.

(\#cnj:syndrome): There is no two-digit number which is both a perfect square *and* a perfect cube.

(\#cnj:crush): If $p$ is a prime number and $p > 5$, then $p^4$ ends in 1. *(Hint here: https://www.youtube.com/watch?v=Q_UdUwm3Biw.)*

(\#cnj:defeat): There is no three-digit number which is a perfect square.

(\#cnj:frighten): There is no perfect square between 4100 and 4200.

(\#cnj:rich): $(a + 1)^3\geq 3^a$ for $a\in{\mathbb Z^+}$, $a\leq 4$.

(\#cnj:dive): The product of two non-integers is never an integer.

(\#cnj:stun): No integer greater than 2, when written in English with the Latin alphabet, has more letters than the number itself. *(Think carefully about which numbers need to be included on your list of possibilities here.)*

(\#cnj:dirty): No integer greater than 2, when written in Russian using the Cyrillic alphabet, has more letters than the number itself. *(Again, think carefully about which numbers need to be included on your list of possibilities here.)*

(\#cnj:nest): If $p$ is a prime number such that $3 \leq p \leq 23$, then $8 \mid (p+1)(p-1)$.

(\#cnj:cupboard): Every positive integer up to and including 28 is at least one of the following: prime, perfect, triangular, or can be written as $b^c$, where $b\in{\mathbb Z}$ and $c\in{\mathbb Z^+}$, $c > 1$.
  
(\#cnj:study): Every integer between 20 and 30 (inclusive) can be written as the sum of *exactly* five **non-zero** square numbers.

(\#cnj:curl): If $x$ is a positive integer less than 5, the last digit of $x^5$ is $x$.

(\#cnj:drag): There are fewer square numbers below 50 than prime numbers.

(\#cnj:junior): Every even integer between (and including) 4 and 30 can be written as a sum of two primes.

(\#cnj:world): The sum of two distinct square numbers is a square number. *(**Distinct** means the two square numbers can't be the same.)*

(\#cnj:landscape): For $x, y, a \in \mathbb R$, if $x > y$ then $ax > ay$.

(\#cnj:write): It's impossible to move a knight from one corner of a chess board to the corner diagonally opposite in 4 moves. *(You don't play chess? Look up online how a **knight** moves.)*

(\#cnj:wash): Each integer in the set 2, 4, 6, 8, ..., 24, 26 can be written the sum of *at most* three perfect squares.

(\#cnj:cat): There are no integers $a$, $b$ and $c$ such that $(1+\frac{1}{a})(1+\frac{1}{b})(1+\frac{1}{c}) = 2$.

(\#cnj:refund): If the sum of two integers is even, then at least one of the summands is even. *(Don't know what a **summand** is? Have a search online...)*

(\#cnj:snitch): The sum of two consecutive perfect squares between 100 and 200 is an odd number.

(\#cnj:crumple): The sum of any two distinct perfect squares between 100 and 200 is an odd number.

</div>\EndKnitrBlock{exercise}
</div> 

<!--chapter:end:11-test.Rmd-->

# Direct proof

<div class="alert alert-warning" role="alert">
<strong>Note: You should be familiar with the flowchart of proof in Chapter 10 before reading this chapter.
</strong> 
</div>

Welcome to our second method of proving conjectures: **direct proof**. 

Direct proofs use algebra to move from $P$ to $Q$. 

## Steps

1. Make sure the conjecture is in the form **If ... then ...**. This is good practice for any method of proof, but especially direct proof. 

2. What do you know? What information does $P$ give you? What do you know about the subject of the conjecture?

3. How can what you know get you to the conclusion you need to make, $Q$? 

<div class="alert alert-warning" role="alert">
<strong>Be aware!
</strong> 

- You might have to try out different routes from $P$ until you find one that gets you to $Q$.

- It is wrong to use $Q$ in your proof. You of course should use it to guide your work, like a goal to reach, but $Q$ isn't a tool to be used in a direct proof. (See **Assuming the thing to be proved is true** in Chapter 9, section 4.)
</div>

## Formal definition

Simply, prove that "If $P$ then $Q$".

## Conjectures

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-114"><strong>(\#exr:unnamed-chunk-114) </strong></span>Use the following examples to practise. Solutions are below.
  
(\#cnj:wave): The sum of two even numbers is even.

(\#cnj:welcome): The square of an odd number is also odd.

(\#cnj:wood): The sum of the first $n$ positive integers is $\frac{n}{2}(n+1)$.

(\#cnj:weapon): For any four consecutive integers, the difference between the product of the last two and the product of the first two of these numbers is equal to their sum.
</div>\EndKnitrBlock{exercise}
</div> 

***

***Solutions:***

***

Conjecture \@ref(cnj:wave): First, we rewrite the conjecture,

<center> If $a$ and $b$ are even integers, then $a+b$ is even. </center>

Now we're ready for a direct proof.

\BeginKnitrBlock{proof}<div class="proof">\iffalse{} <span class="proof"><em>Proof. </em></span>  \fi{}Since $a$ and $b$ are even, they can be written as
\begin{align}
    a &= 2k \\
    b &= 2l
\end{align}
where $k$ and $l$ are integers. Therefore the sum of $a$ and $b$ is
\begin{align}
    a + b &= 2k + 2l\\
    &= 2(k + l)
\end{align} 
by factoring out 2.

As the sum of integers equals an integer, $k + l$ must equal some integer. Let's call it $m$. Therefore we have
\begin{align}
    a + b &= 2m
\end{align}
which is clearly even.</div>\EndKnitrBlock{proof}

***

Conjecture \@ref(cnj:welcome): First, we rewrite the conjecture,

<center> If $a$ is an odd integer, then $a^2$ is odd. </center>

Now we're ready for a direct proof.

\BeginKnitrBlock{proof}<div class="proof">\iffalse{} <span class="proof"><em>Proof. </em></span>  \fi{}If $a$ is an odd integer, it can be expressed as
\begin{align}
    a &= 2k + 1 
\end{align}
where $k$ is an integer. Squaring our odd number, we get
\begin{align}
    a^2 &= (2k + 1)^2 \\
    &= 4k^2 + 4k +1  \\
    &= 2(2k^2 + 2k) +1 (\#eq:bessie) 
\end{align}
As $2k^2$ is an integer and $2k$ is an integer, $2k^2 + 2k$ is an integer, which we'll call $l$. Therefore Equality  \@ref(eq:bessie)  becomes
\begin{align}
    a^2 &= 2l+1  
\end{align}
and $a^2$ is therefore odd.</div>\EndKnitrBlock{proof}

***

Conjecture \@ref(cnj:wood): See https://www.youtube.com/watch?v=aaFrAFZATKU.

***

Conjecture \@ref(cnj:weapon): First, we rewrite the conjecture,

<center> If four integers are consecutive, then the difference between the product of the </center>
<center> last two and the product of the first two of these numbers is equal to their sum. </center>

Now we're ready for a direct proof.

\BeginKnitrBlock{proof}<div class="proof">\iffalse{} <span class="proof"><em>Proof. </em></span>  \fi{}Four consecutive integers can be write as $a, a+1, a+2, a+3$.

Then the product of the first two will be

\begin{align}
    a(a+1) &= a^2 + a (\#eq:bernie)
\end{align}

and the product of the last two will be

\begin{align}
    (a+2)(a+3) &= a^2 + 5a + 6 (\#eq:betty)
\end{align}
    
The difference between Equality \@ref(eq:betty) and Equality \@ref(eq:bernie) is
\begin{align}
    (a^2 + 5a + 6) -  (a^2 + a) &= 4a + 6  (\#eq:bess)
\end{align} 

We need to show this Equality \@ref(eq:bess) is the same as the sum of the four numbers, which is

\begin{align}
    a + a+1 + a+2 + a+3 &= 4a + 6
\end{align}

As this is the same as Equality \@ref(eq:bess), we are done.
</div>\EndKnitrBlock{proof}
<!--   (\#eq:betty) (\#eq:bertie)  -->

***

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-118"><strong>(\#exr:unnamed-chunk-118) </strong></span>Some of these conjectures are false; disprove them by finding a **counterexample**. Some of them are true; prove them using a proof by **exhaustion** (from last class) or a **direct proof** (from this class).

(\#cnj:waste): If $a$ and $b$ are both perfect squares, then $ab$ is also a perfect square.

(\#cnj:web): The sum of two odd integers is even.

(\#cnj:waiter): All odd primes end with 1, 3, 7 or 9.

(\#cnj:wrap): If $a$ and $b$ are both odd, then the difference of their squares is even. *(This means if you square two odd numbers and find the difference between these two squares, the difference will be even.)*

(\#cnj:worth): The sum of two consecutive integers is odd.

(\#cnj:worry): The sum of three consecutive integers is odd.

(\#cnj:workshop): The sum of three consecutive integers is divisible by 3.

(\#cnj:witch): The sum of three consecutive odd numbers is divisible by 3.

(\#cnj:war): The sum of two consecutive odd numbers is divisible by 4.

(\#cnj:withdraw): For a right-angled triangle, the square of the hypotenuse is equal to the sum of the squares of the other two sides. This is the *Pythagoras Theorem*. Prove it algebraically with a direct proof using the picture below.
</div>\EndKnitrBlock{exercise}

<img src="figures/Diagram_of_Pythagoras_Theorem_simplified.png" width="45%" style="display: block; margin: auto;" />

(\#cnj:woman): The product of three consecutive integers is divisible by 6.

(\#cnj:wealth): There is no four-digit number that reverses its digits when multiplied by 4 (in other words, ABCD x 4 = DCBA).

(\#cnj:window): Summing two 3-digit numbers results in a 4-digit number.

(\#cnj:weed): If a number is divisible by 4, then it is divisible by 2.

(\#cnj:wander): If a number is divisible by 2, then it is divisible by 4.

(\#cnj:word): If $a$ is a positive nonprime whole number and some prime number $p$ divides $a$, then some other prime $q$ ($q \neq p$) also divides $a$.

(\#cnj:warrant): If $a + 4 > 0$, then $a$ is positive.

(\#cnj:wake): For any negative number $a$, $a^2 > a$.

(\#cnj:wreck): If $a^2$ is divisible by $2$, then so is $a$.

(\#cnj:worm): If $a^2$ is divisible by $3$, then so is $a$.

(\#cnj:whizz): To multiply a two-digit number by $11$, simply add the two digits of the number togetheIf the sum of the two digits is $10, 11, 12, ..., 19$, carry the one over to the first number.r, then insert it in between the two digits.  <br /> *For example $11 \times 11 = 121$, $23 \times 11 = 253$,  $77 \times 11 = 847$.*

(\#cnj:wend): In the picture below, the larger square is twice the area of the smaller square.

<div class="figure" style="text-align: center">
<img src="figures/sqinacircinasq.png" alt="The figure shows a square **inscribed** in a circle, which is **inscribed** in another square." width="45%" />
<p class="caption">(\#fig:unnamed-chunk-120)The figure shows a square **inscribed** in a circle, which is **inscribed** in another square.</p>
</div>

</div>

<!--chapter:end:12-test.Rmd-->

# Proof by cases

Our third method of proof is called **proof by cases**. Proving something by cases is very similar to proving something by exhaustion. 

## Steps

The steps in a proof by cases are similar to those in a proof by exhaustion:

1. Perform a partition of $P$ into cases. <br /> *Note that a partition of $P$ into "*cases*" is similar to the list of possibilities you create for a proof by exhaustion, except that cases are generally more broad (usually containing multiple elements) than each single possibility in a proof by exhaustion.*

2. Show that the conjecture is true for each of the cases on your list. <br /> *In a proof by exhaustion, you had to show that the conjecture was true for each possibility, which usually required testing just a single number. Similarly for a proof by cases, you need to show that $P \rightarrow Q$ for each case, but as cases generally contain more elements, something like a direct proof will be needed for each case.*

<!-- For example, while the list of possibilities in a proof by exhaustion might be each whole number from 1 to 20 or each possible route taken by a knight on a chessboard, the cases in a proof by cases might be *all* negative numbers and *all* non-negative numbers, or *all* even integers between 1 and 20 and *all* odd integers between 1 and 20, or *all* whole numbers and *all* non-whole numbers. -->

Here are some examples of how you might split up a proof into cases (Step 1), depending on what type of number the conjecture concerns:

**Family** | **Possible cases** 
------------- | ------------- 
$a \in \mathbb Z$ | **Case 1:** $a$ is even <br /> **Case 2:** $a$ is odd <br /> <br /> **Case 1:**  $a = 3k$ <br /> **Case 2:** $a = 3k + 1$ <br /> **Case 3:** $a = 3k + 2$ <br /> with $k \in \mathbb Z$ <br /> In other words, every integer is either a multiple of $3$, one more than a multiple of $3$, or two more than a multiple of $3$. <br /> <br /> **Case 1:** $a$ is positive <br /> **Case 2:** $a$ is negative <br /> **Case 3:** $a$ = 0
$a \in \mathbb R$ | **Case 1:** $a$  is rational <br /> **Case 2:** $a$ is irrational <br /> <br /> **Case 1:** $|a| > 1$ <br /> **Case 2:** $|a| \leq 1$ <br /> <br /> **Case 1:** $a$ is positive <br /> **Case 2:** $a$ is negative <br /> **Case 3:** $a$ = 0
Pairs of numbers $a, b$ | **Case 1:** both $a, b > 0$ <br /> **Case 2:** both $a, b < 0$ <br /> **Case 3:** $a > 0$ and $b < 0$ (w.l.o.g.^[See Chapter 14 for more on w.l.o.g.]) <br /> **Case 4:** at least one of $a$ and $b$ equals 0 <br /> <br /> **Case 1:** $a,b \neq 0$ <br /> **Case 2:** at least one of $a$ and $b$ equals 0

<div class="alert alert-danger" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-121"><strong>(\#exr:unnamed-chunk-121) </strong></span>Verify that for each of the examples given in the table above, the cases are **distinct** and **complete** (i.e. they form a partition).
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-122"><strong>(\#exr:unnamed-chunk-122) </strong></span>Can you think of any other possible cases for the families of numbers in the table?
</div>\EndKnitrBlock{exercise}
</div>

<div class="alert alert-warning" role="alert">
<strong>Note:
</strong> 

- You might partition $P$ into cases differently to a classmate. Don't worry! There are many ways to prove the same thing - just make sure you don't miss any numbers! 
<!-- For example, if $P$ says $a$ is an integer and -->

<!-- - you split the proof into positive integers and negative integers, then you have forgotten to consider $a = 0$, and your cases are not complete. You will have to amend one of the two cases to include $a = 0$, or add it as its own case.  -->

<!-- - you split the proof into cases $a \geq 0$ and $a \leq 0$, then 0 is contained in both cases, meaning the cases overlap, which also isn't good. You should amend one of the cases so it no longer includes 0. -->

- Once you have partitioned $P$ into cases, consider each case separately from one another. 

- For conjectures in this course that require a proof by cases, you will probably need 2, 3, or maybe 4 cases. However, there is no upper limit for how many you can use. Proofs involving between 5 and 10 cases are common. You should always try to use the smallest number of cases possible.^[The first proof of the *Four Colour Theorem* used 1936 cases. Since then, mathematicians have managed to reduce this number to close to 600, which is still a lot, but less than 1936! <br /> The Four Colour Theorem states that any map, like a map of the states of the U.S. or countries of the world, can be coloured using only four colours in such a way that regions sharing a common boundary (other than a single point) do not share the same colour. In other words, a cartographer knows that she needs only four colours to colour *any* map. See https://www.cantorsparadise.com/the-four-color-theorem-8eece6ab6b12.]

</div>

## Formal definition

To prove "If $P$ then $Q$" by cases, show that

<center>

If $P_1$ then $Q$.

If $P_2$ then $Q$.

$\vdots$

If $P_n$ then $Q$.

</center>

where $P_1$, $P_2$, ..., $P_n$ is a partition of $P$.

## Exhaustion versus cases

Let's compare a couple of conjectures we previously proved by exhaustion and a couple which can be proved using cases, to see the difference between "*possibilities*" in a proof by exhaustion and "*cases*" in a proof by cases.

**Conjecture** | **Proof by exhaustion** | **Proof by cases**
------------- | ------------- | -------------
Conjecture 11.4 (from Chapter 11) | The video solution identified four possible divisors of $97$ (using some clever reasoning about prime numbers and the square root of $97$ to not identify more possibilities than necessary) and then checked them all. Finding none divided $97$, and being satisfied that this list of candidate divisors was complete, the conjecture was declared true. <br /> **List of possibilities:** $2, 3, 5, 7$. |
Conjecture 11.3 (from Chapter 11) | In the video solution, the list of possibilities was identified as the integers $0, 1, 2, 3, ..., 9$. Again, this list was long enough to ensure completeness but not longer than it needed to be. <br /> **List of possibilities:** $0,1,2,3,4,5,6,7,8,9$. |
(\#cnj:hobby): Integers retain their parity when squared. || We should first check the conjecture is true for even integers, then check it's true for odd integers.  <br /> **Partition of $a \in \mathbb Z$ into cases:**  <br /> **Case 1:** All even integers. <br /> **Case 2:** All odd integers. 
(\#cnj:haunt): There is no integer $a$ such that $a^2 + a^3 = 100$. | | **Partition of $a \in \mathbb Z$ into cases:**  <br /> **Case 1:** $a \in \mathbb Z^-$ <br /> **Case 2:** $a=0$ <br /> **Case 3:** $1 \leq a \leq 4$ <br /> **Case 4:** $a \geq 5$  
(\#cnj:have): For $a, b \in \mathbb R$, $|a + b| \leq |a| + |b|$. || As we're dealing with the modulus function^[Recall the modulus function: $|a| = a$ for $a \geq 0$, and $|a| = -a$ for $a < 0$.], it  makes sense to build cases by varying the sign of $a$ and $b$. <br /> **Partition of $a \in \mathbb R$ into cases:**  <br /> **Case 1:** $a$ and $b$ both $\geq 0$. <br /> **Case 2:** $a$ and $b$ both $< 0$. <br /> **Case 3:** $a \geq 0$, $b <0$, $|a| \geq |b|$. <br /> **Case 4:** $a \geq 0$, $b <0$, $|a| < |b|$. 
(\#cnj:hallway): All perfect squares are either a multiple of $3$ or one more than a multiple of $3$. | | See **Exercise 13.3** below.

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-123"><strong>(\#exr:unnamed-chunk-123) </strong></span>What do you think for Conjecture \@ref(cnj:hallway)? What cases should we use?
  
*Solution: See below for my suggestion of cases for this conjecture.*
</div>\EndKnitrBlock{exercise}
</div>

## Conjectures

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-124"><strong>(\#exr:unnamed-chunk-124) </strong></span>We have already met the following four conjectures above. Use them to practice the method of proof by cases. Solutions are below, as usual. 
  
(\#cnj:hobby): Integers retain their parity when squared.

(\#cnj:haunt): There is no integer $a$ such that $a^2 + a^3 = 100$.

(\#cnj:have): For $a, b \in \mathbb R$, $|a + b| \leq |a| + |b|$.

(\#cnj:hallway): All perfect squares are either a multiple of $3$ or one more than a multiple of $3$.
  
**Also, watch 0:00-9:30 of this video for a couple more examples of proof by cases:** https://www.youtube.com/watch?v=dheuJkuSNyI.
</div>\EndKnitrBlock{exercise}
</div> 

***

***Solutions:***

***

Conjecture \@ref(cnj:hobby): First, we rewrite the conjecture,

<center> If $a$ is an even integer, then $a^2$ is an even integer. <br /> If $a$ is an odd integer, then $a^2$ is an odd integer.  </center>

Now we're ready for a proof by cases. We'll use a direct proof within each of the two cases.

\BeginKnitrBlock{proof}<div class="proof">\iffalse{} <span class="proof"><em>Proof. </em></span>  \fi{}<br />
**Case 1:** $a$ even

Since $a$ is even, it can be written as
\begin{align}
    a &= 2k
\end{align}
where $k$ is an integer.

Then,
\begin{align}
    a^2 &= (2k)^2 \\
    &= 4k^2 \\
    &= 2(2k^2)
\end{align} 
by factoring out $2$.

$2k^2$ is clearly an integer. Let's call it $m$. Therefore we have
\begin{align}
    a^2 &= 2m
\end{align}
which is clearly even.

**Case 2:** $a$ odd

Since $a$ is odd, it can be written as
\begin{align}
    a &= 2k + 1
\end{align}
where $k$ is an integer. (Note that we are allowed to reuse the letter $k$ as cases are separate from one another.)

Then,
\begin{align}
    a^2 &= (2k + 1)^2 \\
    &= 4k^2 + 4k + 1 \\
    &= 2(2k^2 + 2k) + 1
\end{align} 
by factoring out $2$.

$2k^2 + 2k$ is clearly an integer. Let's call it $m$. Therefore we have
\begin{align}
    a^2 &= 2m + 1
\end{align}
which is clearly odd.
</div>\EndKnitrBlock{proof}

***

Conjecture \@ref(cnj:haunt): First, we rewrite the conjecture,

<center> If $a \in \mathbb Z$, then $a^2 + a^3 \neq 100$.  </center>

Now we're ready for a proof by cases.

\BeginKnitrBlock{proof}<div class="proof">\iffalse{} <span class="proof"><em>Proof. </em></span>  \fi{}<br />
**Case 1:** $a \in \mathbb Z^-$ <br /> 
For all negative integers $a^2 + a^3 \leq 0$, as $|a^3| \geq |a^2|$ and $a^3 < 0$. 
  
**Case 2:** $a=0$ <br /> 
$0^2 + 0^3 = 0 \neq 100$.
  
**Case 3:** $1 \leq a \leq 4$ <br /> 
We'll use proof by exhaustion for these four possibilities.

If $a=1$ then $a^2 + a^3 = 2 \neq 100$. <br />
If $a=2$ then $a^2 + a^3 = 12 \neq 100$. <br />
If $a=3$ then $a^2 + a^3 = 36 \neq 100$. <br />
If $a=4$ then $a^2 + a^3 = 80 \neq 100$. <br />
  
**Case 4:** $a \geq 5$  <br /> 
As $5^2 + 5^3 = 150 > 100$, all integers from $5$ and up will be too large for $a^2 + a^3$ to equal $100$.
</div>\EndKnitrBlock{proof}

***

Conjecture \@ref(cnj:have): First, we rewrite the conjecture,

<center> If $a, b \in \mathbb R$, then $|a + b| \leq |a| + |b|$.  </center>

Now we're ready for a proof by cases.

\BeginKnitrBlock{proof}<div class="proof">\iffalse{} <span class="proof"><em>Proof. </em></span>  \fi{}<br />
**Case 1:** $a$ and $b$ both $\geq 0$ <br />
Since $a,b \geq 0$, we know that $|a| = a$ and $|b| = b$. Also, as $a+b \geq 0$, we know that $|a+b| = a+b$. We have,
\begin{align}
    |a + b| &= a + b
\end{align}
and
\begin{align}
    |a| + |b| &=  a + b
\end{align}
Therefore $|a + b| = |a| + |b|$, which satisfies the conjecture.

**Case 2:** $a$ and $b$ both $< 0$ <br />
Since $a,b <0$, we know that $|a| = -a$ and $|b| = -b$. Also, as $a+b <0$, we know that $|a+b| = -(a+b)$. We have,
\begin{align}
    |a + b| &= -(a + b) \\
  &= -a - b
\end{align}
and
\begin{align}
    |a| + |b| &=  -a - b
\end{align}
Therefore $|a + b| = |a| + |b|$, which satisfies the conjecture. 

**Case 3:** $a \geq 0$, $b <0$, $|a| \geq |b|$  <br />
Since $a \geq 0$, $|a| = a$. Since $b<0$, we know that $|b| > 0$. 

Thus 
\begin{align}
    |a| + |b| &> a
\end{align}

As $b<0$ and $|a| \geq |b|$, we know that
\begin{align}
    |a + b| &< a
\end{align}
Therefore $|a + b| < a < |a| + |b|$, which satisfies the conjecture. 

**Case 4:** $a \geq 0$, $b <0$, $|a| < |b|$ <br />
Since $a \geq 0$, $|a| = a$. Since $b<0$, $|b| = -b$.

  Therefore 
\begin{align}
    |a| + |b| &= a - b
\end{align}

As $b<0$ and $|a| < |b|$, we know that $a + b < 0$ and thus 
\begin{align}
    |a + b| &= -(a+b) \\
    &= -a-b
\end{align}
The conjecture says that $|a + b| \leq |a| + |b|$, so we must show that
\begin{align}
    -a-b &\leq a - b
\end{align}
Adding $b$ to both sides gives $-a \leq a$ which, as $a \geq 0$, is clearly true.
</div>\EndKnitrBlock{proof}

***

Conjecture \@ref(cnj:hallway): First, we rewrite the conjecture,

<center> If $a$ is a perfect square, then $a$ is either a multiple of $3$ or one more than a multiple of $3$.  </center>

Now we're ready for a proof by cases. 

\BeginKnitrBlock{proof}<div class="proof">\iffalse{} <span class="proof"><em>Proof. </em></span>  \fi{}If $a$ is a perfect square, then there is some integer that when squared gives $a$. As all integers are either a multiple of $3$, one more than a multiple of $3$ or two more than a multiple of $3$, I'll consider these three cases. We'll use a direct proof within each case.

**Case 1:** $a=(3n)^2, n \in \mathbb Z$ <br /> i.e. $a$ is the square of a multiple of $3$, which covers square numbers like 0, 9, 36, 81, 144, ...

We have
\begin{align}
    a &= (3n)^2 \\
    &= 9n^2 \\
    &= 3(3n^2)
\end{align}
which is clearly a multiple of 3.

**Case 2:** $a=(3n + 1)^2, n \in \mathbb Z$ <br /> i.e. $a$ is the square of one more than a multiple of $3$, which covers square numbers like 1, 16, 49, 100, 169, ...

We have
\begin{align}
    a &= (3n+1)^2 \\
    &= 9n^2 + 6n + 1 \\
    &= 3(3n^2 + 2n) + 1
\end{align}
which is clearly one more than a multiple of 3.

**Case 3:** $a=(3n + 2)^2, n \in \mathbb Z$ <br /> i.e. $a$ is the square of two more than a multiple of $3$, which covers the remaining square numbers, like 4, 25, 64, 121, 196, ...

We have
\begin{align}
    a &= (3n+2)^2 \\
    &= 9n^2 + 12n + 4 \\
    &= 9n^2 + 12n + 3 + 1 \\
    &= 3(3n^2 + 4n + 1) + 1 
\end{align}
which is clearly one more than a multiple of 3.

As we've accounted for all square numbers, we're done.
</div>\EndKnitrBlock{proof}

***

<div class="alert alert-danger" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-129"><strong>(\#exr:unnamed-chunk-129) </strong></span>Before moving forward, read Chapter 14, **Without loss of generality**. This is a really useful technique that can save you a lot of time when using proof by cases.
</div>\EndKnitrBlock{exercise}
</div> 

<div class="alert alert-info" role="alert">
\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-130"><strong>(\#exr:unnamed-chunk-130) </strong></span>Some of these conjectures are false; disprove them by finding a counterexample. Some of them are true; prove them using one (or a combination of more than one) of the methods we've met so far.

(\#cnj:highway): $5a+6$ has the same parity as $a$.

(\#cnj:hay): $a^2 + a^3$ is even for all integers $a$.

(\#cnj:hip): If $a$ and $b$ are integers, $a^2b^2$ is even.

(\#cnj:heart): For all numbers $a, b, c$, if $ab = bc$ then $a = c$.

(\#cnj:harvest): For any integer $a$, $(3a-1)$ is a multiple of 2.

(\#cnj:harm): The sum of two consecutive numbers is odd.

(\#cnj:hover): Let $a$ be an integer. Then $a^{2} + a$ is even.

(\#cnj:hang): There are no negative square numbers.

(\#cnj:hole): If $a$ is prime, then $a + 13$ isn't.

(\#cnj:half): There is no two-digit prime number (with different digits) which is still prime when you swap its digits.

(\#cnj:hot): For $a \in \mathbb Z^+$, $a^2 - a + 11$ is prime.

(\#cnj:holt): Zero is even.

(\#cnj:horse): For any pair of integers $a$ and $b$, there is an integer $c$ such that $a^2 + b^2 = c^2$, where $c > a$ and $c > b$.

(\#cnj:heavy): MAX($a, b$) + MIN($a, b) = a + b$ for any $a$ and $b$.

(\#cnj:hardware): If $a>c$ and $b>c$ for any numbers $a,b$ and $c$, then MAX$(a,b) - c$ is always positive.


(\#cnj:honour): Let $a$ be an integer. If 3 does not divide $a$, then 3 does divides $a^2 - 1$.

(\#cnj:harmony): If $a$ and $b$ are both positive integers and $n = ab$, then either $a \leq \sqrt{n}$ or $b\leq \sqrt{n}$.

(\#cnj:hilarity): The only way for $3a^2 + 4a + 3$ to be even is if $a$ is odd.

(\#cnj:headquarters): For integers $a$, $b$, $c$, $d$ and $n$, $(an + b)$ and $(cn + d)$ have different parity to one another only when $a$ and $b$ have different parity to one another AND $c$ and $d$ have different parity to one another.

(\#cnj:history): 127 is prime.

(\#cnj:helicopter): If $a$ is an integer, then $a^2 + 1$ is prime.

(\#cnj:homely): If $a > 0$, then $\sqrt a < a$.
</div>\EndKnitrBlock{exercise}
</div>

<!--chapter:end:13-test.Rmd-->

# Without loss of generality

"Without loss of generality", or simply *w.l.o.g.*, is an incredibly useful technique which will save you a lot of time when using proof by cases. When used correctly, it allows you to merge two cases into one.

Here's a general example: 

*I ask all students that I teach to complete a questionnaire which asks them, among other things, how many siblings they have. After looking at the results, I assemble in one room all those students who indicated that they have just one sibling. I am interested in the age difference between these students and their sibling. I ask them to subtract their sibling's age from their age. If the answer is between 0 and 5 years, they must stand on the left side of the room. If the answer is more than 5, they must stand on the right side of the room. If the answer is between 0 and -5, they must stand at the front of the room. If the answer is below -5, they must stand at the back of the room.*

Notice that because I asked them to subtract their sibling's age from their age, a positive number indicates that they are older than their sibling, and a negative number indicates that their sibling is older than them.

But then I realise, why do I care whether the answer is positive or negative? Aren't I just interested in the difference in the ages? Do I really need to know who was older, the student or their sibling? If not, then I can tell them to simple subtract the lower age from the upper age. This will produce a nonnegative number, which, if I'm only interested in the difference in ages, is enough information for me. I have condensed four cases into two, losing no crucial information.

<div class="alert alert-warning" role="alert">
<strong>W.l.o.g. is used whenever no crucial information is lost by cutting out cases.
</strong> 
</div>

Let consider another example. Imagine a conjecture in which $P$ says that $a,b \in \mathbb R$. Depending on the conjecture, we could use four cases to partition here:

**Case 1:** $a,b \geq 0$ <br />
**Case 2:** $a,b < 0$ <br />
**Case 3:** $a\geq 0$, $b < 0$ <br />
**Case 4:** $a <0$, $b \geq 0$ <br />

Whilst there is something fundamentally different about **Cases 1, 2** and **3** (because positive and negative numbers usually behave quite differently to each other), **Case 4** is essentially the same as **Case 3**. Unless the order of $a$ and $b$ is important, we can use **Case 3** whenever we have a nonnegative number and a negative number, which covers everything **Case 4** covers. **Case 4** is therefore redundant and without loss of generality can be merged with **Case 3**. Then, for example, we had $a=-5$ and $b = 2$ (**Case 4**), we can just swap the letters (so $a=2$ and $b = -5$) and this is covered in **Case 3**. In the proof, we would write "One of $a,b$ nonnegative, the other negative. W.l.o.g., let $a\geq 0$, $b < 0$".

Let's look at a couple of conjectures. First, a conjecture where w.l.o.g. can be used, and then a conjecture where it can't.

## When w.l.o.g. does work

(\#cnj:hall): The product of an odd integer and an even integer is even.

We are considering the product of two integers, $a \cdot b$. One of these integers is even, and the other is odd.
  
W.l.o.g., let's say that $a$ is the even one and $b$ is the odd one, so

\begin{align}
  a &= 2m \\
  b &= 2n + 1
\end{align}

with $m, n \in \mathbb Z$.^[Notice I have used two different integers here, $m$ and $n$, as the conjecture doesn't say $a$ and $b$ must be consecutive (though of course they can be).] We could now continue with our proof, having halved the amount of work we need to do!

**Do you see why w.l.o.g. worked here?** If I wanted to demonstrate this conjecture to someone by asking them to pick two numbers, one even and one odd, I just assign the even one to $a$ and the odd one to $b$. If we had made $a$ the odd one and $b$ the even one, the proof would look identical, so our choice of which was odd and which was even was unimportant. That's what w.l.o.g. means!

Here's the complete proof:

\BeginKnitrBlock{proof}<div class="proof">\iffalse{} <span class="proof"><em>Proof. </em></span>  \fi{}W.l.o.g., let's say that $a$ is the even one and $b$ is the odd one, so

\begin{align}
  a &= 2m \\
  b &= 2n + 1
\end{align}

with $m, n \in \mathbb Z$. 
  
We have

\begin{align}
  a \cdot b &= (2m)\cdot (2n+1) \\
  &= 4mn + 2m\\
  &= 2(2mn+m)
\end{align}

which is clearly even.
</div>\EndKnitrBlock{proof}

## When w.l.o.g. doesn't work

Sometimes w.l.o.g. doesn't work.  That's because changing the letters *does* fundamentally change the case we're considering. Let's look at an example...

(\#cnj:hope): The product of two consecutive numbers is even.^[Note, we could simply use the fact that conjecture \@ref(cnj:hall) is true and our knowledge of the alternating nature of the parity of integers to declare this conjecture true, but I prove it in full here as a useful illustration.]

We are considering the product of two integers, $a \cdot b$. If two integers $a$ and $b$ are consecutive, then $b = a + 1$. If we multiply them, we get
  
\begin{align}
    a \cdot b &= (a)(a+1) \\
    &= a^2 + a
\end{align}
    
but it isn't obvious that this is even, so we'll need a new strategy.

As $a$ and $b$ are consecutive integers, one is even, and the other is odd, because parity alternates for integers.

Let's make $a$ the even one and $b$ the odd one, so,
  
\begin{align}
    a &= 2m \\
    b &= 2m + 1  
\end{align} 

Their product is  

\begin{align}
    (2m)\cdot (2m+1) &= 4m^2 + 2m\\
    &= 2(2m^2+m)  
\end{align} 
which is clearly even.

But notice, this proof only covers pairs of consecutive integers where the smaller number is even, for example $(2, 3)$, $(4, 5)$, ($-2$, $-1$). It does *not* cover pairs of consecutive integers where the smaller number is odd, for example $(1, 2)$, $(-1, 0)$, ($7$, $8$). If you ask a friend to pick two consecutive numbers and they pick 7 and 8, we **must** assign 7 to $a$ as it's the smaller of the two numbers, but we *can't* assign 7 to $a$ because we said "let's make $a$ the even one".

We should label the case above as **Case 1**, then provide a second case, where $a$ is odd and $b$ is even:

**Case 2:** 

\begin{align}
    a &= 2m + 1 \\
    b &= (2m + 1) + 1 \\
    &= 2m + 2
\end{align}

The product is

\begin{align}
    (2m + 1)\cdot (2m+2) &= 4m^2 + 4m + 2\\
    &= 2(2m^2+2m + 1)
\end{align}

which is clearly even.

We've shown that this conjecture is true if the smaller of the two consecutive numbers is even, and if the smaller of the two consecutive numbers is odd. These two cases cover all possible pairs of consecutive numbers, and in both cases, we found the statement to be true, so the conjecture is true. We are done!

Here's what the proof looks like in full:

\BeginKnitrBlock{proof}<div class="proof">\iffalse{} <span class="proof"><em>Proof. </em></span>  \fi{}We call our two consecutive numbers $a$ and $b$. W.l.o.g., let $a$ be the smaller of the two.

**Case 1:** $a$ even, $b$ odd.

\begin{align}
    a &= 2m \\
    b &= 2m + 1
\end{align}

Thus,

\begin{align}
  a \cdot b &= (2m)\cdot (2m+1) \\
  &= 4m^2 + 2m\\
  &= 2(2m^2+m)
\end{align}

which is clearly even.

**Case 2:** $a$ odd, $b$ even.

\begin{align}
    a &= 2m + 1 \\
    b &= (2m + 1) + 1 \\
    &= 2m + 2
\end{align}
    
Thus,

\begin{align}
    a \cdot b &= (2m + 1)\cdot (2m+2) \\
    &= 4m^2 + 4m + 2\\
    &= 2(2m^2+2m + 1) 
\end{align}

which is clearly even.
</div>\EndKnitrBlock{proof}


<!--chapter:end:14-test.Rmd-->
