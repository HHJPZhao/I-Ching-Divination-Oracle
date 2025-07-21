# I-Ching-Divination-Oracle
I Ching Divination Oracle 64 Hexagrams
User Manual: The I Ching Divination Oracle

[https://hhjpzhao.github.io/I-Ching-Divination-Oracle/] (https://hhjpzhao.github.io/I-Ching-Divination-Oracle/)

1. Welcome to the Oracle
Welcome! This guide will walk you through how to use the I Ching Divination Oracle application. The I Ching, or Book of Changes, is an ancient oracle with roots in Chinese philosophy. It does not predict the future, but rather offers wisdom and insight into your current situation, helping you to reflect and make decisions with greater clarity.

Approach your questions with sincerity and an open mind. The oracle responds best to questions about your own conduct and attitude, such as "What is the best approach to my current challenge?" rather than "Will I get the job?"

2. How to Begin a Reading
To begin your consultation with the oracle, simply focus on your question or the situation you wish to gain insight into. When you feel ready, press the "Begin Casting" button.

This will initiate the process of building your hexagram, one line at a time.

3. The Casting Process: Tossing the Coins
A hexagram is made of six lines, and each line is determined by a simulated toss of three coins. You will perform this action six times to build the complete hexagram.

Building Upwards: The hexagram is built from the bottom to the top. The first line you cast will be the bottom line, and the sixth and final line will be the top line.

Casting a Line:

Click the "Cast Line..." button.

An animation will show three coins being tossed.

The outcome of the coin toss determines the type of line that is drawn.

Understanding the Lines: There are four possible outcomes for each toss, resulting in two types of lines:

Stable Lines (Unchanging):

--- (Solid Line): A young, stable yang line.

--- --- (Broken Line): A young, stable yin line.
These lines form the foundation of your primary hexagram but do not change.

Changing Lines:

---X--- (Solid Line with an X): An old, changing yang line. This line is full of energy and is about to transform into its opposite (a yin line).

--O-- (Broken Line with an O): An old, changing yin line. This line is at a point of transition and is about to become a yang line.

Changing lines are important because they reveal where the energy of your situation is shifting, leading to a second hexagram.

4. Understanding Your Results
Once you have cast all six lines, the "Show Result" button will appear. Clicking it will reveal your reading, which may include one or two hexagrams.

The Primary Hexagram: This is the first hexagram you see, formed by the initial state of the six lines you cast. It represents your current situation and the primary forces at play. Read its Judgment and Image texts carefully for the core message.

The Relating (or Transformed) Hexagram: If your casting included one or more changing lines (X or O), a second hexagram will also be displayed. This hexagram is formed by transforming the changing lines into their opposites. It points to where your current situation is heading or reveals an underlying context to your question.

5. A Note on Interpretation
The wisdom of the I Ching is symbolic and poetic. The texts are not meant to be literal instructions but rather catalysts for your own intuition and reflection.

The Judgment (彖辭): This provides the core decision or assessment of the situation.

The Image (象辭): This describes the symbolism of the two trigrams that make up the hexagram and advises how a wise person (君子, jūnzǐ) would act in harmony with its spirit.

Take your time with the reading. Let the imagery and advice settle in your mind. The insights you gain are a reflection of your own inner wisdom, awakened by the oracle.


# GitHub Rulebook: The I Ching Divination Oracle Project

## 1. Introduction

Welcome to the I Ching Divination Oracle project! This document serves as the official rulebook for contributing to this repository. Its purpose is to ensure a smooth, transparent, and collaborative development process. By following these guidelines, we can maintain high code quality, keep our history clean, and make it easy for everyone to contribute effectively.

---

## 2. Core Philosophy

* **Respect & Collaboration:** Treat all contributors with respect. Open discussion and constructive feedback are the cornerstones of our collaboration.
* **Clarity & Intention:** Your code, commits, and pull requests should be as clear as possible. Explain *why* you are making a change, not just *what* you changed.
* **Preserve the Spirit:** The project blends ancient wisdom with modern technology. All contributions should honor this spirit by being thoughtful, well-crafted, and aesthetically pleasing.

---

## 3. Branching Strategy

We use a simplified Git-Flow model. All development happens on feature branches, which are then merged into `develop`. The `main` branch is reserved for stable, production-ready releases.

* **`main` Branch:**
    * This branch is **protected**. Direct pushes are forbidden.
    * It represents the official, live version of the application.
    * Merges to `main` only happen from the `develop` branch when preparing for a new release and must be done via a Pull Request.

* **`develop` Branch:**
    * This is the primary branch for ongoing development. It is the base from which all feature branches are created.
    * It should always be in a state where it could potentially be released, though it may contain uncompleted features.

* **Feature Branches:**
    * All new features, bug fixes, or style changes must be done in a feature branch.
    * Create your branch from the latest version of `develop`.
    * Use a descriptive naming convention:
        * For new features: `feature/bilingual-text-updates`
        * For bug fixes: `fix/coin-animation-glitch`
        * For documentation: `docs/update-rulebook`
        * For refactoring: `refactor/hexagram-data-structure`

---

## 4. Committing Code

Clean, atomic commits create a readable history, which is invaluable for debugging and understanding the project's evolution.

* **Commit Style:** We follow the [**Conventional Commits**](https://www.conventionalcommits.org/) specification. This makes our commit history easy to read and allows for automated changelog generation.
    * **Format:** `<type>[optional scope]: <description>`
    * **Common Types:**
        * `feat`: A new feature (e.g., adding the coin toss animation).
        * `fix`: A bug fix (e.g., correcting a typo in a hexagram's text).
        * `style`: Code style changes that do not affect logic (e.g., formatting, whitespace).
        * `refactor`: Code changes that neither fix a bug nor add a feature.
        * `docs`: Changes to documentation (like this rulebook).
        * `chore`: Routine tasks and maintenance.

* **Commit Messages:**
    * **Subject:** Write a concise, imperative-mood subject line (e.g., `feat: add coin toss animation`).
    * **Body (Optional):** If the change is complex, use the commit body to explain the 'what' and 'why'.

    **Example Commit:**
    ```
    feat: add bilingual Chinese interpretations

    Integrates the original Chinese text for hexagram names, judgments,
    and images into the data structure and result cards. This provides a
    more authentic experience for users.

    - Adds Noto Serif SC font for clear Chinese character rendering.
    - Updates the data array with `chinese_judgment` and `chinese_image`.
    - Modifies the `createHexagramCard` function to display text bilingually.
    ```

---

## 5. Pull Requests (PRs)

Pull Requests are the heart of our review process. All code must be reviewed before being merged into the `develop` branch.

* **Process:**
    1.  Push your `feature/*` or `fix/*` branch to the GitHub repository.
    2.  Create a Pull Request targeting the `develop` branch.
    3.  Fill out the PR template completely.
    4.  Request a review from at least one other contributor.
    5.  Address any feedback or requested changes by pushing new commits to your branch.

* **PR Template:**
    * **Title:** Use a clear, descriptive title that summarizes the changes.
    * **Description:**
        * **What does this PR do?** Briefly describe the changes.
        * **Why is this change needed?** Explain the problem or the goal.
        * **How to test:** Provide steps for the reviewer to test your changes.
    * **Link Issues:** If your PR resolves an open issue, use keywords like `Closes #123`.

---

## 6. Code Quality & Style

Consistency is key. The style of the project should feel unified, regardless of who wrote the code.

* **Follow Existing Style:** Look at the existing HTML, CSS, and JavaScript and follow its patterns for naming, formatting, and structure.
* **Comments:** Write clear comments for complex logic. The I Ching calculations, state management, and animation sequences are good candidates for detailed comments.
* **Linter/Formatter:** The project should be configured with Prettier for code formatting and ESLint for identifying potential issues. Ensure your code is clean according to these tools before submitting a PR.

---

## 7. Issue Tracking

Use GitHub Issues to track bugs, feature requests, and other tasks.

* **Bug Reports:** Use the "Bug Report" template. Provide a clear title, steps to reproduce the bug, expected behavior, and actual behavior.
* **Feature Requests:** Use the "Feature Request" template. Clearly describe the proposed feature and explain why it would be a valuable addition.
* **Labels:** Use labels (`bug`, `enhancement`, `documentation`, `help-wanted`) to keep our issues organized.

---

## 8. Code of Conduct

All contributors are expected to adhere to the project's Code of Conduct. We are committed to providing a welcoming and harassment-free environment for everyone. (A `CODE_OF_CONDUCT.md` file based on the Contributor Covenant should be added to the repository root).
