# MIAE Student Website Contributing Guide

So you'd like to contribute to our website? Below are some guidelines for contributers to follow. Any help with documentation, design ideas, or bug reports is greatly appreciated!

> [!WARNING]
> If you are not a McGill student or not part of the MIAE, please only contribute by opening an issue or a PR.

## Issues

If you've found a bug, would like to suggest an idea, or have something you want us to look at, please open an [issue](https://github.com/miae-sec/miae-sec.github.io/issues) with the description. If the issue is suitably described one of the members of the team will get back to you.

## Events

If you'd like to contribute an event description to add to our website, please follow these steps:

1. Follow git best practices to open a new branch off `dev`:
    1. `git checkout dev`
    2. `git pull`
    3. `git checkout -b yyyy-event-name`
2. Ensure you can build the current website, as described in the README
3. Create a new file in the `_events` directory, named `yyyy-mm-dd-name-of-event.md` where the date is the date of the event
4. Write the properties of the file:
```markdown
---
title: _title of event_
tags: 
 -  _type of event_
 cover: _path to cover image, use `/assets/events/`_
 media:
  - _bulleted list of other images to include
---
_Description of the event. If you're unfamiliar with markdown, see [this](https://www.markdownguide.org/) guide._
```

5. After running the website you should see this event show in the events tab
6. Commit your changes
    1. `git add .`
    2. `git commit -m 'description of the changes`
    3. `git push`
7. Open a [PR](https://docs.github.com/en/pull-requests/how-tos/create-pull-requests/creating-a-pull-request) and tag one of the members of the organization as a reviewer.
8. Once approved, merge your PR and see your event on the MIAE website!

## People

If you'd like to add yourself or a member to the team, please follow these steps:

1. Follow git best practices to open a new branch off `dev`:
    1. `git checkout dev`
    2. `git pull`
    3. `git checkout -b yyyy-event-name`
2. Ensure you can build the current website, as described in the README
3. Edit the `team.yml` file in `_data` with the following:
```yaml
- name: Your name
    role: Your role on the team
    bio: >
        a description of your role
```
4. Add a headshot to `/assets/team` named `firstname-lastname.jpg`
5. Commit your changes
    1. `git add .`
    2. `git commit -m 'description of the changes`
    3. `git push`
6. Open a [PR](https://docs.github.com/en/pull-requests/how-tos/create-pull-requests/creating-a-pull-request) and tag one of the members of the organization as a reviewer.
7. Once approved, merge your PR and see your event on the MIAE website!
. 
