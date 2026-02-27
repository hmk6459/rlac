---
title: "Post: Assignment 1"
categories:
  - Blog
tags:
  - link
  - Post Formats
link: https://github.com
---

Welcome to assignment 1

---
title: "Assignment 1"
excerpt_seperator: ""
categories:
    - Assignments
---

## Introduction

Growing up, we defined the Harry Potter universe by its 'magical infrastructure', including the physical tools and the iconic villains that drive the plot. When we started this project, we expected words like 'Voldemort' and 'Wand' to be the statistical anchors of every story. It’s almost common sense: Harry Potter is about wizards. However, our research challenged this baseline assumption. Looking at the data, we found a significant gap where some fanfictions barely mention a 'wand' at all. This discovery forces a shift in our perspective. If these core magical elements are missing, what are these stories actually about? Can we even categorize them as 'Harry Potter' novels anymore, or have they become something else entirely?"


<!--	Exported from Voyant Tools (voyant-tools.org).
The iframe src attribute below uses a relative protocol to better function with both
http and https sites, but if you're embedding this into a local web page (file protocol)
you should add an explicit protocol (https if you're using voyant-tools.org, otherwise
it depends on this server.
Feel free to change the height and width values or other styling below: -->
<iframe style='width: 509px; height: 363px;' src='https://voyant-tools.org/tool/Trends/?query=voldemort&query=wand&corpus=2285a99186968a5c7cfd5e8001fcc496'></iframe>
Figure 1. Relative Frequency Chart between ‘Wand’ and ‘Voldemort across the analyzed texts

## Analysis

Looking through the Voyant tools website, we found something interesting: in the majority of the materials we checked, the number of times wands and Voldemort are mentioned is nearly identical. We found this interesting, as from our knowledge of the movies and some books, wands and the prince of darkness don’t really have any correlations, so it got us wondering, why would this be the case? But at the same time, this graph made us think about another interesting observation. It is common knowledge that Harry Potter books are books about wizards, the most famous line is literally “you are a wizard, Harry”, so when we notice that there are some fanfiction articles that barely contain the word wand we become curious to understand these texts better. 

![as](/rlac/assets/images/fig2.jpg)
Figure 2. Relative Frequency Chart between ‘spell’, ‘flying’, and ‘invisible.’ 

Although some of the terms, we’ll admit, were in a way expected not to appear as frequently because they are closely tied to objects such as the invisible cloak, we were quite surprised by this analysis, where we can clearly see that even the word spell is barely mentioned in some of the books/articles. This, in some way, shows the drawbacks of using Voyant tools and other forms of distant reading, as mentioned in “Distant Reading: A Conversation with Ama Bemma Adwetewa-Badu.” The context is still something that is missing, and if we truly wanted to understand these trends and why they are so low/high, we would still need to read the book. The best example for this we can clearly see from the Lyingleia’s fanfiction, which, by the data present, makes it difficult to understand why it would be considered a part of a big wizard fiction franchise when it clearly doesn't use most of the terms we associate with magic or wizards in general. 


![Heatmap](/rlac/assets/images/figure3.png)
Figure 3: Heatmap of words such as ‘wand’, ‘magic’, hogwarts, ‘potion, and ‘spell’. 

To get a more precise view, we generated a Heatmap in Posit-Cloud. The results were the following: the NYU version contains zero mentions of "wand" or "spell," and only two instances of "magic." Similarly, Yellowsunchild shows a negligible frequency of these terms. Now that we have the numbers, our next step was to dig deeper into these two stories, to best understand what's actually holding the plot together, if it isn't magic.

![Word Cloud](/rlac/assets/images/figure4.png)
Figure 4. Word Cloud of Yellowsunchild and Lyingleia’s fanfictions

From an outer lens, we see, of course yellowsunchild’s book having a clear disparity in word frequency between the two corpora. However, both books seem to follow the life of a teenager. In both stories, the characters go through what feels like a university experience. There are mentions of books, notes, dorms, conversations, and even romantic moments, which reflect aspects of student life that many readers may recognize. From these details, the setting can become more relatable to students and highlight the stage of life when people are still figuring themselves out. We wished to understand better when exactly these words appear and within what contexts. 

![Collacoate of Darco in Yellowsunchild](/rlac/assets/images/figure5.png)
Figure 5. Collocate of Darco in Yellowsunchild’s fanfiction

We used the Collocates tool to look at the words associated with Draco. Given his prominence in the word cloud, he is clearly a central figure in the fanfiction. We see that he is highly linked to social verbs and nouns like "kiss," "lips," and "text." This signals a social lens that moves characters like Harry and Draco out of the "Hero" role and into the "Student" role.

![Word Cloud](/rlac/assets/images/figure6.png)
Figure 6. Word Cloud of the Two Rowling books and Witchdragon

In contrast, when studying the two Rowling books and the fanfiction by Witchdragon, they use noticeably different vocabulary as opposed to the Yellowsunchild and Lyingleia’s fanfictions. We see terms like “death”, “ wizard, “wand,” “sword,” and “magic” appear, which introduce a darker, more fantastical tone that sharply differs from the university-centered language of the earlier texts.
These discoveries pushed us to dig deeper into how magical language is used across the series versus fanfiction. We wanted to get a better grasp of how much the canon storyline relies on these words compared to the fan-authored versions. To do this, we used Posit Cloud to measure the density of a "magical vocabulary" list. This allowed us to see not just if the words were there, but how consistent they were throughout each text.


![Figure Bar](/rlac/assets/images/figure7.png)
Figure 7. (Bar Chart) of the Magical Vocabulary per 10,000 words

As shown on the graph, we can see that magic words are much more present in the original books as opposed to in fanfiction. 

## Conclusion

Together, our research shows a major shift in how fanfiction uses language compared to the original books. Rowling’s vocabulary is often built around magical conflict, power, and war. In contrast, these fanfiction stories are built on words about relationships, emotional intimacy, and student life. This change shows that for these authors, the human connections are the most important part of the narrative.

We found a post by Karl-Erlend Mikalsen, a senior academic adviser at the University of Tromsøthat explains, that explains and complements our research by asking: what would Harry Potter actually be about without the magic? She argues that if you strip the wizardry away, the core story is really about "an abused and neglected adopted child... fantasising about birthdays and friends... and caring adults." This idea is a fairly accurate lens for looking at our findings in Yellowsunchild and Lyingleia’s fanfiction. The high frequency of words like "notes," "dorms," and "romantic moments" suggests that these fanfictions might be focusing more on the human foundations, as Mikalsen describes.

However, there are vital aspects to consider within our previously made conclusions based from the two tools. As Ted Underwood argues in ‘The Risks of Distant Reading,’ and from our previous class discussions, a computational model doesn’t ‘read’ context; it simply identifies patterns from a list of terms and makes its own conclusions based on that. Our analysis of Figure 2 confirms this risk: the data shows the word 'spell' disappears in Lyingleia’s text, but that doesn't mean the entire wizarding world is gone. On the positive hand, as Underwood suggests, the model has helped us identify a massive shift between the two groups of texts we analyzed, which a human reader might miss, from a narrative of magical war to a narrative of domestic student life.

Similarly, Erez Lieberman Aiden, a computational geneticist at Baylor, argues that a healthy academic field requires a balance between those who are 'overly enthusiastic' in using data and those who 'slam the brakes on it.' In the context of our study, this means that while Voyant and Posit Cloud cannot replace the nuance of a human reader, they remain essential tools for identifying the broad cultural shifts that allow us to see the Harry Potter universe from a new perspective.

In Rowling's books, particularly in Chamber of Secrets and Deathly Hallows, magical terminology is very present. For example, the words “wand,” “magic,” “death,” “Voldemort,” and “sword” are consistently and densely present. These words point to a narrative structure that is centered on conflict, danger, and the maintenance or destruction of power. The wizarding world is prominently presented as a world that is defined by magical systems, power structures, and war. Even in instances where the characters are having emotional experiences, these experiences are embedded in a larger context of magical struggle. The language itself is structured in this way, with objects of power, spells, and enemies being lexically central.

By contrast, the fanfiction we examined presents a noticeably different language use. Magical vocabulary appears at a significantly lower rate or disappears entirely. Yet the absence of frequent magical words does not mean the absence of narrative substance. Instead, the vocabulary shifts more towards everyday actions and emotions. Words such as “walked”, “text”, “spoke”, and “hand” become more prominent, which implies more focus on human emotions and connections rather than magical conflict and politics. 

This does not mean that the wizarding world of fanfiction has been discarded. Rather, it assumes it. The magical world has been treated as a given knowledge shared by the reader and the writer. Since the reader is already familiar with what Hogwarts, wands, and spells represent, the writer of fanfiction has the liberty to concentrate on other areas of the story. Thus, it has not been discarded; rather, it has been shifted to other areas of fantasy, like character and relational development.

Through distant reading tools such as Voyant tools and Posit Cloud, we can easily observe how lexical patterns reflect deeper narrative transformations. So, to answer our earlier question, if Harry Potter is not a book about wizardry, perhaps it is about human relations and emotions in the wizarding world. 