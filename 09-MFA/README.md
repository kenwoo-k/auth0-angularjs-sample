# MFA

This example shows how to add ***MultiFactor Authentication*** to your `Auth0` authentication flow. To enable MFA in your Auth0 account, go to the [Multifactor Authentication section](https://manage.auth0.com/#/guardian) of the management area and enable either Push Notifications or SMS. There is no need of extra code configuration.

You can read a quickstart for this sample [here](https://auth0.com/docs/quickstart/spa/angularjs/09-mfa). 

## Getting Started

To run this quickstart you can fork and clone this repo.

Be sure to set the correct values for your Auth0 application in the `auth0.variables.js` file.

To run the application

```bash
# Install the dependencies
bower install

# Get the plugins
ionic state restore --plugins

# Run
ionic serve
```


## Important Snippets

### 1. Login

```js
// components/login/login.controller.js
(function () {

  ...

  function LoginController(authService) {

    var vm = this;
    vm.authService = authService;

  }

}());
```