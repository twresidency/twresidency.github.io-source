# artist-residency-source

This is the source code for the [Artist Residency]() website. The site is built using [Hexo](https://hexo.io/).

## How to get started

Make a folder to house the source code locally, and initialize hexo:
```
  $ mkdir artist-residency-source
  $ cd artist-residency-source
  $ hexo init
```
Set origin remote repository to this github repo and pull:

```
	$ git remote set-url origin https://github.com/anirudh-eka/artist-residency-source.git
	$ git pull
```

Install dependancies:

```
  $ npm install
```

Run the server, to check it out locally!
```
  $ hexo serve
```

## Deploy

This hexo site is configured to deploy the static site to Github, at [this github repository](https://github.com/anirudhstuff/anirudhstuff.github.io/tree/master). You must have push privelages to this repo to deploy. To deploy, do the following:

```
  $ hexo deploy
```

Checkout the live site [here](http://anirudhstuff.github.io/)!