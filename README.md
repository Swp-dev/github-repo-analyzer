# GitHub Repository Analyzer CLI

A simple CLI tool to analyze any GitHub repository and display useful statistics directly in the terminal.

It fetches repository data from the GitHub API and presents it in a clean, formatted output including repository metrics, language distribution, and commit activity graphs.

---

## 📌 Features

* Repository statistics overview
* Stars, forks, watchers, issues
* Contributor and release count
* Language usage chart
* Commit activity graph (weekly commits)
* Clean terminal UI with tables and charts

---

## 📦 Installation

Clone the repository:

```
git clone https://github.com/Swp-dev/github-repo-analyzer.git
cd github-repo-analyzer
```

Install dependencies:

```
npm install
```

Run the tool:

```
node analyze.js owner/repo
```

Example:

```
node analyze.js facebook/react
```

---

## 🔔 Example Output

```
GitHub Repository Analyzer

Repository: facebook/react
Stars: 230000
Forks: 48000
Watchers: 6700
Open Issues: 1000
Primary Language: JavaScript
Contributors: 1600
Releases: 250
Created: Tue May 29 2013
Last Update: Fri Mar 07 2026
```

Languages chart example:

```
Languages

JavaScript   ████████████████████ 82.3%
TypeScript   ████                 10.1%
CSS          ██                    5.2%
Other        █                     2.4%
```
---

## Usage

Basic command:

```
node analyze.js owner/repo
```

Example:

```
node analyze.js king/awesome
node analyze.js vercel/domain
node analyze.js hello/open-src
```

---

## Star Goals

If this project receives community support, new features will be added.

### ⭐️ 15 Stars — Version 2

Add GitHub token support to increase API rate limits.

Why this matters:

GitHub limits unauthenticated requests to:

```
60 requests per hour
```

Authenticated requests allow:

```
5000 requests per hour
```

How to create a GitHub token:

1. Go to:

```
https://github.com/settings/tokens
```

2. Click **Generate new token (classic)**

3. Enable permission:

```
public_repo
```

4. Copy the token.

Example usage (planned in v2):

```
export GITHUB_TOKEN=your_token_here
node analyze.js facebook/react
```

---

### ⭐️ 50 Stars — Version 3

HTML Dashboard Report

Version 3 will introduce a web-based report for each analyzed repository.

Instead of only CLI output, the tool will generate a visual dashboard including:

* repository statistics
* interactive charts
* language distribution graphs
* commit activity charts
* contributor insights

Example command:

```
node analyze.js facebook/react --html
```

Output:

```
report.html
```

Opening the report will show a full dashboard in the browser.

---

## 🌐 Roadmap

Future improvements may include:

* repository health score
* contributor leaderboard
* popularity score
* export reports
* npm global CLI support

---

## ❤️ Contributing

Contributions are welcome.

You can help by:

* opening issues
* submitting pull requests
* suggesting features

---

## License

MIT License
