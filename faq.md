# Frequently Asked Questions: Conscious Language Program

## What is a "conscious language" effort?

The phrase "conscious language" refers to selecting words and phrases consciously, intentionally, considering connotations as well as denotations. The software industry sometimes uses certain words, like blacklist, and slave, that may carry a great deal of emotional and historical baggage. We are encouraging projects to choose phrases that clearly communicate the technical meaning, without using metaphors or colloquialisms.

This has the dual purpose of removing problematic terms, and also communicating more clearly, particularly to those who are working in a secondary language.

Our goals are to identify where problematic terms are used, collaborate on replacement terminology, support project contributors in making updates, and report on joint progress.

## Why is this important?

If open source is truly meant to be inclusive and a place where anyone can participate, it must be welcoming to all. If words or phrases convey secondary unintended meanings to our audience (or are simply confusing!) we are potentially limiting participation in our projects, which is antithetical to this goal.

## What terms are we recommending you consider?

We have identified the terms "master/slave" and "whitelist/blacklist" to work on because these are considered most visible and problematic across the industry.

Over time, we may recommend consideration of other terms, such as words that reference mental health, gender, physical handicaps, and several other categories. We may also give tips on avoiding colloquialisms that simply don't translate well or prove a barrier to understanding.

## What are the recommended replacement terms?

To proceed, teams should follow the [recommendations outlined by the Linux kernel](https://lkml.org/lkml/2020/7/4/229). These recommendations have informed the terminology recommendations we provide below. 

To ensure consistency and success, it is imperative for product team stakeholders to align internally. For example, documentation teams should engage in discussions with their engineering leadership to reach an agreement on replacement terms. This will ensure that the product documentation will match the code.

When master refers to the main branch, our recommendation is to replace it with main.

Our recommendations for master/slave terminology are:

 * primary / secondary
 * source / replica
 * initiator, requester / responder
 * controller, host / device, worker, proxy
 * director / performer

Our recommendations for blacklist/whitelist terminology are:

 * denylist / allowlist
 * blocklist / passlist

If your project opts to use some other term or phrase, please [let us know](https://github.com/conscious-lang/conscious-lang-docs/issues) that you’ve done so, and why, so that we can learn from your decisions.

### Why does 'master' matter outside of the context of master/slave?

While 'master/slave' is a clear example, 'master' is a word that has context-specific meanings that have different connotations. We recommend you consider, is 'master' the most accurate word you can use? Is this the word you would consciously choose in this case?

A further question to consider in the use of the word 'master' is: Is it a thing that is controlling things without giving those things free will?

## Oh no! Slippery slope! Newspeak!

We've heard concerns that this initiative
puts us on a slippery slope to Newspeak portrayed in the 1984 dystopia
by George Orwell. This initiative is completely different from Newspeak.
Newspeak involved multiple changes but the most essential were:

 * Removing precise words in favor of general words so that it would become difficult to form precise thoughts
 * Using the opposite word for the true situation to disguise what's really happening

Everything in the conscious language initiative is *the exact opposite* of that.

For example, "Denylist" is both more precise and more accurate than "blacklist";

"Primary" is both more precise and more accurate than "master" in projects that have made that switch.

The goal of this project is to use more precise words, in order to avoid
unintended connotations that some common words and phrases have. Not
only does this eliminate the hurt caused by those connotations, it also
improves understanding, particularly for people who are reading in a
second language, where those idioms may be confusing.

## How can I educate myself on why these terms are problematic?

Here are some resources on the topic:
 * [ Terminology, Power, and Inclusive Language in Internet-Drafts and RFCs](https://tools.ietf.org/html/draft-knodel-terminology) - IETF draft argues for more inclusive language conventions by RFC authors
 * [Welcoming Nomenclature](https://www.youtube.com/watch?v=hZuFeFuazwo) - Community Central presentation by Rich Bowen (Red Hat)
 * [Is It Enough To Remove Words With Racist Connotations From Tech Language? Hint: No](https://www.npr.org/2020/07/09/889502179/is-it-enough-to-remove-words-with-racist-connotations-from-tech-language-hint-no) - NPR interview with web developer Caroline Karanja
 * [Why is everything white?](https://www.bbc.com/news/av/world-us-canada-52988605/muhammad-ali-why-is-everything-white) (1971) - interview with Muhammed Ali
 * [That Word Black (2014)](http://mcwriting11.blogspot.com/2014/06/that-word-black-by-langston-hughes.html) - blog post by Langston Hughes
 * [Broken Metaphor: The Master-Slave Analogy in Technical Literature (2007)](https://www.jstor.org/stable/40061475?seq=1) - article in JSTOR, requires free membership to read
 * [Terminology, Power and Oppressive Language](https://tools.ietf.org/id/draft-knodel-terminology-00.html) - article with recommendations by Mallory Knodel and Niels ten Oever
 * [Why "master" matters](https://twitter.com/mislav/status/1270388510684598272) - A twitter thread.

## How can I get a list of projects that need help in this effort?

[Answer needed]
