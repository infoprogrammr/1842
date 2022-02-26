# House Targareact

A simple ongoing project in order to prepare the Game of Thrones characters for winter and to allow me to practise my new React knowledge. This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Goals

To build my first React project without a tutorial.

## Features

There are characters and an arsenal.

![screen shot 2019-01-26 at 14 40 27](https://user-images.githubusercontent.com/42243785/51788663-7e48c080-2178-11e9-8693-a00c154a6ffe.png)

Users can give a character a weapon and it will disappear in the arsenal, arming the character.
If the user tries to give a character a weapon that is already taken, an error message will appear.

![screen shot 2019-01-26 at 14 40 49](https://user-images.githubusercontent.com/42243785/51788664-80ab1a80-2178-11e9-8c40-f3191637a421.png)

Users can click on a character and see their description.

![screen shot 2019-01-26 at 14 45 39](https://user-images.githubusercontent.com/42243785/51788713-22cb0280-2179-11e9-80bf-beb17306bead.png)


## Architecture

- There's one source of truth - the App component, which holds all the states.
- The App component renders the Character components, which, in turn, renders the Description components
- The App also renders the Arsenal components.

## To run

In the project directory, run:

### `npm start`

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

## Testing

- I didn't TDD this project, because I wanted to become familiar with React itself first.  
- Feature testing is done with Cypress, a technology I learnt after Makers. 
- Testing is ongoing: it is currently not unit tested, as I wanted to learn Jest to do so.

To run all the feature tests:

First, keep the server running. Then:
```
$ npx Cypress run
```

...will print out the tests in the terminal. Or:

```
$ npx Cypress open
```
and then click on each test, or on 'Run all Specs'. This will allow you to see the tests with images. 

## Future Improvements

- Perhaps change the Arsenal class to a Stateless Functional Component
- The weapon buttons should probably be a component, as there's a lot of repetition of them.
- Implement some sort of game
- Learn Jest and test it

