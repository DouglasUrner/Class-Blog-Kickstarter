# Class Blog Design Notes

## Overview

* Meteor 1.3 (original built around beta.5)

* MongoDB

* React

  With [BlazeToReact][O.1] as glue.

* [React Router][0.2]

Because it allows nested routes and the code is more concise.

* Bootstrap UI Framework (in the form of [react-bootstrap][O.3])

```sh
meteor add twbs:bootstrap
meteor add ian:accounts-ui-bootstrap-3
npm install --save react-bootstrap
```

[O.1]: https://atmospherejs.com/thereactivestack/blazetoreact
[O.2]: https://github.com/rackt/react-router
[O.3]: https://react-bootstrap.github.io


## User Accounts & Authentication

Google configuration at: [Google Developers Console][UAA.1] as the Class Blog project.

Setup based on the [Adding user accounts][UAA.2] section of the Meteor
[Todo App with React][UAA.3] and a simplified (Google only) version of the
[Roll Your Own Authentication][UAA.3] recipe from The Meteor Chef.

Workflow:

Packages:
* [accounts-ui][UAA.6]
* [accounts-google][UAA.7]

### Roles

[Using the Roles Package][UAA.6]

**admin**

**teacher**

**student**

**mentor** (parent or other interested party, able to browse the blog with the same view as their student(s), but with no rights to create new content – not sure if they should be allowed to comment or not)


[UAA.1]: https://console.developers.google.com
[UAA.2]: https://www.meteor.com/tutorials/react/adding-user-accounts
[UAA.3]: https://www.meteor.com/tutorials/react/creating-an-app
[UAA.4]: https://themeteorchef.com/recipes/roll-your-own-authentication
[UAA.6]: https://themeteorchef.com/snippets/using-the-roles-package/
