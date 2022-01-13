# Combining the power of open-source projects and communities

## The need

Suppose you are automating a web-based process.

The target system is a modern [single-page application](https://en.wikipedia.org/wiki/Single-page_application) built with [React](https://reactjs.org/).

Modern web apps are dynamic. The views change on the fly. The HTML markup that defines the structure of those views is ever-mutating. Things happen immediately, almost immediately, after a while, and sometimes in no particular order ([asynchronously](<https://en.wikipedia.org/wiki/Asynchrony_(computer_programming)>)).

You need an automation tool capable of handling all that dynamic behavior.

## The solution - Part I

Let's see. [Playwright](https://playwright.dev/) seems promising. An open-source tool for browser automation that uses the multitude of open-source JavaScript projects out there to build something powerful.

> "Playwright enables reliable end-to-end testing for modern web apps." - https://playwright.dev/

Playwright itself started as a [fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/about-forks) of another open-source automation tool - [Puppeteer](https://developers.google.com/web/tools/puppeteer).

The Playwright community seems active. All the source code is available at their [repository](https://github.com/microsoft/playwright). The [issues](https://github.com/microsoft/playwright/issues) are open for all to participate.

Open-source contributions can come in as feature requests, bug reports, solutions or workarounds for tricky cases, documentation, examples, helping others on the forums, chats, and discussion groups, improvements to existing code, or even entirely new features in the form of pull requests.

One needs to know JavaScript quite well to work with Playwright effectively.

Maybe there's a more high-level solution for writing the automation that does not require JavaScript knowledge? Something slightly more human-readable than JavaScript code?

## The solution - Part II

Another open-source project, [Robot Framework](https://robotframework.org/), seems promising:

> "Robot Framework is a generic open source automation framework. Robot Framework has an easy syntax, utilizing human-readable keywords." - https://robotframework.org/

Human-readable syntax sounds excellent. Again, there seems to be an active community contributing to the project.

But Robot Framework seems to be written in [Python](https://www.python.org/), an open-source programming language. Surely it can not work with Playwright since that is JavaScript-based?

[Robot Framework Browser](https://robotframework-browser.org/). What's this?

> "powered by Playwright"

Great! Now you can leverage the power of a modern web automation tool and use human-readable syntax.

The installation instructions seem to indicate you need quite a bunch of stuff to run all this.

Maybe there's another solution that enables the use of Playwright, Robot Framework, and Robot Framework Browser and makes installing all that easy and consistent everywhere (you are planning to develop the automation with a team of three people - keeping the environments in sync on everyone's machine is important).

## The solution - Part III

Yet another open-source project, [rcc](https://github.com/robocorp/rcc), seems to do the trick of making things more convenient:

> "RCC is a set of tooling that allows you to create, manage, and distribute Python-based self-contained automation packages. RCC is a foundation that allows anyone to build and share automation with ease." - https://github.com/robocorp/rcc

There's even a template for creating a Playwright-based project, utilizing the Robot Framework Browser library and the human-readable syntax of Robot Framework!

Now you still need a good tool for authoring the automation. The tool should support at least code auto-completion, syntax validation, formatting, running the automation...

## The solution - Part IV

[Robocorp](https://robocorp.com/) suggests the use of [VS Code](https://code.visualstudio.com/), an open-source integrated development environment (IDE) plus [a couple of open-source extensions for building automations](https://marketplace.visualstudio.com/search?term=robocorp&target=VSCode&category=All%20categories&sortBy=Relevance).

## Together, we can accomplish great things

So many great open-source projects, so many communities working for the benefit of all, so many possibilities for combining the pieces to build something new. Standing on the shoulders of others.

This feels powerful. This feels _right_. **This is the way.**
