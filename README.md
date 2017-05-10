##### Beta - Please keep in mind that this application is under heavy development

# Rasa UI

Rasa UI is a web application built on top of, and for, Rasa NLU. Rasa UI provides a web application to quickly and easily be able to create agents, define intents and entities. It also provides some convenience features for Rasa NLU, like training your models, monitoring usage or viewing logs. Our goal is to replace API.ai with Rasa, so many a lot of the terminology and usage are similar in concept.

## Features

- Training data stored in DB
- UI for managing training data
- Initiate training from training data from UI
- Review Rasa configuration and component pipelines
- Log requests for usage tracking, history, improvements
- Usage dashboard
- Easily execute intent parsing using different models

![Screenshot1](https://github.com/paschmann/rasaui/blob/master/resources/rasa_ui_1.png)

## Getting Started

Rasa UI can run directly on your Rasa NLU instance, or on a separate machine.


### Prerequisites

[PostgreSQL](https://www.postgresql.org/) - Used for storing training data (entities, intents, synonyms, etc.)

[Postgrest](https://postgrest.com) - Provides a RESTful API for PostgreSQL db

[Node.js/npm](https://nodejs.org/en/) - Serves Rasa UI and acts as a middleware server for logging (to the PostgreSQL DB)


### Installing

Please ensure prerequisites are fulfilled

Clone/download the Rasa UI repository

```
git clone https://github.com/paschmann/rasaui.git
```

Update your package.json file to include the IP Addresses of your postgrest and rasa servers.
Update your app.js file to include the IP Addresses of your local middleware server and postgrest server

## Running

Run npm start from the server folder

```
npm start
```

Your web application should be available on http://localhost:5001

## Contributing

Please read [contributing.md](https://github.com/paschmann/rasaui/contributing.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Authors

* **Paul Aschmann**

See also the list of [contributors](https://github.com/paschmann/rasaui/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [license.md](license.md) file for details