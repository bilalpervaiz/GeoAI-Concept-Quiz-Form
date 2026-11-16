# Foundations of AI quiz

A 10-question, 15-minute quiz. Static files only, made for GitHub Pages.

## Files

- `index.html`: the quiz. This is the link you share.
- `results.html`: your results page. Keep this link to yourself.

## Host it on GitHub Pages

1. Create a new public repository, for example `ai-quiz`.
2. Upload `index.html` and `results.html` (Add file > Upload files) and commit.
3. Go to Settings > Pages, set Source to "Deploy from a branch", choose `main` and `/ (root)`, and save.
4. After a minute or two the site is live:
   - Quiz (share this): `https://YOUR-USERNAME.github.io/ai-quiz/`
   - Results (yours): `https://YOUR-USERNAME.github.io/ai-quiz/results.html`

## How the score reaches you

When he submits, the quiz posts one line (name, score, time used) to the free
notification service ntfy.sh, on this topic:

    bilal-ai-quiz-e21c4d8c76bd

`results.html` reads that topic. You can also get a push notification on your
phone: install the ntfy app and subscribe to the topic name above.

Things to know:

- ntfy.sh keeps messages for about 12 hours, so check results the same day.
- The topic name is the only protection. Anyone who has it (it is in the page
  source) can read or post to it. To change it, replace the topic name in both
  HTML files with any long random string.
- If the post fails, he is told to send you his result with "Copy result" or a
  screenshot.
- "One attempt" is remembered in his browser only. Another browser or a
  private window allows a retake.

## Change the questions

Edit the `Q` list near the top of the script in `index.html`. `a` is the
position of the correct option, counting from 0. The pass mark is `PASS = 7`.
