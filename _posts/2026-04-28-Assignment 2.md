---
title: "Assignment 2"
excerpt_seperator: ""
categories:
    - Assignments
---

## Introduciton

The use of computational methods in literary analysis provides researchers with alternative tools for working with texts. Stylometric analysis and TF-IDF (term frequency-inverse document frequency) analysis provide researchers with tools to uncover patterns of text concerning authorship, style, and thematic similarity within a corpus. But since each computational tool produces different results, researchers need to determine what constitutes a meaningful textual similarity.

In this essay, we compare the output produced by the Stylo tool in R programming language and the output provided by TF-IDF and its application for principal component analysis. We apply both computational tools to a small set of science fiction stories written by authors including Philip K. Dick, Leigh Brackett, Andre Norton, and H. G. Wells. This essay demonstrates that the contrasting clustering patterns produced by these methods reveal fundamentally different ways of interpreting the corpus.

## Gender Differentiation Between the Texts

One particularly revealing difference between the two methods comes up when examining “Jackie Sees a Star” by Marion Zimmer Bradley. This short story  was particularly interesting to us, because it would always show up separated from the other texts when examining into the TF-IDF visualization and would also always be differentiated when classified with stylo. When looking deeper into this we noticed something interesting. 

![TF-IDF300Analysis](/rlac/assets/images/tf-idf300.png)
Figure 1. TF-IDF Visualization

In the TF-IDF visualization the text always appears in close proximity to “The Bluemoth” by Leigh Bracket which suggests that there is a thematic similarity between the two, such as similar vocabulary and narrative focus. And this is consistent with different MFW’s analyzed, no matter if it's 200 or 500, the result is always similar (will show both examples here). However, in the Stylo clustering, “Jackie Sees a Star” consistently appears as an outlier, separated not only from Brackett’s work but also from Bradley’s other texts. The difference emphasizes the key distinction between the two algorithms, where TF-IDF categorizes documents according to their content, whereas Stylo extracts styles, indicating that “Jackie Sees a Star” could be written in a significantly different narrative voice or syntax.

![Stylo200Words](/rlac/assets/images/stylo200.png)
Figure 2. Stylo Vizualization of 200 most frequent words

This finding also complicates any attempt to correlate gender with the algorithmic patterns. Although both the authors, Bradley and Brackett are females, their works do not form a stable cluster in either method. Instead, the result suggests that stylistic variations within a single author might be as significant as differences in between authors. 

This, thus suggests that gender might not play a major role as a difference between authors, reinforcing Underwood’s argument that distant reading methods often fail to capture the full complexity of literary identity. 

But we did notice something else that also caught our attention. If you look to the bottom of the TF-IDF visualization displayed above, there is something interesting to notice there. There is a distinct line between texts made by male and by female authors. To dig deeper into this, let's turn on the Loadings and see what are some of the words that make this difference. 

![TF-IDF300Analysis](/rlac/assets/images/tf-idf500loading.png)
Figure 3. TF-IDF Visualization with loadings

The graph seems to suggest that there is a clear difference between male and female gender authors, but if we instead use the stylo classification, like the one we used above it is clear that this is not the case. This suggests that the underlying stylistic features of the texts, such as syntax and grammatical patterns are not strongly differentiated by author gender.

We decided to further investigate this apparent gender based clustering, so we conducted a comparative analysis using Voyant Tools, separating the corpus into male and female authored texts. 

![MaleWordsCloud](/rlac/assets/images/MaletextsWordCloud.png)
Figure 4. Word Cloud of most frequent words in Male author texts

![FemaleWordsCloud](/rlac/assets/images/FemaletextsWordCloud.png)
Figure 5. Word Cloud of most frequent words in Female author texts

The word clouds reveal that much of the difference between the authors and their texts result from the repeated names of characters and the structural elements rather than any fundamental difference in style. For example, as we can see the name “Hendricks” is an important part in the works of Philip K. Dick and Henry Kuttner, both male authors, while names “Dane” and “Stark” are common names in works written by Leigh Brackett and Andre Norton, who are female writers. Moreover, words such as “said” are commonly used by male writers in these examples, suggesting a more dialogue driven narrative. While female writers use words such as “eyes” and “come” pointing to a more descriptive style of writing. 


These findings suggest that the difference that the TF-IDF clustering was “picking up” was less about gender of the authors, and more about the difference in narrative focus, such as character-centered storytelling and recurring lexical patterns. Since TF-IDF amplifies distinctive vocabulary, it is particularly sensitive to proper nouns and repeated narrative elements, which can create the appearance of broader categorical divisions within the corpus.

