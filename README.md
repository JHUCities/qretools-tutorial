# The QREtools tutorial

Learn QREtools with 35 short lessons. Each lesson is a file with one or two gaps to
fill in. Part 1 makes a small bank of questions about the parks of a neighborhood.
Part 2 makes a survey that asks those questions.

All the lessons work in the same way. Open the file of the lesson, read the comment at
the top, and do the steps. When you finish the steps, the dashed circle beside the file
becomes a green tick. Then go to the next lesson.

## Before you start

1. **Make your own copy.** At the top of this page, press **Use this template** →
   **Create a new repository**. A private repository is permitted. Do not tick
   "Include all branches".
2. **Install the QREtools app** on your copy:
   <https://github.com/apps/qretools/installations/new>. Select your account, then
   "Only select repositories", then your copy. Without the app you can read the lessons,
   but you cannot save them.
3. **Open your copy in QREtools.** Go to <https://qretools.com>, write your copy as
   `owner/name`, and sign in with GitHub.
4. **Open lesson 2.** In the tree on the left, open Questions → `lesson02_intent` →
   `consent`.

**To save your work:** press **Save** on each file when its tick is green. Save puts
the open file on your own branch on GitHub (`qretools-<your login>`). Your work is then
safe if you close the tab. `main` does not change until you open a pull request and
merge it. The pull-request icon beside the name of your branch ("Propose changes")
opens a pull request.

**If you cannot do a lesson:** the complete tutorial is on the
[`solutions` branch](https://github.com/JHUCities/qretools-tutorial/tree/solutions) of
the original repository. Compare your file with the same file on that branch.

## From a terminal

`qretools check .` lists the fields to fill in and the errors to correct. These are the
same findings that the app shows. `mise.toml` gives the versions of Node and of
`qretools`. With [mise](https://mise.jdx.dev), run `mise install`, then run
`qretools check .`. Without mise, run `npx qretools@<the version in mise.toml> check .`.
To get a later version, change the version in `mise.toml`.

## The lessons

**Part 1: the question bank** (Questions, in the tree)

Lesson 1 is in Settings → `workspace.yaml`: the agency, the code every question here is published under.

| # | Folder | You learn |
|---|---|---|
| 2 | `lesson02_intent` | a question's parts; the intent; to-fill-in circles and the Findings list |
| 3 | `lesson03_text` | the question text; the optional title, source and note |
| 4 | `lesson04_options` | response options: codes and labels |
| 5 | `lesson05_number` | a number question: min, max, decimals |
| 6 | `lesson06_open` | a free-text question; completion (Cmd-I) |
| 7 | `lesson07_craft` | advice on wording: one question, one thing; saving |
| 8 | `lesson08_shared_scale` | shared scales; the inspector; go to a definition |
| 9 | `lesson09_use_the_name` | warnings and quick fixes |
| 10 | `lesson10_new_scale` | making a new shared scale |
| 11 | `lesson11_concept` | shared concepts |
| 12 | `lesson12_universe` | the universe: whom a question is for |
| 13 | `lesson13_instruction` | instructions to the respondent |
| 14 | `lesson14_unit` | units |
| 15 | `lesson15_select_all` | select all that apply; "None of these" |
| 16 | `lesson16_fill` | fills: an earlier answer's words in the text |
| 17 | `lesson17_required` | settings: a field every question must have |
| 18 | `lesson18_required_in` | settings: a field one folder must have |
| 19 | `lesson19_missing` | settings: missing values |
| 20 | `lesson20_select_all_storage` | settings: how select all that apply is stored |
| 21 | `lesson21_variants` | duplicates across the bank, and deliberate variants |
| 22 | `lesson22_your_own` | your own question from scratch; moving and deleting |

**Part 2: the instrument** (Instruments, in the tree)

| # | File | You learn |
|---|---|---|
| 23 | `lesson23_first_instrument` | an instrument: say, ask, the Outline |
| 24 | `lesson24_stop` | stop |
| 25 | `lesson25_branch` | if, then; whom a branch's questions are for |
| 26 | `lesson26_else_if` | else, and else if; `in {…}` |
| 27 | `lesson27_compute` | computed values; and, or |
| 28 | `lesson28_cast` | a computed number: cast, and reversing a scale |
| 29 | `lesson29_fill` | what fills a question's text |
| 30 | `lesson30_ask_twice` | asking a question twice: `as` |
| 31 | `lesson31_roster` | a roster: once per person; `{{index}}` |
| 32 | `lesson32_more` | a roster that asks "another?"; each |
| 33 | `lesson33_checks` | checks: info, warning, blocking |
| 34 | `lesson34_order` | order, timing and inputs |
| 35 | `lesson35_survey` | the whole survey; DDI and Qualtrics downloads |

## Not in the tutorial

- **Questions from a different repository.** An instrument can ask the questions of a
  different workspace at a release (`uses: other: owner/repo@v1`). It cannot ask them at
  a branch. The [workspace template](https://github.com/JHUCities/qretools-template)
  tells you how to do this, and how QREtools numbers the DDI version of a question.
- **`legacy`.** A field that brings in an older bank.

What QREtools is: [About QREtools](https://github.com/JHUCities/qretools#readme).

## How this tutorial is written

The instructional copy follows the writing rules of
[ASD-STE100](https://asd-ste100.org) (Simplified Technical English), Issue 9: one
instruction in each sentence, the imperative for each step, the active voice, the
present tense, full forms in place of contractions, and short sentences. The
specification is free to request from ASD, and its copyright stays with ASD, so this
repository records only our own decisions and does not reproduce any part of it.

Two things do not follow ASD-STE100:

- **The example questions.** The `text` of a question is what the respondent reads, so
  it is the instrument of measurement. Its wording follows the craft of survey design.
  The `intent`, the labels of the options, and the `say` lines of the instruments are
  the same.
- **The approved words.** ASD-STE100 has two parts: the writing rules and a dictionary
  of approved words. This tutorial follows the writing rules. Nobody has yet checked the
  copy against the dictionary, so some words here are probably not approved words.

## License

© 2026 Johns Hopkins University. The tutorial is licensed under Creative Commons
Attribution 4.0 International (CC BY 4.0, `LICENSE`): you may share and adapt it, for any
purpose, if you credit "QREtools tutorial, Johns Hopkins University" and link to the
license.
