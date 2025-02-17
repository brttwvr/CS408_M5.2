# Author - CS408 template and Brett Weaver 
# Lab No. M5.2

# web-dev-starter

This is a starter project for web development with no frameworks and minimal
dependencies. It is intended to be a starting point for web development projects
that are written in plain HTML, CSS, and JavaScript.

## Getting Started

To get started, clone this repository and run the following commands:

```bash
npm install
```
This will install the necessary dependencies for the project.

## Development

It is recommended to use the VSCode Live Server extension to run the project
locally. This will allow you to see changes in real-time as you make them. There
is no need to run a build process or refresh the page manually. Additionally,
you do not need to setup a local server to run the project.

## Testing

To run the tests for the project, run the following command:

```bash
npm test
```

## Accessibility Lab Answers

Color

 The text is difficult to read because of the current color scheme. Can you do a test of the current color contrast (text/background), report the results of the test, and then fix it by changing the assigned colors?

- Using the contrast checker at https://webaim.org/resources/contrastchecker/, with the background value of #00FF00 and foreground value of #000000, the returned result was a contrast ratio of 1:1, which failed for all tests, including WCAG AA and AAA for normal text, WCAG AA and AAA for large text, and WCAG AA for graphical objects and user interface components.  Based on these results, I updated the background color to white.    
    
Semantic HTML

The content is still not very accessible — report on what happens when you try to navigate it using a keyboard.

- The tab key allows navigation to links, inputs, buttons, and the audio controls. The arrows up and down allow for scrolling on the page.  

Can you update the article text to make it easier for screen reader users to navigate?
The navigation menu part of the site (wrapped in <div class="nav"></div>) could be made more accessible by putting it in a proper HTML semantic element. Which one should it be updated to? Make the update.

- This was switched to the nav element.  I also updated index.html to use appropriate semantic HTML (eg., h1, p, etc.), as well as updating the corresponding references in style.css

The Images

The images are currently inaccessible to screen reader users. Can you fix this?

- I added alt text to the images for accessiblity. 

The Audio Player

The <audio> player isn't accessible to hearing impaired (deaf) people — can you add some kind of accessible alternative for these users?

- Yes, you can add an accessible transcript of the audio to allow for hearing impaired and deaf people to access the audio.

The <audio> player isn't accessible to those using older browsers that don't support HTML audio. How can you allow them to still access the audio?

- You can create custom controls to allow for access to those using such older browsers. 

The Forms

The <input> element in the search form at the top could do with a label, but we don't want to add a visible text label that would potentially spoil the design and isn't really needed by sighted users. How can you add a label that is only accessible to screen readers?

- I added an aria-label with the text "Search".

The two <input> elements in the comment form have visible text labels, but they are not unambiguously associated with their labels — how do you achieve this? Note that you'll need to update some of the CSS rule as well.

- I added labels for each of the name and comment. 

The Show/Hide Comment Control

The show/hide comment control button is not currently keyboard-accessible. Can you make it keyboard-accessible, both in terms of focusing it using the tab key and activating it using the return key?

- I added the role of button, and the tabindex of 0.

The Table

The data table is not currently very accessible — it is hard for screen reader users to associate data rows and columns together, and the table also has no kind of summary to make it clear what it shows. Can you add some features to your HTML to fix this problem?     

- I used th elements to define the table headers, and added the column and row scopes where appropriate to define the same. I also added a caption element with a summary as to what information the table provides. 

Other Considerations?

Can you list two more ideas for improvements that would make the website more accessible?

- Perhaps adding a means by which a transcript of the entire page can be generated and downloaded as a small file size could be useful. 

- Similarly, adding a tool that can read the text of the page, or the transcript, to the user by pressing a button.

