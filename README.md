# My Portfolio

One Paragraph of project description goes here

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites


```
Github,Heroku account, Node, npm 
```

### Installing

A step by step series of examples that tell you have to get a development env running

Steps will be:

```
Install Express Generator - In Terminal npm install express-generator -g
Express Generator

Run express --view=ejs --css=sass --git heroku-express
Command reads as follows: Run express generator with ejs engine/view support. Sass as the css engine. Add a .gitignore file. Producing all of this in a folder called heroku-express.
```

Run local server to verify -> DEBUG=heroku-express:* npm start
Open the package.json file and add "dev": "NODE_ENV=dev nodemon ./bin/www" right below the start direction. The end result of your file should look like this:

```
{
  "name": "heroku-express",
  "version": "0.0.0",
  "private": true,
  "scripts": {
    "start": "node ./bin/www",
    "dev": "NODE_ENV=dev nodemon ./bin/www"
  },
  "dependencies": {
    "body-parser": "~1.15.2",
    "cookie-parser": "~1.4.3",
    "debug": "~2.2.0",
    "dotenv": "^4.0.0",
    "ejs": "~2.5.2",
    "express": "~4.14.0",
    "morgan": "~1.7.0",
    "node-sass-middleware": "0.9.8",
    "serve-favicon": "~2.3.0"
  }
}
Via Terminal: Run npm run dev. Now you should be running nodemon with the environmet variable NODE_ENV equal to dev
```

End with an example of getting some data out of the system or using it for a little demo


## Deployment

[Heroku](https://signup.heroku.com)

## Built With

* [Express](http://expressjs.com/) - The web framework used
* [Node.js](https://nodejs.org/en/) - Package management
* [Bootstrap](http://getbootstrap.com/) - Theme styling

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. 

## Authors

* **Alex Diaz** - *Initial work* - [Portfolio](https://github.com/alexdiaz94/myPortfolio)


## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone who's code was used
* Inspiration
* etc
