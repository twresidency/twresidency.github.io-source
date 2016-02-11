# artist-residency-source

This is the source code for the [Artist Residency]() website. The site is built using [Hexo](https://hexo.io/).

## How to get started

```
  $ git clone --recursive https://github.com/twresidency/twresidency.github.io-source.git
  $ cd twresidency.github.io-source
  $ npm install
```

Run the server, to check it out locally!
```
  $ hexo serve
```

## Deploy

This hexo site is configured to deploy the static site to Github, at [this github repository](https://github.com/twresidency/twresidency.github.io). You must have push privelages to this repo to deploy. To deploy, do the following:

```
  $ hexo deploy
```

Checkout the live site [here](https://twresidency.github.io)!

## Theme

Most of the styling of a Hexo site exists in the `themes` folder. This is a nice separation of data from styling, which allows you to swap themes pretty effortlessly. 

### Add a theme

Themes in a Hexo site are [git submodules](), which are basically git repos inside of a git repo. If there is a Hexo theme already in a remote repo, then all you have to do is:

```
	$ git submodule add [git repo url] themes/[name of theme]
```

If you want to create a new theme, then you must make a seperate theme project. [Check the hexo docs](https://hexo.io/docs/themes.html) for more info on how to make a theme. After you do push it up to GitHub. Then to add the theme just use the command line command above with the `git clone` url for your new theme on Github.

### Work on a theme

Often it's easiest to work on a custom theme when you are working within a Hexo site. Because of git submodules, this is possible! You can edit, add, do whatever in your theme and see what your site looks like as you make changes. Once you are ready to commit the changes and push. `cd` into the root of the theme, which would look like this if you were at the root of your site:

```
	$ cd themes/[name of theme]
``` 

Now, if you do `git status` you will only see changes to do with the theme because you're in the inner theme repo that is a submodule of your hexo site.You can:

```
	$ git add
	$ git commit -m "the changes I made in my theme are earth shattering"
```

 If you have privelages to push this repo:

```
 	$ git push
```

