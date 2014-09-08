hexo-multilanguage-example
==========================

This is an example using HEXO (http://hexo.io) to generate a static multilanguage site



How was this example created?
=============================

This describes the steps needed to get a full functional multilanguage site up and running, if you're not just cloning this repository. It gives an overview of the necessary steps for creating a site - it's not an accurate, full detailed description of any single step this repository is made of.

### Install Hexo

Install [HEXO](http://hexo.io), for more informations see [docs](http://hexo.io/docs/).

```
npm install hexo -g
```

create a folder `my-site` and step into it

```
mkdir my-site
hexo init
```

install required node packages

```
npm install
```

### Install Theme

For this demo we use the [HEXO Landscape Theme](https://github.com/hexojs/hexo-theme-landscape). Now, until development is finished and a pull request ist commited, we use a modifed `multilanguage` branch of this [fork](https://github.com/jkuetemeier/hexo-theme-landscape/tree/multilanguage).

You need to install [Grunt](http://gruntjs.com) as a requirement, if you not alread have it. See [Getting startet](http://gruntjs.com/getting-started) for more informations on Grunt.

```
npm install -g grunt-cli
```

Now clone the theme into the directory `landscape`

```
cd themes
git clone https://github.com/jkuetemeier/hexo-theme-landscape.git landscape
```

and checkout the Branch `multilanguage`

```
cd landscape
git checkout multilanguage
```

and install the theme dependencies

```
npm install
grunt
```
