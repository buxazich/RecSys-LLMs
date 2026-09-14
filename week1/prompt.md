# Homework 1: Corrected Prompt

## Problem with the original prompt

The original request was too broad: it asked the AI assistant to create a random lunch recommender and publish it on GitHub Pages. That led the assistant to propose a new project instead of investigating and correcting the provided starter code.

## Corrected prompt

> Review the provided Random Lunch Menu Generator starter project. Do not create a new implementation from scratch and do not replace its design or core random-selection behavior.
>
> First, inspect the supplied `index.html` and identify concrete HTML, CSS, JavaScript, icon, accessibility, and documentation errors. Then make the smallest reasonable changes needed to fix those errors while preserving the starter project's structure and appearance.
>
> In particular, verify that every Font Awesome class exists in the linked Font Awesome 6.4.0 stylesheet, that repeated button clicks cannot create competing delayed updates, and that the generated result is accessible to keyboard and assistive-technology users.
>
> Update `README.md` so it accurately documents the files that really exist in the repository. Do not claim that `style.css`, `script.js`, `assets/`, or `LICENSE.md` exist unless those files are actually present. Use the final GitHub Pages URL in the Live Demo section.
>
> Finally, summarize each problem found and its correction. Keep the result as a corrected version of the provided starter code.

## Expected result

- The original one-file application structure is retained.
- Broken icon references are corrected.
- Rapid interaction does not create overlapping results.
- The interface works with a keyboard and assistive technology.
- The documentation matches the repository contents.
