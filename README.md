# ai-branch

[![npm version](https://img.shields.io/npm/v/ai-branch.svg)](https://www.npmjs.com/package/ai-branch)
[![npm downloads](https://img.shields.io/npm/dm/ai-branch.svg)](https://www.npmjs.com/package/ai-branch)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/lxgic-studios/ai-branch)](https://github.com/lxgic-studios/ai-branch/stargazers)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0+-blue)](https://www.typescriptlang.org/)



Stop wasting time thinking up branch names. Just describe what you're doing and get a clean, conventional branch name back.

## Install

```bash
npm install -g ai-branch
```

## Usage

```bash
npx ai-branch "Add dark mode to settings"
# → feat/add-dark-mode-settings

npx ai-branch "Fix login redirect loop" --checkout
# → fix/login-redirect-loop (and checks it out)
```

## Setup

Set your OpenAI API key:

```bash
export OPENAI_API_KEY=sk-...
```

That's it. It'll pick the right prefix (feat, fix, chore, etc.) and format everything in kebab-case.

## Options

- `-c, --checkout` - Create the branch and switch to it automatically

## How it works

Sends your description to GPT-4o-mini, gets back a properly formatted branch name. Uses conventional prefixes so your git history stays clean.

## License

MIT
