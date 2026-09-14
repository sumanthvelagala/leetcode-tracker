# LeetCode Company Tracker

A static web app to browse, filter, and track company-tagged LeetCode questions ranked by frequency.

**Live site:** https://sumanthvelagala.github.io/leetcode-tracker

## Features

- Filter questions by company, topic, difficulty
- Sorted by frequency (probability of being asked)
- Mark questions as solved — saved in your browser
- Export/Import progress as JSON to move between devices
- 436+ companies supported
- No login required, no backend

## Data Source

All question data is sourced from the community-maintained repository:

**[liquidslr/leetcode-company-wise-problems](https://github.com/liquidslr/leetcode-company-wise-problems)**

This app does not host or redistribute any question data. It fetches CSVs directly from that repository at runtime via `raw.githubusercontent.com`. All credit for the data goes to the contributors of that repo.

## How it works

- On load, fetches `5. All.csv` for each selected company from the source repo
- Data is cached in your browser for 24 hours
- Solved progress is stored in localStorage and can be exported as JSON

## Disclaimer

This tool is for personal interview preparation only. All LeetCode problem titles and links belong to [LeetCode](https://leetcode.com).
