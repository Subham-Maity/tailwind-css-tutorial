

<Callout type="info" emoji="💡">
  <div >
    <h5 className="text-left h-10 text-gray-400 font-extrabold md:text-1xl mt-0 mb-0" > Click here if you would like to modify or contribute </h5>
    <a href="https://github.com/Subham-Maity/tailwind-css-tutorial" target="_blank">
      <img align="left"
           alt="GitHub"
           src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white"
      />
      <p align="left">
        <img src="https://media1.giphy.com/media/2HCaWITqHdJmmEA2b7/giphy.webp?cid=ecf05e47oblnld6xqs4q4svq3w8lnpcltavzi667j872uwq7&rid=giphy.webp&ct=s"  width="50"/>
      </p>
    </a>
  </div>
</Callout>

# Introduction

## Message from the Developer


<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,borderRadius: "20px" ,overflow: "hidden" }  }>
  <div align="center">
    <div style={{ border: '1px solid #888', padding: '0rem 1rem', textAlign: 'center' }}>
      <h2 align="left">Author</h2>
      <p align="center">
        <img style={{ border:"solid #888" ,opacity: 1 ,borderRadius: "20px" ,overflow: "hidden" }  } src="https://media4.giphy.com/media/Hicydpti7wG3vA8Zr4/giphy.gif?cid=ecf05e47pq44hry9re27thxnjcezuifd6b0gzyvbxpfy4ua3&rid=giphy.gif&ct=g"/>
      </p>
      _Hey I'm your XAM(subham). In this tutorial you will learn how to create a basic website using tailwind css. I hope you will enjoy this tutorial. If you have any doubt or suggestion please feel free to contact me. I will be happy to help you. Thank you for your support. Have a nice day!_
      — Xam
      <h7 align="center">
        **Are you exited to learn about the Tailwind CSS?**
        I promise you, you'll get a million dollar course free of charge and a complete step-by-step guide in the course . So, what are you waiting for?
      </h7>
    </div>
  </div></div>


- Why should we use tailwind css in our project?
<details>
  <summary>Answer</summary>
  Tailwind CSS makes it quicker to write and maintain the code of your application.One of the reasons Tailwind CSS is so much better than Bootstrap is that it doesn't impose difficult-to-reverse design decisions since apps and sites are made up of pre-designed widgets. With Tailwind CSS, you just need a set of utility classes, so you can work with exactly what you want.
</details>

- What Exactly is Tailwind CSS?


<details>
  <summary>Answer</summary>
  It's a low-level CSS framework that lets you create custom-built designs without having to override opinionated component styles. It's really easy to create beautiful custom user interfaces with CSS without having to spend much time coding. The utility-first design of Tailwind CSS allows you to style every component specifically, the way you want. Adapting the "form follow function", the name of the utility class predicts its exact function to make it easier to design. Using Tailwind, you can customize and extend the most critical CSS properties.
</details>


- Advantages of Using Tailwind CSS


<details>
  <summary>Answer</summary>
  1. **It is Highly Customizable:** Tailwind CSS is a highly customizable framework. Although it comes with a default configuration, it is simple to override it with a tailwind.config.js file. The configuration file enables easy customization of color palettes, styling, spacing, themes, etc. Tailwind combines the perfect utilities that facilitate easy management of projects and derive maximum CSAT.

  2. **It Has Common Utility Patterns:** Eliminate the hassle of naming classes with Tailwind CSS. The availability of common utility patterns solves numerous problems like specifying classes, organizing them, cascading them, and much more. Utility classes simplify the process of creating custom components. You do not need to hard-code with Tailwind CSS. You can apply the theme() function to extract values from the configuration files.

  3. **It Can Be Optimized Using PurgeCSS:** A major advantage of Tailwind CSS is that optimization can be performed using PurgeCSS. PurgeCSS can reduce the file size considerably by scanning the HTML and removing unused classes. It is easy to set up PurgeCSS in combination with Tailwind CSS and is highly recommended to do so before deploying the site. As the size of the project grows, the size of the CSS file also increases. However, this does not happen when using Tailwind. The use of a standardized set of classes keeps the file size small as long as the project remains active.

  4. **It Enables Building Complex Responsive Layouts Freely:** The Tailwind CSS framework uses a default mobile-first approach. The availability of utility classes makes it easier to build complex responsive layouts freely. Utility classes can be used across a variety of breakpoints conditionally which helps in building complex responsive layouts hassle-free.

  5. **It Facilitates Fluid Community Interaction:** Stuck with an unsolvable issue? The Tailwind CSS community can be the perfect solution. Become a part of this community and get comprehensive assistance from fellow users as and when required. Find answers to all your CSS-related queries on-the-go and create exceptional applications/websites without any hurdle. The Tailwind CSS team offers quick solutions for the speedy resolution of issues.
