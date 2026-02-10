# Swiss German Verb Conjugation Practice

An interactive web application for practicing Swiss German verb conjugations.

## How It Works

- The app displays a random verb and asks you to match pronouns with their correct conjugations
- Click a pronoun on the left, then click the matching conjugation on the right
- Get instant feedback on whether your match is correct
- Track your score as you practice

## Pronouns

The app uses these Swiss German pronouns:
- ich
- du
- er/si/es
- mir
- ihr
- Si

## Setup

1. Open `index.html` in a web browser
2. The app will load verbs from `data/verbs.json`

## Adding Verbs

Edit `data/verbs.json` to add more verbs. The format is:

```json
[
  {
    "infinitive": "schaffe",
    "conjugations": [
      "schaffe",
      "shaffsch",
      "shafft",
      "shaffed",
      "shaffed",
      "shaffed"
    ]
  },
  {
    "infinitive": "another verb",
    "conjugations": [
      "ich form",
      "du form",
      "er/si/es form",
      "mir form",
      "ihr form",
      "Si form"
    ]
  }
]
```

**Important:** The conjugations array must have exactly 6 entries in this order:
1. ich
2. du
3. er/si/es
4. mir
5. ihr
6. Si

## Hosting on GitHub Pages

1. Initialize a git repository:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   ```

2. Create a new repository on GitHub

3. Push your code:
   ```bash
   git remote add origin https://github.com/yourusername/swissgerman-verbs.git
   git branch -M main
   git push -u origin main
   ```

4. Enable GitHub Pages:
   - Go to your repository settings
   - Navigate to "Pages"
   - Select "main" branch as source
   - Your site will be available at `https://yourusername.github.io/swissgerman-verbs/`

## Features

- Randomized verb selection
- Shuffled conjugations to prevent memorization by position
- Visual feedback for correct and incorrect matches
- Score tracking
- Responsive design
- Works offline once loaded
