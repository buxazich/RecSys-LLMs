# Random Lunch Menu Generator

A corrected version of the starter project provided for Homework 1. The application suggests a random lunch option when the user clicks the **Generate Lunch!** button.

## Homework objective

The purpose of this work is to investigate the provided prompt and starter code, identify their errors, and correct them. The project is based on the supplied `index.html`; it is not a new implementation created from scratch.

## Live demo

**[Open Random Lunch Menu Generator](https://buxazich.github.io/RecSys-LLMs/week1/)**

## Problems found and corrections

| Problem | Correction |
| --- | --- |
| The original prompt asked for a new project instead of an audit. | Replaced it with a prompt that explicitly requires minimal corrections to the starter files. |
| The README template listed files that did not exist. | Documented the actual one-file application structure. |
| Several Font Awesome icon names were invalid or outdated. | Replaced them with valid Font Awesome 6.4.0 classes. |
| Rapid clicks could start overlapping delayed updates. | Disabled the button while a result is being generated. |
| The same lunch could appear twice in a row. | Excluded the immediately previous result from the next draw. |
| Dynamic results were not announced by assistive technology. | Added a live status region and hid decorative icons from screen readers. |
| Keyboard focus and reduced-motion preferences were not handled. | Added visible focus and reduced-motion styles. |

## How it works

1. The page stores the starter lunch options in a JavaScript array.
2. On page load or button click, JavaScript selects a random array item.
3. The selected lunch name and icon appear after a short loading animation.
4. The immediately previous option is excluded from the next draw.

## Project structure

```text
week1/
├── index.html  # Corrected starter application with inline CSS and JavaScript
├── prompt.md   # Corrected prompt used to audit the starter project
└── README.md   # Project description and documented corrections
```

## Run locally

Clone or download the repository, then open `week1/index.html` in a web browser. No build step or package installation is required.

## Technologies

- HTML5
- CSS3
- JavaScript
- Font Awesome 6.4.0
- GitHub Pages
