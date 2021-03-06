## Repository Outdated Packages

**Repository Outdated Packages** is an open-source **package version compare and notifier tool** based on [Nestjs](https://nestjs.com/) framework.
Subscribe to get email every day about the package updates (Currently only supported for Javascript/Typescript and PHP applications).

## Online Demonstration

- https://outdated-packages-marketing.herokuapp.com/

## Screenshots

![Image of Yaktocat](https://github.com/erbilsilik/outdated-packages/blob/master/intro.png)

![Image of Yaktocat](https://github.com/erbilsilik/outdated-packages/blob/master/subscribe.png)

![Image of Yaktocat](https://github.com/erbilsilik/outdated-packages/blob/master/outdated-packages.png)

## 🚀&nbsp; Installation and Running

`` npm install && npm run start ``

#### Docker

`` docker build -t outdated-packages .``

`` docker run -p 8080:8080 outdated-packages ``

CURL 

```
curl --request POST \
  --url https://outdated-packages.herokuapp.com/api/v1/repo-subscriptions \
  --header 'content-type: application/json' \
  --data '{
	"url": "https://github.com/axios/axios", 
	"emails": ["your.email@yme.com", "your.email2@me.com"]
}'
```

## Configurations

.env file

```
NODE_ENV=
PORT=

REDIS_HOST=
REDIS_PASSWORD=
REDIS_PORT=

GITHUB_OAUTH_TOKEN=

SENDGRID_API_KEY=
SENDGRID_EMAIL=
SENDGRID_PASSWORD=
```


## 🤝&nbsp; Found a bug? Missing a specific feature? Want to support?

- Currently we only support Javascript/Typescript and PHP. You are welcome to support for other languages
- Tests are missing
- 3rd party Semver module integration for more accuracy

Feel free to **file a new issue** with a respective title and description. If you already found a solution to your problem, **we would love to review your pull request**!
