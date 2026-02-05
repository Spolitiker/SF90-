# SF90 Robot Control

This repository contains the code for controlling the SF90 robot via a simple web interface.

## How to use

- Open the website: https://spolitiker.github.io/SF90-/
- Click the **ENGINE START** button to turn the robot on.
- Click the **ENGINE STOP** button to turn the robot off.

## How to update the webpage

- Edit the `index.html` file with your changes.
- Push changes to the GitHub repository.
- The page will update automatically on GitHub Pages.

## Notes

- Make sure your ESP device IP is correctly set in the fetch request inside `index.html` (currently commented out).
- This page uses simple JavaScript and CSS for UI control.