This distinction leads to some interesting considerations regarding the interpretation of computational results. The fact that gender is present in content-based processing, while absent in stylistic analysis, implies that the term “gendered writing” could actually be less related to language construction than story-telling and other narrative choices. In other words, computational analysis not only uncovers patterns but also constructs them.

## Comparative Analysis of Two “Outliers”, Jackie Sees a Star and The Salvaging of Civilization

Upon analyzing the TF-IDF visualization, two significant outliers emerged: Marion Zimmer Bradley’s Jackie Sees a Star and H.G. Wells’ The Salvaging of Civilization. These texts are positioned on opposite ends of the graph, far from the (0,0) origin, indicating a high degree of thematic and lexical divergence from the rest of the corpus. To investigate this gap, we employed Voyant Tools for distant reading and supplemented our findings with biographical research on the authors.

### Quantitative Data Comparison

The most immediate difference is found in the scale of the works:

* Longest Document: The Salvaging of Civilization (51,390 words).

* Shortest Document: Jackie Sees a Star (1,896 words).

### Distinctive Vocabulary and Content

The frequency of distinctive words highlights a complete lack of thematic overlap between the two texts:

* The Salvaging of Civilization: Dominant terms include "great" (150), "state" (118), "bible" (116), "people" (115), and "life" (107).

* Jackie Sees a Star: Key terms center on characters and setting, such as "Jackie" (25), "mig" (21), "spaceship" (10), "kid" (10), and "dave" (9).

![Bubblines](/rlac/assets/images/bubblines.png)
Figure 6. Bubblines 

As a starting point, we analyzed the Bubblines to get a sense of the frequency and distribution of terms in the two corpora. Based on the visualizations, we see almost no direct similarities in terms of term usage, with just a single usage of the term “word” by Bradley.

![WellsWordCloud](/rlac/assets/images/wellsWordCloud.png)
Figure 7. Word Cloud of most frequent words in Wells' work

The Word Cloud (Cirrus) for Wells’ work reveals a philosophical and historical lens, with prominent mentions of "war," "history," and "education". This suggests a scholarly text intended for an adult or academic audience, which is an observation supported by the fact that Wells was a four-time Nobel Prize nominee.

![JackieSeesaStarWordCloud](/rlac/assets/images/JackieSeesaStarWordCloud.png)
Figure 8. Word Cloud of most frequent words in "Jackie Sees a Star" 

In contrast, the Cirrus for Jackie Sees a Star emphasizes domestic and juvenile themes, with words like "family," "father," "mother," and "kid". This suggests a narrative focused on a family’s experience, likely within the science fiction or fantasy genres, as the word spaceship is also present in the visualization.

By combining TF-IDF visualizations with close reading as well as some surface reading with Voyant tools, we can confirm that the thematic distance between these texts is driven by a split genre. While Wells seems to focus more on broad societal structures, Zimmer Bradley prioritizes a character-driven narrative. In fact, this can be supported by analyzing the bibliography of the two authors. Firstly, through the Internet Speculative Fiction Database. Analyzing Bradley first, whose two most popular author tags are science fiction (25) and fantasy (14). (ISFD)

An interesting finding shows that Marion Zimmer Bradley has cited Kuttner as an influence throughout her work (Wikipedia). So linking this to fig 2, we see that the bradleys 2 other texts seem to be similar to Kuttner’s works, whilst Jackie is a Star seems to be an outlier, and the other two have similarities in terms of writing styles.

Now analyzing H.G wells, he was an English writer, prolific in many genres. (Wikipedia). The term “Many” here suggests that he may have different writing styles that he uses for certain texts he writes. Analyzing this further using the Internet Speculative Fiction Database, we see which author tags he is associated with, including, but not limited to, war, fantasy, evolution, travel, and satire. By taking a surface reading approach of the salvaging of civilizations, against the other two texts, we can argue the reason as to which he the text seems to be situated away from the others is that he spreads optimism that has belief in humanity to rebuild society through ideas and thinking, two words also seen on the wordcloud, which he tends to not do through his other works and particularly The Island of Doctor Moreau and The War of the Worlds, which tends to expose humanities mistakes and failures. These points support our earlier claim that an author can change their style of writing at any point in time, and the visualizations we see are a result of that.

