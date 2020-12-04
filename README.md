# Issara Institute - ReactJS assignment

Here we provide the instructions for developing ReactJS application, designed by the Issara Institute team, to test the proficiency of applicants for the ReactJS Frontend Developer position

## Prerequisites
* Knowledge of ReactJS, HTML, CSS, UI libraries (Ant Design and/or Bootstrap)
* Knowledge of installing npm packages (both local & global)
* Knowledge of creating React application using [Create React App](https://facebook.github.io/create-react-app/)
* Knowledge of fetching JSON data from a REST API endpoint
* A Github account in order to share his/her code with us

## Submission guidelines

### Sharing the code

All applicants must share their code in one of the following ways:

 - Upload their code on their Github account by creating a public repository and sharing the link via email.
 - Creating a zip file of their project folder (excluding the node_modules directory) and either uploading it to a cloud service (sharing the link with us) or attaching it to an email (if size < 20 MB).

### Deploying the code for testing

All applicants are also required to deploy their assignment to a server or to any of the static hosting service providers ([link to help with deployment](https://facebook.github.io/create-react-app/docs/deployment)).

## Assignment Details

This assignment is a frontend React applications with no backend development required.

The idea is to build a single page that displays the profiles of service providers (the data is obtained from an API endpoint). Each service provider's profile should contain a `logo, company name, email, website, rating score and rating count`.

#### API endpoint for service providers

All service providers profiles data is to be fetched from the following API endpoint:
```
Method: GET
URL: https://server-dot-ilm-client-dev.appspot.com/api/v1/service-providers?lang={{language_code}}
```

The `{{language_code}}` in the URL is the placeholder for the language code. It should be dynamically replaced by the language code selected in a language selector component (you should create one). For example, if selected language code is `en` then the URL would look like this:

https://server-dot-ilm-client-dev.appspot.com/api/v1/service-providers?lang=en

The schema of the data received in the response is:
```Javascript
// Array of service providers
[
  {
    id,	// profile id
    email,
    website,
    name, // company name
    comments_count,
    rating_score,
    rating_count,
    ...
  }
]
```

#### API endpoint for languages

All supported languages are to be fetched from the following API endpoint:
```
Method: GET
URL: https://server-dot-ilm-client-dev.appspot.com/api/v1/localization/languages
```

The schema of the data received in the response is:
```Javascript
// Array of languages
[
  {
    id,
    code, // language code
    name, // language name
    flag, // flag image
    updated_at
  }
]
```


## Assignment

**Deadline for submission:** 5 days

This assignment is designed for applicants who have learned ReactJS and have minimal hands-on experience in developing react application.

Extended demo of how it might look like - https://client-dot-ilm-client-dev.appspot.com/services

**Notes:**
- this is extended demo, for this assignment you don't need to add filters, search and any other extra information that wasn't mentioned earlier such us address, category, etc

- language selector is missing in the demo (you need to create one)

- feel free to come up with your own layout (number of service providers displayed per row) and styling (background, color, size, etc)

### What are we looking for?

With this assignment we would evaluate the following:

 - Ability to create new react projects using [Create React App](https://facebook.github.io/create-react-app/)
 - Understanding of JSX
 - Passing props to components
 - Understanding of stateful and stateless Components
 - Basic understanding of state management and component lifecycle methods
 - Fetching data from an API endpoint
 - Conditional rendering
 - Working with lists
 - Ability of the applicant to learn a new React UI library and use its components in their app

### Instructions
This app should be a responsive (mobile, tablet and desktop) and will be tested on Chrome browser.

The entire app must be designed using the [Ant Design](https://ant.design/) or [React Boostrap](https://react-bootstrap.github.io/) library.

## General Tips

 - Feel free to use Google, StackOverflow or any other resource
 - Open the data API link in your browser and examine the response schema
 - Please feel free to get in touch with the Issara Institute's team to clear any doubts related to the aforementioned instructions.
