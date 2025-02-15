<h2 align="center">
<img align="center" width="70" height="70" src="./assets/logo.png"><br/>
<br/>
Awesome Dev News
</h2>

This is source repository for `awesome-dev.news` site - created using `Liveboat` page generator.

If you'd like to host your own, custom version of this page see [Liveboat Github Runner](https://github.com/exaroth/liveboat-github-runner) for Github Pages hosting or [Liveboat](https://github.com/exaroth/liveboat) repo for everything else.


## Contributing

### Adding feed links

The site is created using `Liveboat` static site generator which aims to be compatible with `Newsboat` RSS reader, for shorthand overview of the syntax see [Liveboat URL File Breakdown](https://github.com/exaroth/liveboat-github-runner?tab=readme-ov-file#liveboat-url-file-breakdown) or [Newsboat Documentation](https://newsboat.org/releases/2.10.2/docs/newsboat.html) for full overview.

In order to add additional feeds to the page:

1. Fork the repository
2. Edit `./config/urls` file
3. Add feed reference in following format

```
<feed_url> "~<Feed title>" ! <tag_list...>
```

for example:

```
https://blog.rust-lang.org/feed "~Rust Blog" ! dev official rust
```

> [!NOTE]
> 1. Please add `!` within the record to only include record links as part of existing query feeds
> 2. Include human readable title via `"~<feed title>"` 
> 3. Try to limit number of tags to 3 if possible
> 4. Do not include any additional query feeds as part of PR

Additionally:

- Include only active feeds which release news at least few times a year
- Do not include feeds containing promotional materials about company products
- Feel free to add feeds for categories not included on the site yet, make sure to tag these accordingly
 
### Bugs and Feature requests

Bugs/feature requests should be submitted to [Liveboat issues](https://github.com/exaroth/liveboat/issues) page.

## Acknowledgments

- Vectors and icons by <a href="https://goodstuffnononsense.com/hand-drawn-icons/space-icons/?ref=svgrepo.com" target="_blank">Good Stuff No Nonsense</a> in CC Attribution License via <a href="https://www.svgrepo.com/" target="_blank">SVG Repo</a>





