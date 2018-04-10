Classless for Hugo
==================

This Hugo theme features the basic [Classless](https://classless.alhur.es/) templates for your posts and list of posts. One of the [themes supported on Classless](https://classless.alhur.es/themes) may be chosen from your site's `config.toml`, along with the hash of the commit which you want to reference. That is needed because the provider, https://rawgit.com/, needs that to serve cached, cdnized versions of the themes hosted on https://github.com/fiatjaf/classless/tree/master/themes/.

Supported parameters on `config.toml`:

```toml
[params]
theme = "the theme name, choose from https://classless.alhur.es/themes"
commit_sha = "if in doubt, go to https://github.com/fiatjaf/classless and copy the 7 characters from the line that says: 'Latest commit xxxxxxx'"
description = "a description of your site, will be used on `body > header` and on the <meta> description, when not overriden by pages (in normal posts, it is overriden by the post summary)."
show_summaries = false // if you don't want automatic summaries in list pages
```

Partials that should be overwritten:

  * `layouts/partials/aside.html`: the HTML content of the `body > partial` Classless element.
  * `layouts/partials/footer.html`: the HTML content of the `body > partial` Classless element.

All posts (under `content/posts/`) support the following extra parameters:

```yaml
cover: a URL to an image to be used on the `article > header` and on list pages
hide_date: if you want to hide the date
tags:
  - an
  - array
  - of-tags
```
