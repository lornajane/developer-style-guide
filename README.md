# Developer Style Guide

A style guide for technical contributors to technical documentation projects. The goal is to be "just enough" guidance, short enough to read and yet comprehensive enough to support contributors who aren't specialist wordsmiths. This guide is published for your reference, or for you to adapt for your own purposes.

## Target a single audience and outcome

Know who you are writing for. The new junior developer needs different context and explanation than the Ops person trying to follow disaster recovery documentation. If it helps to think of a specific individual, do that. The key here is to not write down what you know, but write down what the reader needs to reach the desired outcome. An example outcome could be completing a task, learning about a specific topic, or understanding a set of options.

## Structure your writing

If your organisation offers templates, always use them; consistency helps readers a lot, even if the content is created by many authors. If not, try the [Diátaxis](https://diataxis.fr/) framework as inspiration on how to frame different content types - and don't be afraid to create more than one article from a single topic or assignment. If no structure is provided as a template, create your own by writing the subheadings of the piece before you write the words.

Use subheadings, images or diagrams, lists, and other content types to communicate to your readers. This "page furniture" helps them to navigate potentially long and complex technical articles.

## Be positive and inclusive

Focus on things the user _can_ do. Don't explain what can't be done, isn't supported, or hasn't been implmented yet unless these are central to the topic.

> Example: Instead of "you cannot back up your data yourself" you could say "data backups can be arranged by contacting the support team".

Inclusive language helps make your writing useful to the widest possible range of people. Avoid gendered language, using "they" and "theirs" rather than "he" or "she". Even when this feels clunky to write, it makes a positive impact on your readers. Other language to find alternatives for includes terms that could seem ableist such as using "OCD" or "crazy" in your writing. It's already standard practice to avoid socially-loaded terminology such as master/slave, blacklist/whitelist, and so on. Keeping a wordlist that is automatically checked, or using a tool like [AlexJS](https://alexjs.com/) can help with spotting words and phrases that can be improved.

Beware of jargon and abbreviations, because they can be difficult for newcomers to understand. Expand your abbreviations the first time you use them, and link to definitions or supporting content for any special terms to give the user the option of reading on , or clicking the link to learn more.

## Write commanding titles

Titles should use _imperative_ language to make it clear what the reader is doing in each section. It can feel like an abrupt style, but imagine ordering a small robot to perform each action and you will be pretty close. The side benefits of this approach are that it's often easier to translate, and tends to match user search terms more closely.

> Example: Instead of "Configuring the widget" use "Configure the widget"

Use sentence case for titles, and check them automatically using a tool like [Vale](https://vale.sh/). Add product names and other proper nouns to Vale to avoid false reports.

## Choose examples and screenshots wisely

If a picture is worth a thousand words, then a good example is worth at least twice that amount. In both cases:

- Choose content that the user will know or easily understand. Avoid "foo", and instead use "Alice" if it's a name, "Bucket" if it's a product, "paleblue" if it's a colour, and so on. Your reader will internalise that their data should look like your data.
- Avoid pop culture references, using these can exclude groups from other demographics than your own.
- Every example and screenshot needs text with it, explaining what it shows and why that's useful to the user.

Code examples are always valuable, adding more examples is usually a good thing.

Screenshots are both more difficult to get right and more difficult to maintain over time since small changes to a UI will mean repeating all the screenshots. Use them when you think the user would be likely to struggle with words alone. If you take a series of screenshots, use a small and consistent window size for them all. Always reduce the file size as much as you can, and include alt text on every image (tools such as [Markdownlint](https://github.com/DavidAnson/markdownlint) can check for alt text automatically).

## Add hyperlinks

Add links. Link to the tools you mention, the concepts that the user might not know already, and to other articles that are likely to be useful to this reader. Adding links to supporting material can enrich all content types, and help the reader to find their way to success.

Choose words that represent where the link goes to, such as "see the [section on hyperlinks](#add-hyperlinks)". Some tools will offer the links with their link text as a list, so meaningful words or phrases and avoiding duplicate link text within a page is good practice.

## Avoid technical documentation missteps

Technical writing has some unwritten norms that exist for mostly good reasons of readability and comprehension. In particular, here are some things you should NOT do:

- Use exclamation points. It's not a gossip magazine, it's technical documentation.
- Use question marks, especially in titles. It very easily reads like a car advert.
- Add emoji, unless the platform you are writing for has it as an established acceptable practice. Emoji are difficult to keep consistent between authors, can be distracting, and can also make the content less accessible.

---

## Using the developer style guide in your own projects

The guide is licensed under Creative Commons Zero, so please take it and do as you please. A link to where you found it is appreciated, but not required.

## Contributing to the style guide

Issues and pull requests are both welcome, but no promises are given that they will be accepted. Please note that this guide uses British English as standard.
