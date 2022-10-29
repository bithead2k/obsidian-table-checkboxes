# Obsidian Tables Checkboxes
This plugin for [Obsidian](https://obsidian.md) replaces markdown checkboxes `-[]` inside markdown tables with HTML checkboxes.

## Example
https://user-images.githubusercontent.com/66573865/197360507-251c2586-c11c-412c-a368-7c275ff247a2.mp4



## How to use

- Simply enable the plugin and type a markdown checkbox inside a table. It will get converted to a HTML checkbox.
- In either live preview or view mode, (un)check the checkbox and the state will be reflected in your file.

## How it works

- Whenever a closing bracket `]` is typed, the plugin checks if it's a markdown checkbox `- []` inside of a markdown table `| - [ ] |`.
- It then changes the checkbox to HTML `<input type="checkbox" unchecked>`.
- When a HTML checkbox is clicked, the location of the table and then the cell gets identified. The plugin then changes the `unchecked` attribute to `checked`, or vice versa.

## Known issues
- Checkboxes in fully identical tables can cause issues.

Empty/duplicate cells should no longer cause issues.
