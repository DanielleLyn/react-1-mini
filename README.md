<img src="https://devmounta.in/img/logowhiteblue.png" width="250" align="right">

# Project Summary

In this project, we'll introduce you to React by creating a small project from scratch. We'll make use of the `create-react-app` CLI tool to quickly generate a React boilerplate. The goal of this project is to create a simple interface for creating a list of friends with their name and picture.

## Setup

* Fork and clone this repository.
* Run `sudo npm install -g create-react-app`.

## Step 1

### Summary

In this step, we'll use `create-react-app` to create a React boilerplate.

### Instructions

* `cd` into the root directory of the project.
* Run `create-react-app ./`.
* Delete the `README.md` the boilerplate generates and rename `README.old.md` back to `README.md`.

### Solution

<img src="https://github.com/DevMountain/react-1-mini/blob/solution/readme-assets/1g.gif" />

## Step 2

### Summary

In this step, we'll clear the boilerplate that is made for us in `src/App.js`.

### Instructions

* Open `src/App.js`.
* Inside of the `return()` statement, replace everything with a single `<div>` element.

### Solution

<details>

<summary> <code> src/App.js </code> </summary>

```js
import React, { Component } from 'react';
import logo from './logo.svg';
import './App.css';

class App extends Component {
  render() {
    return (
      <div>

      </div>
    );
  }
}

export default App;
```

</details>

## Step 3

### Summary

In this step, we'll add the necessary elements inside the `<div>` element for capturing user input.

### Instructions

* Open `src/App.js`.
* Inside of the `<div>` element add two inputs with lables and an `Add Friend` button:
  * The first input should be for getting a URL to a picture.
  * The second input should be for getting a name.
* Run `npm start` to spin up a development server and see your changes.

### Solution

<details>

<summary> <code> src/App.js </code> </summary>

```js
import React, { Component } from 'react';
import logo from './logo.svg';
import './App.css';

class App extends Component {
  render() {
    return (
      <div>
        <span>Picture:</span>
        <input />

        <span>Name:</span>
        <input />

        <button>Add Friend</button>
      </div>
    );
  }
}

export default App;
```

</details>

<br />

<img src="https://github.com/DevMountain/react-1-mini/blob/solution/readme-assets/1.png" />

## Step 4

### Summary

In this step, we'll add a `state` to our `src/App.js` for managing a list of friends and also the values for creating a new friend. We'll also create a few methods of our own for updating state. One will be called `updatePicture`, this method is responsible for updating the value of `picture` on `state`. Another will be called `updateName`, this method is responsible for updating the value of `name` on `state.` And the last will be called `addFriend`, this method is responsbile for adding a new friend to the `friends` array on `state` and clearing the values for `picture` and `name` on `state`.

### Instructions

* Open `src/App.js`.
* Above the `render` method, add a new method called `constructor`.
* Inside the `constructor` method, invoke `super`.
  * This allows us to set state.
* Create a new state object, by using `this.state = {}`, with the following keys:
  * `friends` - An empty array.
  * `picture` - An empty string.
  * `name` - An empty string.
* Underneath the `constructor` method, create a new method called `updatePicture`:
  * This method should have a `value` parameter.
  * This method should update `picture` on `state` by using `this.setState()`.
* Underneath the `updatePicture` method, create a new method called `updateName`:
  * This method should have a `value` parameter.
  * This method should update `name` on `state` by using `this.setState()`.
* Underneath the `updateName` method, create a new method called `addFriend`:
  * This method doesn't need any parameters.
  * This method should use `this.setState()` to push a new friend object into the `friends` array on `state` and clear the values of `picture` and `name` on `state`.
    * A friend object should have a `picture` and `name` key.
      * { picture: "http://via.placeholder.com/50x50", name: "James Lemire" }

### Solution

<details>

<summary> <code> src/App.js </code> </summary>

```js

```

</details>

## Contributions

If you see a problem or a typo, please fork, make the necessary changes, and create a pull request so we can review your changes and merge them into the master repo and branch.

## Copyright

© DevMountain LLC, 2017. Unauthorized use and/or duplication of this material without express and written permission from DevMountain, LLC is strictly prohibited. Excerpts and links may be used, provided that full and clear credit is given to DevMountain with appropriate and specific direction to the original content.

<p align="center">
<img src="https://devmounta.in/img/logowhiteblue.png" width="250">
</p>

