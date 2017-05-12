---
description: Style guide for Adobe I/O documentation describing standards and conventions for contributors
keywords: style, guide, adobe, documentation
title: Documentation style and grammar conventions
---

## Style Standards

Over time, different publishing communities have written standards for the style
and grammar they prefer in their publications. These standards are called
[style guides](http://en.wikipedia.org/wiki/Style_guide). Generally, Adobe's developer
documentation uses the standards described in the
[Associated Press's (AP) style guide](http://en.wikipedia.org/wiki/AP_Stylebook).
If a question about syntactical, grammatical, or lexical practice comes up,
refer to the AP guide first. If you don’t have a copy of (or online subscription
to) the AP guide, you can almost always find an answer to a specific question by
searching the web. If you can’t find an answer, please ask
[Colene](https://twitter.com/colene) and
we will find the answer.

That said, please don't get too hung up on using correct style. We'd rather have
you submit good information that doesn't conform to the guide than no
information at all. Adobe I/O's tech writers and authors are always happy to help you with the
prose, and we promise not to judge or use a red pen!

> **Note**:
> The documentation is often written with paragraphs wrapped at 80 column lines to
> make it easier for terminal use. You can probably set up your favorite text
> editor to do this automatically for you.
> This is not a requirement, though.

### Prose Style

In general, try to write simple, declarative prose. We prefer short,
single-clause sentences and brief three-to-five sentence paragraphs. Try to
choose vocabulary that is straightforward and precise. Avoid creating new terms,
using obscure terms or, in particular, using a lot of jargon. For example, use
"use" instead of leveraging "leverage".

That said, don’t feel like you have to write for localization or for
English-as-a-second-language (ESL) speakers specifically. Assume you are writing
for an ordinary speaker of English with a basic university education. If your
prose is simple, clear, and straightforward it will translate readily.

One way to think about this is to assume developers working with Adobe's APIs are generally university
educated and read at least a "16th" grade level (meaning they have a
university degree). You can use a
[readability tester](https://readable.io/) to help guide your judgment. For
example, the readability score for the phrase "Containers should be ephemeral"
is around the 13th grade level (first year at university), and so is acceptable.

You should not assume that readers have completed a computers science degree, as many developers are self-taught or have learned at coding bootcamps. This means that you do not have to introduce or define simple concepts and acronyms like API or "importing a module".  More complex, and formal concepts can be used, but should be followed by an explanation. 

For example:

* "Containers should be ephemeral, *they can be stopped at any time.*"
* "HTTP PUT requests are idempotent, *this means making the same request twice will yield the same result.*"
* "The `sort` method has linear time complexity, *sorting twice as many items will take two times as long*"

In all cases, we prefer clear, concise communication over stilted, formal
language. Don't feel like you have to write documentation that "sounds like
technical writing."
Technical documentation should read like the explanations of a friendly, helpful experienced co-worker that you just reached out to via chat.

Content on Adobe I/O should be written as if passed in a conversation “from developer to developer”. 

Imagine Adobe I/O as the helpful colleague in the office next door, who is always willing to explain, but never condescending, who always has an answer, but never makes you feel like she knows it better, who  can always find humor in a difficult situation, but never avoids the hard questions.

Put the user first, the developer second, the technology third – our technology does not matter, what matters is what **you** can do with it for *your user*.

### Metaphor and Figurative Language

One exception to the "don’t write directly for ESL" rule is to avoid the use of
metaphor or other
[figurative language](http://en.wikipedia.org/wiki/Literal_and_figurative_language) to
describe things. There are too many cultural and social issues that can prevent
a reader from correctly interpreting a metaphor. This is especially the case for sports metaphors.

### Other Style Tips

Use active voice in instructions and when describing system behavior. Instead of "The API Gateway is used to apply rate limits to incoming HTTP requests" write "The API Gateway applies rate limits to incoming HTTP requests.

Address the reader directly and write "you can do this" instead of "this can be done".

Do not use buzzwords and adjectives that do not describe the concept at hand, the purpose of our documentation is to explain and educate, not to sell.

## Specific Conventions

Below are some specific recommendations (and a few deviations) from AP style
that we use in our docs.

### Contractions

As long as your prose does not become too slangy or informal, it's perfectly
acceptable to use contractions in our documentation. Make sure to use
apostrophes correctly.

### Use of Dashes in a Sentence.

Dashes refers to the en dash (–) and the em dash (—). Dashes can be used to
separate parenthetical material.

Usage Example: This is an example of a PhoneGap client – which uses the Big Widget
to run – and does x, y, and z.

Use dashes cautiously and consider whether commas or parentheses would work just
as well. We always emphasize short, succinct sentences.

More info from the always handy [Grammar Girl site](http://www.quickanddirtytips.com/education/grammar/dashes-parentheses-and-commas).

### Pronouns

It's okay to use first and second person pronouns, especially if it lets you avoid a passive construction. Specifically, always use "we" to
refer to Adobe and "you" to refer to the user. For example, "We built the
`exec` command so you can resize a TTY session." That said, in general, try to write simple, imperative sentences that avoid the use of pronouns altogether. Say "Now, enter your SSH key" rather than "You can now enter your SSH key."

As much as possible, avoid using gendered pronouns ("he" and "she", etc.).
Either recast the sentence so the pronoun is not needed or, less preferably,
use "they" instead. If you absolutely can't get around using a gendered pronoun,
pick one and stick to it. Which one you choose is up to you. One common
convention is to use the pronoun of the author's gender, but if you prefer to
default to "he" or "she", that's fine too.

### Capitalization

#### In General

Only proper nouns should be capitalized in body text. In general, strive to be
as strict as possible in applying this rule. Avoid using capitals for emphasis
or to denote "specialness".

#### Starting Sentences

Because code samples should always be written exactly as they would appear
on-screen, you should avoid starting sentences with a code sample.

#### In Headings

Headings take title case to differentiate from sentence case in normal text and to increase readability and to make it easier to skim text.

1. Capitalize the first word of the title/heading and of any subtitle/subheading;
2. Capitalize all “major” words (nouns, verbs, adjectives, adverbs, and pronouns) in the title/heading, including the second part of hyphenated major words (e.g., Self-Report not Self-report)

### Punctuation

#### Periods

We prefer one space after a period at the end of a sentence, not two.

See [lists](doc-style.md#lists) below for how to punctuate list items.

#### Exclamation Marks and Semicolons

Both should be avoided. If you need a semicolon, try to rewrite your sentence as two, shorter sentences. The need for an exclamation mark is often an indicator for deeper issues in the content:

> "This feature is really cool!" should be rewritten as "With this feature, you can do this …, which is useful, because …"

> "Don't forget to call `Session.save()`!" can be better written as a note or warning in a separate paragraph.

> "Click the button labeled **next**!" works just as well as "Click the button labeled **next**" and reads much nicer.

### Abbreviations and Acronyms

* Exempli gratia (e.g.) and id est (i.e.): these should always have periods and
are always followed by a comma.

* Acronyms are pluralized by simply adding "s", e.g., PCs, OSs, APIs. Do not use apostrophes to pluralize acronyms

* On first use on a given page, the complete term should be used, with the
abbreviation or acronym in parentheses. E.g., Red Hat Enterprise Linux (RHEL).
The exception is common, non-technical acronyms like AKA or ASAP. Note that
acronyms other than i.e. and e.g. are capitalized.

* Other than "e.g." and "i.e." (as discussed above), acronyms do not take
periods, PC not P.C.

#### Do not Abbreviate These Words

Do not abbreviate these words, as they can introduce colloquialisms, make writing less clear, and lead to confusion:

* developer, developers (not dev or devs)
* administrator, administration, or administrative (not admin)
* repository, repositories (not repo or repos)

### Lists

When writing lists, keep the following in mind:

Use bullets when the items being listed are independent of each other and the
order of presentation is not important.

Use numbers for steps that have to happen in order or if you have mentioned the
list in introductory text. For example, if you wrote "There are three config
settings available for SSL, as follows:", you would number each config setting
in the subsequent list.

In all lists, if an item is a complete sentence, it should end with a
period. Otherwise, we prefer no terminal punctuation for list items.
Each item in a list should start with a capital.

### Structuring Documents

Avoid deep nesting of document structure. Three levels of headings are usually enough.

The same applies to lists: avoid lists that are nested too deeply, in most cases two levels should be enough.

### Numbers

Write out numbers in body text and titles from one to twelve. From 13 on, use numerals.

### Notes

Use notes sparingly and only to bring things to the reader's attention that are
critical or otherwise deserving of being called out from the body text. Please
format all notes as follows:

    ###### Note
    One line of note text
    another line of note text

### Examples

When possible, use examples to make it easier to understand complex concepts. Examples can be either text or code examples.

Some of the technical documentation templates provide special formatting for examples, so please format text examples in Markdown as follows:

```
> One line of example text
> another line of example text
```

### Avoid excess use of "i.e."

Minimize your use of "i.e.". It can add an unnecessary interpretive burden on
the reader. Avoid writing "This is a thing, i.e., it is like this". Just
say what it is: "This thing is …"

### Preferred usages

#### Login vs. Log In.

A "login" is a noun (one word), as in "Enter your login". "Log in" is a compound
verb (two words), as in "Log in to the terminal".

### Oxford comma

One way in which we differ from AP style is that Adobe's developer documentation uses the [Oxford
comma](http://en.wikipedia.org/wiki/Serial_comma) in all cases. 

### Code and UI Text Styling

We require `code font` styling (monospace, sans-serif) for all text that refers
to a command or other input or output from the CLI. This includes file paths
(e.g., `/etc/hosts/docker.conf`). If you enclose text in backticks (\`), markdown
will style the text as code.

Text from a CLI should be quoted verbatim, even if it contains errors or its
style contradicts this guide. You can add "(sic)" after the quote to indicate
the errors are in the quote and are not errors in our docs.

Text taken from a GUI, such as menu text or button text, should be bold.
Use the text exactly as it appears in the GUI. For example:

```none
Click **Continue** to save the settings.
```

Text that refers to a keyboard command or hotkey should be capitalized and bold. For example: **Ctrl-D**.

When writing CLI examples, give the user hints by making the examples resemble
exactly what they see in their shell:

* Add three backticks (\`) before and after shell examples so they get rendered as code blocks.
* Start typed commands with `$ ` (dollar space), so that they are easily
  differentiated from program output.
* Program output has no prefix.
* Comments begin with `# ` (hash space).

Please test all code samples to ensure that they are correct and functional so
that users can successfully copy-and-paste samples directly into the CLI.

## Pull requests

The pull request (PR) process is in place so that we can ensure changes made to
the docs are the best changes possible. A good PR will do some or all of the
following:

* Explain why the change is needed
* Point out potential issues or questions
* Ask for help from experts in the company or the community
* Encourage feedback from core developers and others involved in creating the
  software being documented.

Writing a PR that is singular in focus and has clear objectives will encourage
all of the above. Done correctly, the process allows reviewers (maintainers and
community members) to validate the claims of the documentation and identify
potential problems in communication or presentation.

### Commit messages

In order to write clear, useful commit messages, please follow these
[recommendations](http://robots.thoughtbot.com/5-useful-tips-for-a-better-commit-message).

## Links

For accessibility and usability reasons, avoid using phrases such as "click
here" for link text. Recast your sentence so that the link text describes the
content of the link, as we did in the
["Commit messages" section](#commit-messages) above.

## Graphics

When you need to add a graphic, try to make the file size as small as possible.
If you need help reducing file size of a high-resolution image, feel free to
contact us for help.
Usually, graphics should go in the same directory as the `.md` file that
references them, or in a subdirectory for images if one already exists.

The preferred file format for graphics is PNG, but GIF and JPG are also
acceptable.

If you are referring to a specific part of the UI in an image, use
call-outs (circles and arrows or lines) to highlight what you’re referring to.
Line width for call-outs should not exceed five pixels. The preferred color for
call-outs is red.

Be sure to include descriptive alt-text for the graphic. This greatly helps
users with accessibility issues.

Lastly, be sure you have permission to use any included graphics.

## Word Lists

### How to Handle These Common Words

* add-on (noun, adjective), add on (verb)
* back end (noun), back-end (adjective)
* double-click
* drop-down (noun, adjective), drop down (verb)
* email (never hyphenate, never capitalize unless it begins a sentence) 
* front end (noun), front-end (adjective)
* internet (never capitalize unless it begins a sentence)
* online (never capitalize unless it begins a sentence)
* opt-in (noun, adjective) , opt in (verb)
* pop-up (noun, adjective), pop up (verb)
* signup (noun, adjective), sign up (verb)
* username
* URL
* Open Source (capitalized)
* Inner Source (capitalized, with a space in the middle)

### Avoid These Buzzwords

* Leverage 
* Uplevel
* Innovative 
* Productivity
* Immersive 
* Orchestrate
* Optimize 
* Synergistic
* Actionable 
* Monetize
* Utilize

### Avoid These Tautologies

Developer API (all APIs are for developers)
