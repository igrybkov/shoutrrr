<p align="center">
<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END -->
    <a href="https://github.com/containrrr/shoutrrr">
        <img src="https://raw.githubusercontent.com/containrrr/shoutrrr/gh-pages/shoutrrr.jpg" width="450" /></a>
</p>
<h1 align="center">
    Shoutrrr
</h1>
<p align="center">
    Notification library for gophers and their furry friends.
    Heavily inspired by <a href="https://github.com/caronc/apprise">caronc/apprise</a>.
</p>
<p align="center">
    <img src="https://github.com/containrrr/shoutrrr/workflows/Main%20Workflow/badge.svg" />
    <a href="https://app.codacy.com/app/containrrr/shoutrrr?utm_source=github.com&utm_medium=referral&utm_content=containrrr/shoutrrr&utm_campaign=Badge_Grade_Dashboard"><img
      alt="codacy coverage"
      src="https://img.shields.io/codacy/coverage/30ce077eecde418ca328f4f7868f70c8.svg?style=flat-square"
    /></a>
    <a href="https://app.codacy.com/app/containrrr/shoutrrr?utm_source=github.com&utm_medium=referral&utm_content=containrrr/shoutrrr&utm_campaign=Badge_Grade_Dashboard"><img
 alt="codacy grade" src="https://img.shields.io/codacy/grade/30ce077eecde418ca328f4f7868f70c8/master.svg?style=flat-square" /></a>
    <a href="https://github.com/containrrr/shoutrrr"><img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/containrrr/shoutrrr.svg?style=flat-square" /></a>
    <a href="https://github.com/containrrr/shoutrrr/blob/master/LICENSE"><img alt="license" src="https://img.shields.io/github/license/containrrr/shoutrrr.svg?style=flat-square" /></a>
    <a href="https://godoc.org/github.com/containrrr/shoutrrr"><img           src="https://godoc.org/github.com/containrrr/shoutrrr?status.svg" alt="GoDoc" /></a>
</p>

## Quick Start

### As a package

Using shoutrrr is easy! There is currently two ways of using it as a package.

#### Using the direct send command

```go
  url := "slack://token-a/token-b/token-c"
  err := shoutrrr.Send(url, "Hello world (or slack channel) !")

```

#### Using a sender
```go
  url := "slack://token-a/token-b/token-c"
  sender := shoutrrr.CreateSender(url)
  sender.Send("Hello world (or slack channel) !", map[string]string { /* ... */ })
```

### Through the CLI

Start by running the `build.sh` script.
You may then run send notifications using the shoutrrr executable:

```shell
$ shoutrrr send [OPTIONS] <URL> <Message [...]>
```

## Documentation
For additional details, visit the [full documentation](https://containrrr.github.io/shoutrrr). 

## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://github.com/amirschnell"><img src="https://avatars3.githubusercontent.com/u/9380508?v=4" width="100px;" alt=""/><br /><sub><b>Amir Schnell</b></sub></a><br /><a href="https://github.com/containrrr/shoutrrr/commits?author=amirschnell" title="Code">💻</a></td>
    <td align="center"><a href="https://piksel.se"><img src="https://avatars2.githubusercontent.com/u/807383?v=4" width="100px;" alt=""/><br /><sub><b>nils måsén</b></sub></a><br /><a href="https://github.com/containrrr/shoutrrr/commits?author=piksel" title="Code">💻</a> <a href="https://github.com/containrrr/shoutrrr/commits?author=piksel" title="Documentation">📖</a> <a href="#maintenance-piksel" title="Maintenance">🚧</a></td>
  </tr>
</table>

<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!