</details>

## Setting up Tailwind CSS

<h4 className="text-center font-extrabold md:text-2xl mt-8">Installation</h4>



Install Tailwind CSS

First of all, we will install some important programs which will be required throughout our Tailwind Journey-

- **Install VS code:** You can download VS code from [here](https://code.visualstudio.com/download).
- **Install Live Server:** You can download Live Server from [here](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer). This will help us to run our project on a local server.
- **Adding Tailwind CSS:** To add tailwind CSS to your file, simply visit the official documentation of tailwind CSS [here](https://tailwindcss.com/docs/installation). You can also use the CDN link to add tailwind CSS to your project. You can find the CDN link [here](https://tailwindcss.com/docs/installation/play-cdn).

<Callout>
      <p>
        <strong>Note:</strong> You can also use it for React, Vue, Angular, Svelte, etc. You can find the documentation for all of them [here](https://tailwindcss.com/docs/installation).
      </p>
</Callout>

After that, From the play CDN section, just copy the script and add it to the `<head>` of your HTML file. Hence, we can now use Tailwind CSS in our HTML file.

- **Install Node Js:** You can download Node Js from [here](https://nodejs.org/en/download/).Select your OS and click on next, and your Nodejs will be installed. This will help us to install tailwind CSS in our project.
- **Installing ‘Tailwind CSS IntelliSense’ extension:** This extension provides some advanced features such as autocomplete, syntax highlighting, and linting. You can download it from [here](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss).


<h4 className="text-center font-extrabold md:text-2xl mt-8">Setting</h4>

`index.html`
 There have been several questions about some settings of VS Code t, so I'll walk you through them briefly. My index.html file looks like this:

- add this `script` tag in the `<head>` of your HTML file and inside the `<body>` tag and inside this ``h1`` tag add `class = "text-3xl...."` like this

```html filename="index.html" {6,9-11}
  <!doctype html>
  <html>
  <head>
    <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <script src="https://cdn.tailwindcss.com"></script>
  </head>
  <body>
  <h1 class="text-3xl font-bold underline text-purple-700 text-opacity-75">
    Hello World!
  </h1>
  </body>
  </html>
```


- Preview of the above code:

<h1 className="text-center text-3xl font-bold underline text-purple-700 text-opacity-75">
  Hello World!
</h1>

`settings.json`


## Experiment

Let's try to make a simple nav bar using tailwind CSS



```html filename="index.html" {9,10,11,17}
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <script src="https://cdn.tailwindcss.com"></script>
  </head>
  <body>
    <nav class="px-4 py-4 bg-[#1e293b] text-white">
      <ul class="flex">
        <li class="mx-2 cursor-pointer">Home</li>
        <li class="mx-2 cursor-pointer">About</li>
        <li class="mx-2 cursor-pointer">Contact</li>
      </ul>
    </nav>
    <div class="container">
      <h1 class="text-blue-900 my-12">CodeXam</h1>
    </div>
  </body>
</html>
```
- Preview of the above code:
<nav class="px-4 py-4 bg-[#1e293b] text-white">
  <ul class="flex">
    <li class="mx-2 cursor-pointer">Home</li>
    <li class="mx-2 cursor-pointer">About</li>
    <li class="mx-2 cursor-pointer">Contact</li>
  </ul>
</nav>
    <div class="container">
  <h1 class="text-blue-900 my-12">CodeXam</h1>
</div>

### Explain line by line

Check the highlighted lines `(9,10,11,17)` in the code above. Let's see what they do.
#### Padding,Margins,Background-color,Text-color
- `px-4` means padding in x-axis is 4. `py-4` means padding in y-axis is 4. `bg-[#1e293b]` means background color is #1e293b. `text-white` means text color is white.
#### Flex
- `flex` means display is flex - The flex property sets the flexible length on flexible items. Note: If the element is not a flexible item, the flex property has no effect. Details [here](https://tailwindcss.com/docs/flex).
#### Margin and Cursor
- `mx-2` means margin in x-axis is 2 between the elements. `cursor-pointer` means cursor is pointer when we hover over the element - The cursor property sets the type of mouse cursor, if any, to show when the mouse pointer is over an element. Details [here](https://tailwindcss.com/docs/cursor).
#### Container
- `text-blue-900` means text color is blue-900. `my-12` means margin in y-axis is 12. `container` means the width of the container is 100% of the screen.


### Problems
If you open the browser and go to the console, you will see some errors. like this

<Callout>
  cdn.tailwindcss.com should not be used in production. To use Tailwind CSS in production, install it as a PostCSS plugin or use the Tailwind CLI: https://tailwindcss.com/docs/installation
  (anonymous) @ (index):62
</Callout>

basically, it is saying that we should not use the CDN link in production. So, we will install tailwind CSS in our project.

### Install Tailwind CSS in our project

follow the steps below to install tailwind CSS in our project.

You can check the official documentation [here](https://tailwindcss.com/docs/installation/using-postcss).

- Install Node Js from [here](https://nodejs.org/en/download/).
- Open your project folder in VS Code.
- Installing Tailwind CSS - For Production

We want to use Tailwind CSS in the production of our application, therefore we would install the Tailwind with the help of Post CSS, Vite, and Autoprefixer. To install Tailwind for production, we need to install the following packages:
```bash {1} filename="terminal"
npm install -D tailwindcss postcss autoprefixer
```

### Installing Vite - For Development

Vite is a build tool that aims to provide a faster and leaner development experience for modern web projects. To install Vite, we need to install the following packages:
```bash {1} filename="terminal"
npm install vite
```

<Callout type= 'info' emoji='😊'>
If you want to use vite in your project you have to add this line in your `package.json` file.
</Callout>

- `package.json` file

open `package.json` file add highlighted line in the code below.



```json filename="package.json" {2-4}
{
"scripts": {
  "start": "vite"
},

  "devDependencies": {
    "autoprefixer": "^10.4.13",
    "postcss": "^8.4.18",
    "tailwindcss": "^3.2.2"
  },
  "dependencies": {
    "vite": "^3.2.3"
  }
}
```

It's simply saying that when we run `npm start` it will run `vite` command. You can check the official documentation [here](https://vitejs.dev/guide/#scaffolding-your-first-vite-project).


### Initialising Tailwind CSS
Finally, for the initialization of the Tailwind, you have to use the below command-line:
```bash {1} filename="terminal"
npx tailwindcss init
```
After the execution of the above command, a Tailwind.config.js file will be created. Make sure to add a “*” in the content section as we will be using the Tailwind in the complete content.

- `tailwind.config.js` file

```js filename="tailwind.config.js" {3}
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["*"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```
<Callout type= 'info' emoji='??'>
  Using tailwind ‘Tailwind CSS IntelliSense’ extension in VS Code will help you to write tailwind classes. You can check the official documentation [here](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss).
</Callout>

### Start Vite
Now, we can start Vite by using the below command-line:
```bash {1} filename="terminal"
npm start
```

## All Files For This Tutorial
You can download all the files from github [here](https://github.com/Subham-Maity/tailwind-css-tutorial/tree/main/Chapter%201)
