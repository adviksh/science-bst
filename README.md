# science-bst
This repo contains a BibTeX bibliography style file for submissions to Science magazine. It's based on the [this style file](https://www.sciencemag.org/sites/default/files/Science.bst) offered by Science, with one bugfix and one added feature:

* Items tagged as @article now print their titles, followed by a period.
* There's a new @footnote class designed to print footnotes<sup>1</sup> as part of your References and Notes section.

## Footnotes
1. Create an @footnote entry like the ones below
2. Enter the entire text of the footnote in the "title" field, enclosed in curly brackets {}.
3. The last sentence in your footnote should have no period / full stop at the end. BibTeX will automatically print one, so if you conclude the footnote with a period / full stop, the entry will have two of them in the bibliography.
4. As configured, BibTeX will capitalize the first letter of the first sentence and then defaults to forcing everying else into lower case. To capitalize other letters, including the first words of later sentences and proper nouns, enclose those letters in curly brackets.

Example:

@footnote{footnote-explanation,

  title=  {Put your footnote text here. {U}se curly braces to make sure the first words in later sentences, and any {P}roper {N}ouns get capitalized. If you don't enclose a capital letter in braces, it will get converted to lower case, like the first word of this sentence. {L}ast, make sure not to end your closing sentence with a full stop or period}

}

You can then use \cite{footnote-explanation} in the main text.

<sup>1</sup> Like this.
