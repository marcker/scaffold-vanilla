scaffold-vanilla
========

A scaffold for websites for those using vanilla JavaScript -- static and PHP based (WordPress).

## Goals

- [x] HTML 5
- [x] Stylus (CSS 3)
- [x] Gulp
- [x] Grid: [jeet](http://jeet.gs)
- [x] [Axis](http://axis.netlify.com/)
- [x] Media queries: [rupture](http://jenius.github.io/rupture/)
- [x] Compile `.styl`
- [x] Minify `.js`, `.css`, `.html`, `.php` (html, php: `[pagename]-dev.html` or `[pagename]-dev.php` to `[pagename].html` or `[pagename.php]`)
- [x] Optimize images (it is saved in `images/public`)
- [x] Live reload
- [ ] JavaScript documentation
- [x] Lint `.coffee`
- [x] **Optional** deploy with ShellScript (you should to configure your `ssh` access to not having to enter the password every deploy -- *this does not provide here*)
- [ ] WordPress theme scaffold
- [ ] Tests

## Install

```
git clone https://github.com/marcker/scaffold-vanilla
mv scaffold YourProjectName
cd YourProjectName
rm -rfv .git
git init # optional
```

*You should to uncomment the extensions that you want in the `.gitignore`*

### Static

For static websites.

```
cd static
npm install && npm install jeet
gulp
```

#### Deploy

```
cd deploy
```

Add to file **config**: `../path/to/files/or/files`, `user@ip`, `/path/to/files/on/the/target` (whitespace and comma separated). After:

```
chmod +x deployit.sh
./deployit.shz
```

### Wordpress

* Coming soon


### Related

* [Scaffold using CoffeeScript](https://github.com/marcker/scaffold)
