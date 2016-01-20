# craft-boilerplate
A starting point for using CraftCMS with SASS Grunt tasks.

## Getting Started
To create a new Craft project based on this repo, create your new repo. Let's call it Feast.

In Feast, add this boilerplate repo as a remote,
```
git remote add boilerplate https://dust.git.beanstalkapp.com/craft-boilerplate.git
```
pull in the contents,
```
git pull boilerplate master
```
and then make sure you can't push up to the boilerplate, as that may well break everything.
```
git remote set-url --push boilerplate no_push
```

### Setting Up
Feast is built with <a href="//craftcms.com/">Craft</a>, but the Craft source files are not included with this repo. That would be ridiculous.

So to get it working:
* clone the repo,
* download the <a href="http://craftcms.com/latest.zip?accept_license=yes">latest Craft build</a>,
* copy the contents of public/,
* copy craft/app/,
* copy craft/plugins and craft/storage,
* copy the example craft/config/db.php, and put in your db settings.

We compile all our assets using Grunt. So first run ```npm i``` to install the node modules, ```bower update``` to install the bower components, and then ```grunt build``` to generate all the assets.

## Plugins we use in this project
We don't include plugin files in the repo. That would also be ridiculous. So here is a list of the plugins used:
