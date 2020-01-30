# Mentor

Here is a list of guidelines you should follow during a workshop or a lecture.

## Display

The closer your own setup is to the [standard student's one](setup/ubuntu.md),
the better. That way you can share with them keyboard shortcuts. We use VS Code

When you are video-projecting your screen, please follow these guidelines:

- The only app running on your computer should be Finder, Vs Code, Terminal and Browser
- Have your text editor and terminal with a **light background**. You can install the [Solarized](http://ethanschoonover.com/solarized) theme, with the [VS Code package](https://marketplace.visualstudio.com/items?itemName=ryanolsonx.solarized) and the [OSX terminal theme](https://github.com/tomislav/osx-terminal.app-colors-solarized)
- Zoom a lot your font size (`⌘=`) in Vs Code and your terminal.
- If you don't have a lot of files, hide the folder drawer on the left with `⌘K, ⌘B`.
- Switch from one file to the other with the `⌘P` (Command Palette)
- You should use two windows layouts:
  - Vs Code in full screen
  - Vertical split (50/50) with Vs Code on the right, Terminal on the left

![Split Layout](img/split_layout.png)

## Tools

### Gist

After a long session of live-coding, usually students ask for the code. They like to keep it on their computer, for future's reference. A quick way to share some code files is to use [Github's gist service](http://gist.github.com/). A quicker way than copy/pasting manually every file is to install the [gist](https://www.npmjs.com/package/gist-cli) gem on your computer:

```bash
$ npm i -g gist-cli
```

Then, in an exercise folder, you can run:

```bash
$ gist -p *.js
```

This will automatically create a private gist with **all the JavaScript files** in the current folder. The program will give you the gist private URL that you can then share on Slack.

## Reviewing content

Whenever a student submits an exercise you should give early feedback. When you don't have enough time, please say something like: `Received! I will take a look at it ASAP`. 

If you are overloaded with work, please ask the rest of the students to review the other students pull requests.

Reviews should be professional and objective. 

Once the student has finished the expected assignment, ask for a bit more of information with questions like. 

- How would you improve your solution?
- What are the next steps after this?
- Have you ever considered doing it in another way? How?

This method serves for encouraging critical thinking.

