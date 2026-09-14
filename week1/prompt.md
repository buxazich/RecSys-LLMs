# Homework 1: Random Lunch Menu Recommender

I am working with a provided starter project for a Random Lunch Menu Generator.

The starter project contains:

- `index.html` — the provided application code with inline HTML, CSS, and JavaScript.
- `prompt.md` — the original AI prompt and generated project description.

The application is intended to recommend a random lunch option and be published using GitHub Pages.

## Important homework requirement

This is a debugging and correction assignment.

Do not create a completely new application from scratch. Work only with the provided starter code and prompt. Preserve the existing design, project structure, lunch menu, and core random-selection behavior whenever possible.

## Your task

Carefully investigate both the supplied `index.html` and the original prompt.

### 1. Inspect the starter code

Analyze the existing HTML, CSS, and JavaScript and identify concrete problems, including:

- invalid or outdated Font Awesome icon classes;
- JavaScript behavior that may produce incorrect or overlapping results;
- repeated lunch recommendations;
- missing semantic HTML attributes;
- keyboard accessibility problems;
- screen-reader accessibility problems;
- animation and reduced-motion issues;
- documentation that does not match the actual project.

Do not assume that every item listed above is necessarily broken. Verify each issue before changing the code.

### 2. Correct the application

Make the smallest reasonable changes required to fix the verified problems.

Requirements:

- Keep the application in the supplied `index.html`.
- Keep CSS and JavaScript inline unless separation is necessary to fix an actual error.
- Preserve the original visual design and layout.
- Preserve the existing lunch options.
- Preserve the random lunch recommendation behavior.
- Use valid Font Awesome 6.4.0 Free icon classes.
- Prevent rapid button clicks from producing competing delayed updates.
- Avoid showing the same lunch twice in succession when more than one option exists.
- Ensure that the Generate Lunch button works with a keyboard.
- Make dynamic results understandable to screen-reader users.
- Respect the user's reduced-motion preference.
- Do not introduce frameworks, build tools, package managers, or unnecessary dependencies.

### 3. Correct the documentation

Create or update `README.md` so that it accurately describes the corrected starter project.

The README must contain:

- project title and short description;
- homework objective;
- link to the live GitHub Pages demo;
- table of the problems found and their corrections;
- explanation of how the application works;
- actual project structure;
- local launch instructions;
- technologies used.

Do not mention files that are not present in the repository. In particular, do not claim that separate `style.css`, `script.js`, `assets/`, or `LICENSE.md` files exist.

Use this live demo URL:

https://buxazich.github.io/RecSys-LLMs/week1/

Use this repository URL:

https://github.com/buxazich/RecSys-LLMs

## Required deliverables

Return the complete corrected contents of:

1. `index.html`
2. `README.md`

After the files, provide a concise table containing:

| Problem found | Why it was a problem | Correction made |
| --- | --- | --- |

Do not provide only isolated code snippets or a general explanation. Return complete files that can replace the supplied starter files directly.

## Acceptance criteria

The result is complete when:

- the supplied application structure is retained;
- the page loads without blocking HTML or JavaScript errors;
- all displayed icons exist and render correctly;
- the Generate Lunch button produces one valid result per interaction;
- rapid clicks cannot create overlapping results;
- the same recommendation does not appear twice consecutively;
- dynamic results are announced to assistive technology;
- keyboard focus is visible;
- reduced-motion preferences are respected;
- the README matches the actual repository;
- the GitHub Pages link points to the working application.

Before answering, review the final files against every acceptance criterion.
