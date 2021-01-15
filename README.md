# :grey_question: What tools will we be using?

## React Library

Allows us to organize and re-use our HTML/CSS/JS code.
Used as the front-end library to create the UI/UX of the app

## Node.js / NPM

Install Node.js so that we can get NPM. NPM is used to install external libraries that will be used alongside React.

## Sass

Makes writing CSS easier. Allows us to have "seperate" styling files rather than one huge CSS file (since a website can only use one CSS file).

## Visual Studio Code

-   Text Editor that we are using
-   Get Prettier (formats your code automatically on save) and ESLint (warns us of typos/poor syntax, etc) as plug ins in Visual Studio Code's extensions.

## External Sources

#### [Project plan](https://docs.google.com/document/d/1B4sCE6ka5pTpU2ZDcajNfk9QfNZMcp0dlmIoBAeKcYU/edit):

#### [Documentation For Our Project](https://docs.google.com/document/u/1/d/1lDMahp42n3qlfQCE8brnBVs0vz0HfR5qx7rG0rnUvfw/edit?usp=drive_web&ouid=109247223246109231260):

#### [Clout Coins](https://docs.google.com/document/d/186TNrjQzXsv8thZ4XKPoLi6DU8bzkOPcFlzfbZFGl-8/edit)

# How do we use these tools?

## Starting out with React:

[Following what the documentation says]
(https://reactjs.org/docs/create-a-new-react-app.html)

You can create your own project by opening up your terminal / command prompt (make sure your path listed on terminal is where you want to create the project) and typing

`npx create-react-app YOUR-APP-NAME`
`cd YOUR-APP-NAME`
`npm start`

Where YOUR-APP-NAME can be any name you want to name your project.

It looks like:
<img src="readmeImg/createReactAppCommand.png" height="350"/>

Where do we get `npm start`? If you open up your new project and go to package.json it will say `npm start` in `scripts`; package.json holds all the commands you can run in your terminal. In our case, we only have to worry about `npm start`.

## Starting out with Node.js / NPM:

Super simple way to install other libraries we want to include in our React project. For example, if we want to have loading spinners in our website but we don't want to create it, we can install the library from :

https://www.npmjs.com/package/react-spinners

It looks like this:
<img src="readmeImg/npmDemo.png" height="350"/>

So how do we do it?

1. Go to the location of our project where our package.json holds

<img src="readmeImg/packageLocation.png" height="350"/>

Here, my package.json is in
`C:\projects\kijiji\server\client` (copy the address bar)

2. Then go to terminal and go to the location of the address:
   In Windows I could do `cd C:\projects\kijiji\server\client`

<img src="readmeImg/terminalPackageLocation.png" height="350"/>

3. Type `npm i react-spinners` (to get the command, look at the right side of the image).

:exclamation: However, we want to do
`npm i react-spinners --save` or `npm i react-spinners --save-dev`

By doing `npm i react-spinners --save`, the library name would appear in our package.json's dependancies. This informs others and ourselves what libraries are included in the project.
As shown here:
<img src="readmeImg/dependancies.png" height="350"/>

``--save-dev` should be used if we installed a library that's specifically for developers (90% of the time you won't be using this)

## Starting out with Sass:

Once you have npm installed, it's time to install node-sass. You can do so by running npm install -g node-sass in your terminal to install the package globally (i.e. available across your entire system)

There will be `scss folders` in the project that looks like:
<img src="readmeImg/scssFolder.png" height="350"/>

You will be making your styling changes there.

To run SCSS, on your terminal, go to the folder where the SCSS folder is located and simply run
`sass --watch scss:css`

As shown here:
<img src="readmeImg/scssCompiling.png" height="350"/>

If for some reason the sytlings are not applied, exit with Ctrl + C and start Sass again; sometimes it bugs out.

## Starting out with Visual Studio Code:

-   Make sure to get Prettier and ESLint as extensions. There are turtorials online on how to do so. Very self explanatory on their purposes, will make your life 100x easier.
