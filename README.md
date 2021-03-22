# Wizeline QA Certification

Assessment session 2, backend testing with Postman / Newman

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

* [Node, NPM](https://nodejs.org/en/) - Javascriptruntime and package manager
* [Postman](https://www.postman.com) - The Collaboration Platform for API Development
* [Newman](https://github.com/postmanlabs/newman) - CLI to run postman collections
* [Html reporter](https://github.com/postmanlabs/newman-reporter-html) - HTML Reporter for newman

### Installing

With node and npm installed just run in the root project folder

```
npm install
```

If you didn't installed newman globally, you will need to configure it to the project manually.

## Running the test

Teste are divided on fixtures:

- To run:

```
newman run Todoist_Api.postman_collection.json -e Todoist_Api.postman_environment.json -r html
```


[^Reports]: One report under newman/* will be generated each time the run command is executed

### Considerations

- **Task id**: Tests which requiered a task id should be modified with a real id, otherwise will fail.
- **Negative Cases**: Negative scenarios has been limited to authorization and empty or non existent documents.

### Config

Modify environment file **`Todoist_Api.postman_environment`** with your api token

### TODO:

- Add file to run multiple test (task creation on api).

## Authors

* **Gerardo Alvarez Muñoz** - *Not updated* - [Github](https://github.com/gerhardx)

## Acknowledgments

* Assesment for session 2 of Wizeline Academy 
* [Wizeline Academy](https://academy.wizeline.com)
