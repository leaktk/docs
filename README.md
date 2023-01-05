# LeakTK Docs

User and contributor docs for the LeakTK project.

(Things are still rather WIP here, there's a lot of work to open source still
and only so much time to do it \^_\^).

## Contents

* [Architecture](ARCHITECTURE.md) - The LeakTK architecture and vision.
* [Contributing](CONTRIBUTING.md) - How to contribute to the docs.
* [Glossary](GLOSSARY.md) - Terms used throughout this project.
* [Guides](guides) - User, contributor, and admin guides.
* [Ideas](ideas) - A place to capture ideas for the project

## Why This Project Exists

Individual secrets leaks can be very expensive to a company or damage its
brand. Bad actors can detect and abuse these secrets minutes after
they are exposed, and it is much easier to commit a secret than it is to remove
it. Also the number of secret leaks have been on the rise according to
GitGuardian.

LeakTK is an effort to open source lessons learned from an internal leak
detection tool called PwnedAlert and several companion tools. Most of the
existing tools are written in Python, but we decided to write most of this
project in Rust to make it [blazingly fast](https://www.youtube.com/watch?v=Sp5_d6coiqU)
and to make the components easier to distribute.

We have found that automatically alerting repo-owners directly saves IR analyst
time and effort, and we have caught and dealt with leaks minutes after data was
made public. Part of dealing with those leaks is not only detection (there are
a lot of tools for this) but also mitigation, and prevention. Being able to
tell a full story from leak to resolution is key to reducing the amount of time
the leak is public, and the way to reduce the time the most is to prevent leaks
in the first place.

The internal scanner supports HIBP, GitHub, and GitLab. There is also a
pre-commit hook and a pattern server. This project aims to eventually replace
the internal tools and add additional sources like Jira, Bugzilla, web pages,
and more! We are also looking into a browser plugin and into opportunities to
integrate it with other pipeline and analysis tools.

So in short: This project aims to reduce the number of leaks and help lessen
the pain if one still manages to happen.
