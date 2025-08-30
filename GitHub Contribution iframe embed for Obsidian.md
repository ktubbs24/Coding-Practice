# GitHub Contribution iframe embed for Obsidian

<iframe src="https://jandee.vercel.app/ktubbs24" width="100%" height="300" frameborder="0"></iframe>

Yes, you can embed your GitHub contribution graph in an Obsidian note (including daily ones) using raw HTML for an iframe pointed to a third-party renderer that displays it dynamically.

Here’s how:

1. Find the URL for your contribution graph renderer. For example, using the Jandee service: https://jandee.vercel.app/your-github-username (replace your-github-username with your actual username).
2. In your Obsidian note, switch to source mode and add the following HTML:  
```
<iframe src="https://jandee.vercel.app/your-github-username" width="100%" height="300" frameborder="0"></iframe>
```
3.  Switch back to preview mode, and the graph should appear embedded in the note. Adjust the width and height attributes as needed for better display.

This keeps the graph up-to-date since it pulls from GitHub data. If the service goes down or you prefer a static option, you can generate an image using a tool like the GitHub Contributions Chart Generator at https://github-contributions.vercel.app, download the PNG, save it in your vault, and embed it with Markdown: `![GitHub Graph](path/to/image.png).`

Note: Obsidian supports iframes in preview mode, but they may not work in reading view on all devices or if there are security restrictions in your setup. 