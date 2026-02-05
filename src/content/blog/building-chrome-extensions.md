---
title: "Building Chrome Extensions That Don't Suck"
description: "Lessons learned from building MarkX and JSON Toolbox - practical tips for creating browser extensions users love."
pubDate: 2026-01-15
tags: ["chrome", "extensions", "javascript"]
---

After building several Chrome extensions used by thousands of developers, I've learned a few things about what makes a great extension.

## Keep It Simple

The best extensions do one thing really well. MarkX manages bookmarks. JSON Toolbox edits JSON. That's it.

Users don't want another Swiss Army knife. They want a tool that solves their specific problem without getting in the way.

## Performance Matters

Your extension runs in the background on every page. A few milliseconds of delay adds up to frustrated users.

Tips:

- Lazy load everything
- Minimize content script injection
- Use event pages instead of persistent background scripts
- Cache aggressively

## Design for Dark Mode

In 2026, dark mode isn't optional. Test your extension in both light and dark themes.

## Ship Fast, Iterate Faster

Get something working and ship it. Real user feedback is worth more than weeks of planning.

My first version of MarkX was embarrassingly simple. But it worked, people used it, and their feedback shaped what it became.

## Resources

- [Chrome Extension Docs](https://developer.chrome.com/docs/extensions/)
- [Manifest V3 Migration Guide](https://developer.chrome.com/docs/extensions/mv3/intro/)

What extensions are you building? Let me know on [Twitter](https://twitter.com/quangpl99).
