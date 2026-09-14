# Random Lunch Menu Generator

A debugged and corrected version of the Random Lunch Menu Generator supplied for Homework 1. The application recommends one random lunch option when the user clicks the **Generate Lunch!** button.

## Homework objective

The purpose of this homework is to investigate the provided prompt and code, identify concrete errors, and fix them. This repository corrects the supplied starter project; it does **not** replace it with a new implementation.

The original layout, inline HTML/CSS/JavaScript structure, twelve lunch options, and random-selection behavior were retained. Only changes needed to correct verified problems were made.

**[View the original starter project](https://github.com/dryjins/RecSys-LLMs/tree/main/week1)**

## Live demo

**[Open Random Lunch Menu Generator](https://buxazich.github.io/RecSys-LLMs/week1/)**

## Problems found and corrections

| Problem found | Why it was a problem | Correction made |
| --- | --- | --- |
| The original prompt led to creating a new project instead of examining the supplied files. | This contradicted the homework objective: debug and correct the given starter project. | Reworked the prompt so it requires an investigation and minimal corrections within the starter structure. |
| The generated README described separate `style.css`, `script.js`, `assets/`, and `LICENSE.md` files. | Those files do not exist inside `week1`, so the documented structure and launch instructions were inaccurate. | Documented the actual files and the inline CSS/JavaScript implementation. |
| `fa-bowl-hot`, `fa-pasta`, and `fa-bowl` were not available in the linked Font Awesome 6.4.0 Free stylesheet. | The corresponding food icons could appear blank. | Replaced only those unavailable names with valid Free icon classes while preserving every lunch option. |
| Every click created a new delayed update. | Rapid clicks could leave several timers competing to replace the displayed result. | Disabled the button during the existing 500 ms generation delay, allowing one result per interaction. |
| The changing result had no live-region semantics, and decorative icons had no accessibility treatment. | Screen-reader users might not hear the generated result and could hear irrelevant icon content. | Added a polite atomic status region and marked decorative icons as hidden from assistive technology. |
| The starter had no explicit keyboard focus style or reduced-motion override. | Focus could be difficult to locate, while transitions and the result animation could be uncomfortable for motion-sensitive users. | Added a high-contrast `:focus-visible` outline and a `prefers-reduced-motion` media query. |

## How it works

1. The page stores the starter lunch options in a JavaScript array.
2. On page load or button activation, JavaScript selects a random array item.
3. The button is temporarily disabled while the existing loading state is shown.
4. After 500 ms, the selected lunch name and icon replace the loading state and the button becomes available again.

## Project structure

```text
week1/
├── index.html  # Corrected starter application with inline CSS and JavaScript
├── prompt.md   # Corrected prompt used to audit the starter project
└── README.md   # Project description and documented corrections
```

## Run locally

Clone the repository and open `week1/index.html` in a web browser:

```bash
git clone https://github.com/buxazich/RecSys-LLMs.git
cd RecSys-LLMs/week1
```

No build step or package installation is required.

## Technologies

- HTML5
- CSS3
- JavaScript
- Font Awesome 6.4.0
- GitHub Pages
