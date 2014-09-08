hexo-multilanguage-example
==========================

This is an example using HEXO (http://hexo.io) to generate a static multilanguage site

Notice: It is just a demo and work in progress...


IMPORTANT NOTICE
----------------

Until my pull requests are merged to the official HEXO repo, you have to use
my HEXO fork, with the branch `multilanguage`

```
git clone https://github.com/jkuetemeier/hexo.git
cd hexo
git checkout multilanguage
npm install
```
and now make it your global hexo

```
npm link
```

You can restore the official version later on with
```
npm install hexo -g
```

How to install and use this example repository
=============================================

### Install HEXO

~~Install [HEXO](http://hexo.io), for more informations see [docs](http://hexo.io/docs/).~~

TODAY: Use my hexo version, see notice above.

```
# NO - npm install hexo -g
```

### Clone repo

Clone it to your local folder (or fork it, if you intend to create expansions - pull requests are welcome).

```
git clone https://github.com/jkuetemeier/hexo-multilanguage-example.git example
```

### Install requirements

install site requirements

```
cd example
npm install
```

Now clone the theme into the directory `landscape`

```
cd themes
git clone https://github.com/jkuetemeier/hexo-theme-landscape.git landscape
```

checkout the Branch `multilanguage`

```
cd landscape
git checkout multilanguage
```

and install dependencies

```
npm install

# get back to repo root directory
cd ../../
```

### run the server

start your server

```
hexo server
```

Now you can direct your favorite browser to `http://localhost:4000`

Enjoy!

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

For this demo we use the [HEXO Landscape Theme](https://github.com/hexojs/hexo-theme-landscape). Now, until development is finished and a pull request ist committed, we use a modified `multilanguage` branch of this [fork](https://github.com/jkuetemeier/hexo-theme-landscape/tree/multilanguage).

You need to install [Grunt](http://gruntjs.com) as a requirement, if you not alread have it. See [Getting startet](http://gruntjs.com/getting-started) for more informations on Grunt.

```
npm install -g grunt-cli
```

Now clone the theme into the directory `landscape`

```
cd themes
git clone https://github.com/jkuetemeier/hexo-theme-landscape.git landscape
```

checkout the Branch `multilanguage`

```
cd landscape
git checkout multilanguage
```

install the theme dependencies

```
npm install
grunt
```

### Install Multilanguage Plugin

Install the [HEXO Multilanguage Plugin](https://github.com/jkuetemeier/hexo-plugin-multilanguage)

Use the GitHub version until development is finished and npm version is released:

```
npm install jkuetemeier/hexo-plugin-multilanguage --save
```



