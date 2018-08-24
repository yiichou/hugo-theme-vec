# Vec

Vec is a minimal, clean and beautiful theme for [Hugo](http://gohugo.io/).

[Demo](http://yii.im).

![Vec screenshot](https://github.com/IvanChou/hugo-theme-vec/blob/master/images/tn.png)

![Vec screenshot2](https://github.com/IvanChou/hugo-theme-vec/blob/master/images/tn2.png)

## Installation

```
mkdir themes
cd themes
git clone https://github.com/IvanChou/hugo-theme-vec vec
```

See the [official docs](http://gohugo.io/themes/installing) for more information.

## Quickstart Guide

Make sure you have : 

1. 	Hugo installed
2. Test poject setup with hugo. Instructions on [hugo quickstart guide](https://gohugo.io/overview/quickstart/).
3. Cloned this repo in the themes folder.  

The [exampleSite](exampleSite) folder contains a sample site to quickly get started. 

Copy over the contents of ```config.toml``` and copy the [content](exampleSite/content) and [static](exampleSite/static) folders to your main folder. 

Build using ```hugo server --buildDrafts```  

To create a post use ```hugo new post/post-title.md``` 

## Configuration

You should config your site's `config.toml` file like:

```
baseurl = "https://www.example.com"
title = "Site.title"
theme = "vec"
languageCode = "en-us"
paginate = 15

# Enable comments by entering your Disqus shortname
disqusShortname = "Your Disqus shortname"

# Enable analytics by entering your Google Analytics tracking ID
googleAnalytics = "Your Google Analytics tracking code"

[params]
  Keywords = "key, 关键字, キーワード"
  Description = "There are some words to describe your site"
  
  Avatar = "img/avatar.jpg"
  SelfIntro = "Just a worm, seek for true, live in shadow, no more..." 
  Email = "you@example.com"
  
  GithubID = "Your Github ID"
  TwitterID = "Your Twitter ID"
  FacebookID = "Your Facebook ID"
  LinkedInID = "Your LinkedIn ID"
  GoogleplusID = "Your Googleplus ID"
```

If you use `config.yaml`, plz reformat them to yaml.

### Enable Disqus to your post

1. Add your Disqus Shortname to the site config file;
2. You can enable Disqus per-post, by adding `comments: true` (YAML) or `comments = true` (TOML) in the front matter of your post. To disable it, you can either change the value to `false` or just not include `comments` variable and its value at all. 

### Enable TOC to your post

If you need show table of contents per-post, adding `toc: true` (YAML) or `toc = true` (TOML) in the front matter of your post.

Please notice that TOC will be hidden when browser width is less than 920px.

### Enable Formspree to your page

If you need a form which allows guests to contact you by email, Formspree maybe a good choice.

Firstly, make sure you have already set a Email in the config.toml. And then add `formspree: true` (YAML) or `formspree = true` (TOML) in the front matter of your page.

## Build your site

Add `theme = "vec"` to your `config.toml`, then

```
# Build
hugo

# Run a server
hugo server
```
OR

```
hugo -t vec
hugo server -t vec
```


## Design By

Cedric Fung(@vecio)

## License

Open sourced under [MIT license](https://github.com/IvanChou/hugo-theme-vec/blob/master/LICENSE.md).

