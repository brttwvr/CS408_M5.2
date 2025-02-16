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

    - Using the contrast checker at https://webaim.org/resources/contrastchecker/, with the background value of #dde and foreground value of #2a2a2a, the returned result was a contrast ratio of 10.69:1, which passed for all tests, including WCAG AA and AAA for normal text, WCAG AA and AAA for large text, and WCAG AA for graphical objects and user interface components.  Based on these results, I made no further changes to the color. 
    

    Semantic HTML

    The content is still not very accessible — report on what happens when you try to navigate it using a keyboard.

    - The tab key allows navigation to links, inputs, buttons, and the audio controls. The arrows up and down allow for scrolling on the page.  

    Can you update the article text to make it easier for screen reader users to navigate?
    The navigation menu part of the site (wrapped in <div class="nav"></div>) could be made more accessible by putting it in a proper HTML semantic element. Which one should it be updated to? Make the update.

    - This was switched to the nav element.  







add semantic html (eg, h1, p, etc)

add alt text to images 