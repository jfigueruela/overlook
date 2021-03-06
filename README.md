# Overlook

This is a demo node.js application illustrating various features used in everyday web development, with a fine touch of best practices. The demo app is a blog application where users (signing up using facebook, twitter, github and simple registrations) can create an article, delete an article and add comments on the article.

## Boilerplate

Want to build something from scratch? use the [boilerplate app](https://github.com/madhums/node-express-mongoose)

* Checkout the [apps that are built using this approach](https://github.com/madhums/node-express-mongoose/wiki/Apps-built-using-this-approach)
* The [wiki](https://github.com/madhums/node-express-mongoose/wiki) is wip, it has some information about the way application is setup.

## Requirements

* [NodeJs](http://nodejs.org)
* [mongodb](http://mongodb.org)
* [imagemagick](http://www.imagemagick.org/script/index.php)
* [bower](https://www.npmjs.org/package/bower)

## Install

```sh
$ git clone git@github.com:jfigueruela/overlook.git
$ npm install
$ bower install
```

**NOTE:** Do not forget to set the facebook, twitter, google, linkedin and github `CLIENT_ID`s and `SECRET`s. In `development` env, you can simply copy
`config/env/env.example.json` to `config/env/env.json` and just replace the
values there. In production, it is not safe to keep the ids and secrets in
a file, so you need to set it up via commandline. If you are using heroku
checkout how environment variables are set [here](https://devcenter.heroku.com/articles/config-vars).

If you want to use image uploads, don't forget to set env variables for the
imager config.

```sh
$ export IMAGER_S3_KEY=AWS_S3_KEY
$ export IMAGER_S3_SECRET=AWS_S3_SECRET
$ export IMAGER_S3_BUCKET=AWS_S3_BUCKET
```

then

```sh
$ npm start
```

(Note: When you do npm start, `NODE_PATH` variable is set from package.json start script. If you are doing `node server.js`, you need to make sure to set this)

Then visit [http://localhost:3000/](http://localhost:3000/)

## Tests

```sh
$ npm test
```

## License

MIT

## Acknowledgements
Thanks to Madhusudhan Srinivasa https://github.com/madhums for inspiring this project with his efford in https://github.com/madhums/node-express-mongoose-demo

***
[![reqtangular](https://github.com/codebusters/generator-reqtangular/blob/master/resources/img/reqtangular_banner_250x50.png)](http://reqtangular.blogspot.com.es/)

[![facebook](https://github.com/codebusters/generator-reqtangular/blob/master/resources/img/FB_FindUsOnFacebook-100.png)](https://www.facebook.com/reqtangular)
[![twitter](https://github.com/codebusters/generator-reqtangular/blob/master/resources/img/bird_blue_32.png)](https://twitter.com/reqtangular)
<a href="http://reqtangular.blogspot.com.es/"><img src="http://img1.blogblog.com/html/buttons/blogger-simple-kahki.gif" alt="Powered By Blogger"></a>