An important consideration is that our examination of Jackie Sees a Star highlights the risks of relying purely on distant reading, serving as an additional example to support the previous reference to Underwood’s arguments. Without conducting a close reading or surface reading, one might inaccurately assume the story is told from Jackie’s perspective. In reality, the narrative is delivered through Aunt Dorothy, whose observations are vital in the story's events.  Furthermore, a purely distant approach might overlook the crucial detail that Jackie is a young boy with telepathic abilities, a fact revealed through subtle textual cues in his "inside the head" conversations. All of which suggests that close reading may be required to get the most out of a story.

## Comparative Analysis of Remainder Texts

Having established why these outliers appear at the edges of our data, we now turn to the texts clustered near the center of the TF-IDF visualization to identify the shared linguistic features that draw them toward a common core. Specifically, in Figure 3 we observe that Black Amazon of Mars (Leigh Brackett), Enchantress of Venus (Leigh Brackett), The Black Kiss (Henry Kuttner), The Defenders (Philip K. Dick), and Falcons of Narabedla (Leigh Brackett) cluster closely together.

Our initial assumption, based on how TF-IDF operates, is that these texts rely on “most frequent words” similarly to those of other texts in the corpus. In other words, they do not exhibit a particularly “loud” or distinctive vocabulary compared to Jackie Sees a Star for instance. This appears to be the case, as we see commonly occurring terms such as “from,” “back,” and “be” dominate, indicating a relatively neutral and non-distinct language profile.

However, there are a few considerations to note when using a low number of Most Frequent Words (like 200 MFW), which creates disparities and confusion because a large part of these words are primarily function words. While these words might reveal an author's stylistic tone, they can also be influenced by the content matter, making it hard to distinguish between an author’s unique language and the norms of the genre. For small texts or specific genres like science fiction, style and content often go together, and it becomes difficult to determine if they are grouped because they are written with the same rhythm or simply because they are using the same specialized vocabulary.

## Does changing MFW affect output?

![Stylo500Words](/rlac/assets/images/stylo500.png)
Figure 9. Stylo Vizualization of 500 most frequent words

We extended our analysis by examining whether changing the number of Most Frequent Words (MFW) from the original setting in Figure 2 would affect the cluster structure. Increasing the threshold to 500 MFW did produce a noticeable difference: the distance between the two analyzed texts became even larger. This is not an outcome we initially expected, as it challenges the assumption that expanding the wordlist would lead texts to cluster more closely with other works by the same author.

That said, the overall changes are relatively modest. While some texts shift positions, the general structure of the clusters remains largely stable. One notable exception is Henry Kuttner’s texts, which move slightly closer together under the 500 MFW condition. Although these changes are not large, they are still analytically meaningful and necessitate closer examination.

This observation motivates the next step of our analysis, to investigate why Kuttner’s The Ego Machine becomes more closely aligned with his other works. To do so, we turn to the expanded wordlist to identify which additions contribute to this shift. For consistency with our visualizations, however, we focus only on the top 500 terms rather than the expanded 5000 terms.

![MostFrequentWords](/rlac/assets/images/mostFrequentWords.png)
Figure 10. Most Frequent Words

We examined three terms, “st,” “robot,” and “cyr”, which appear in the wordlist at positions 324, 438, and 457, respectively. Using Voyant Tools, we found that these terms rank among the most frequent in the text and help explain the increased similarity observed under the 500 MFW condition. They illustrate how expanding the MFW threshold can reveal patterns that were not visible when using only 200 MFW, which allowed us to look more closely into additional content-bearing terms that contribute to closer clustering between texts.

## Conclusion

This study shows that using computational tools like Stylo and TF-IDF can help change our interpretation of the text. Our analysis of the science fiction corpus highlights a major split between content and style. While TF-IDF seemed to suggest a clear "gendered" divide between male and female authors, digging deeper with Voyant Tools showed that this was actually caused by specific narrative choices rather than a fundamental difference in how men and women write. The case of outliers like Jackie Sees a Star and The Salvaging of Civilization also serves as a reminder that distant reading has its risks. Without checking the actual text through close reading, a researcher might miss the fact that a story's thematic distance comes from its unique genre or narrative perspective.  Ultimately, the most useful results come from using these tools alongside close or surface reading to get a full picture of an author’s style and intent.

## References

Distant reading. New Books Network. From https://newbooksnetwork.com/distant-reading

https://www.gutenberg.org/ebooks/author/8842

https://www.isfdb.org/cgi-bin/authortags.cgi?65

https://en.wikipedia.org/wiki/H._G._Wells

https://en.wikipedia.org/wiki/Henry_Kuttner 


READY FOR GRADING!