# Paved With Adverbs

>I believe the road to hell is paved with adverbs, and I will shout it from the rooftops. To put it another way, they're like dandelions. If you have one on your lawn, it looks pretty and unique. If you fail to root it out, however, you find five the next day... fifty the day after that... and then, my brothers and sisters, your lawn is totally, completely, and profligately covered with dandelions. By then you see them for the weeds they really are, but by then it's—GASP!!—too late.

*Stephen King, On Writing*

## What is this?

It's currently an exception custom dictionary, for use in LibreOffice.

My end goal is to highlight adverb use in a LibreOffice document, in real-time, whilst typing. Adding an *exception* dictionary results in a custom set of words being underlined, as a spelling mistake. It's not ideal, but it's a stepping stone while I think of a better approach.

To build the word list I found half a dozen lists of common adverbs, merged them, and removed duplicates. It's subjective, but I don't accept that a word like "not" is among the more evil adverbs, and so I removed it. And, I'm in two minds regarding potential-adverbs, such as "always", or "never". None of the lists I found online, so far, included the word "completely"; or "profligately" for that matter. 

> 8th March 2021: Apart from some existing lists' inadequacies, I've found there are some novel interpretations of the CSV format when it comes to dictionary files! This project may be a work in progress but, if nothing else, I've attached a sensibly formated version of the OPTED v0.03 dictiorary as a single Libre Office "Calc" ODS file. It contains 176,049 words in three columns; word, category, definition.

But, should I *even* include "even"... when it can function as a noun, or an adjective, or an adverb, or a verb?

## Working Source Dictionary v1 (28th Feb 2021)

I don't know if I can make this work, or not, but it's becoming clear the adverb lists I've found so far are a bit rubbish! It needs a different approach and I'm now working with the OPTED v0.03. My first attempt to manipulate its CSV files led to some inconsistencies and, because this is a one-off task, I merged them into a single Libre Office Calc speadsheet and filtered the resulting list.

> Link to OPTED v0.03, the Online Plain Text English Dictionary: http://www.mso.anu.edu.au/%7Eralph/OPTED/

The usage conditions of this dictionary are that its content must remain in the public domain and in plain format. I've attached the entire working dictionary file - hope it might be useful to someone!

I now have a list of **3791** adverbs, of which **2757** end in -LY.

## Working Source Dictionary v2 (7th Mar 2021)

The file `OPTED_Adverbs_07mar2021.ods` uses the same OPTED v0.03 source files, but I wrote a better parsing macro to turn them into actual CSV files, as opposed to a series of 26 plain text files that had been given the file-extension "csv". ;-)

> 8th March 2021: The current list contains **3451** adverbs, which may appear a step backward, but it's more refined, eliminating several words that might see only very occasional use as an adverb.

## What's next?

- [ ] In Libre Office, I would prefer adverbs to be highlighted using a different colour, to distinguish them from actual spelling errors. There does not appear to be any way to do that with a custom dictionary, perhaps a macro is required, but either way, that's a work in progress.

> A blog post discussing macros to highlight "confusables" - https://www.louiseharnbyproofreader.com/blog/using-proofreading-macros-highlighting-confusables-with-comparewordlist

- [X] Build and refine a more comprehensive custom dictionary.
