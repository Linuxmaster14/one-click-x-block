# One-Click X/Twitter Block

A Tampermonkey userscript that adds a one-click block button next to every username on X/Twitter.

## Features

- Block button on `@username` handles in followers, following, lists, search results, and profiles
- Block button on tweet timestamps in timelines and replies
- Blocked users are automatically hidden from lists
- Blocked users persist across sessions
- Detects already-blocked users and hides them
- Skips your own profile
- Falls back to profile redirect when direct block isn't available
- SPA-aware: works with X's dynamic navigation

## Install

1. Install [Tampermonkey](https://www.tampermonkey.net/)
2. Create a new script and paste the contents of `one-click-x-block.user.js`
3. Visit [x.com](https://x.com)

## How It Works

Clicking the block icon (⊘) triggers X's native block flow: opens the "More" menu, clicks "Block", and confirms.

If the "More" menu isn't available, the script redirects to the user's profile, blocks, and navigates back.

## License

MIT
