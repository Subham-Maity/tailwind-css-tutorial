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

# Basic Portfolio website using tailwind css

## Message from the Developer


 <div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,borderRadius: "35px" ,overflow: "hidden" }  }>
    <div align="center">
  <div style={{ border: '1px solid #888', padding: '0rem 1rem', textAlign: 'center' }}>
    <h2 class="pb-4" align="left">Author</h2>
    <div style={{ border:"none", position: "relative" ,opacity: 1 ,borderRadius: "45px" ,overflow: "hidden" }  }>
    <p align="center">
      <img src="https://user-images.githubusercontent.com/97989643/201677987-b089d002-66fb-4c4d-85ab-f666cd8d891a.png"/>
    </p>
    </div>
    _Hey I'm your XAM(subham). In this tutorial you will learn how to create a basic website using tailwind css. I hope you will enjoy this tutorial. If you have any doubt or suggestion please feel free to contact me. I will be happy to help you. Thank you for your support. Have a nice day!_
    — Xam
    <h7 align="center">
      **Are you exited to learn about the Tailwind CSS?**
      I promise you, you'll get a million dollar course free of charge and a complete step-by-step guide in the course . So, what are you waiting for?
    </h7>
  </div>
</div></div>




## Landing Page Setup
Landing page is the first page of your website. It is the first impression of your website. So, it is very important to make a good first impression. In this tutorial, we will create a landing page for our website. We will use tailwind css to create our landing page. So, let's get started.

<div style={{margin:"2%" }  } class="gradient-border" id="box"> </div>

## Setup our project
- We create a `experiment folder` in our local machine.
- We create a `index.html` file in our experiment folder.
- Open your `terminal` in vscode and type the following command.
```bash {1}
npm init
```
→ Then just press enter to all the questions.

<Callout type="info" emoji="💡">

If you want to skip all the questions then you can use the following command `npm init -y`

</Callout>

- Now fire up this command in your terminal.
```bash {1}
npm install -D tailwindcss postcss autoprefixer vite
```

- Then fire up this command in your terminal.
```bash {1}
npx tailwindcss init
```
- After the execution of the above command, a Tailwind.config.js file will be created. Make sure to add a `“*”` in the content section as we will be using the Tailwind in the complete content.

 `tailwind.config.js` file 👇

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

- For starting the development server, we will use vite. So,open `package.json` file add highlighted line in the code below.



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

<Callout type="info" emoji="💡">
  You might notice that here already have a `start` script. So, we will replace it with the above code.
</Callout>

- For starting the development server fire up this command in your terminal.
```bash {1}
npm run start
```
<Callout type="info" emoji="💡">
  you can notice in your terminal something like this  Local: http://127.0.0.1:5173/ . This is the url of your development server. You can open this url in your browser.
</Callout>

- If you have Tailwind CSS IntelliSense Extension in your vscode then you will get some suggestions. If you don't have this extension then you can install it from [here](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss). Whenever you point your cursor to the class name you will see what that class does.

-  In chapter one we have created a basic navbar inside `index.html` like this 👇

```html filename="index.html"{6}
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
you can notice that we use a CDN for tailwind css.


<div style={{margin:"2%" }  } class="gradient-border" id="box"> </div>


## Create a basic landing page


### Create a navbar
- Now make a `landing.html` file in your experiment folder.
- Add CDN link of tailwind css in your `landing.html` file like `index.html` file.
- When you follow the link `http://127.0.0.1:5173/ ` after firing up the command `npm run start` you have to change the url to `http://127.0.0.1:5173/landing.html` to see the `landing page.`
- Let me explain line by line (8,11,12)
```html filename="landing.html" {8,11,12}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://cdn.tailwindcss.com"></script>
    <title>Hey I'm a professional blockchain developer  </title>
</head>
<body>
    <nav class="px-4 py-4 bg-[#1e293b] text-white">
        <ul class="px-28 py-4 flex space-x-3 justify-end">
            <li>Home</li>
            <li>About</li>
            <li>Contact US</li>
            <li>Projects</li>
        </ul>
    </nav>

</body>
</html>
```

••••• Output of the above code 👇
<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%" }  }>
  <nav class="px-4 py-4 bg-[#1e293b] text-white">
    <ul class="px-28 py-4 flex space-x-3 justify-end">
      <li>Home</li>
      <li>About</li>
      <li>Contact US</li>
      <li>Projects</li>
    </ul>
  </nav>

</div>

Here we have created a basic navbar.
<img width="15%" height="2px" src="https://user-images.githubusercontent.com/97989643/201496986-b2def9d0-a6b2-46dc-94c3-ee0a7c39fd29.gif"></img>
→ We use title tag to give a title to our website. This title will be shown in the tab of our browser.

→ We use `px-4` class in the `nav` tag to give padding in the horizontal direction.(px means padding left and right)



••••• Output of the above code 👇
<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%" }  }>
  <nav class="px-4">
    <ul >
      <li>Home</li>
      <li>About</li>
      <li>Contact US</li>
      <li>Projects</li>
    </ul>
  </nav>
</div>




→ We use `py-4` class in the `nav` tag to give padding in the vertical direction.(py means padding top and bottom)

••••• Output of the above code 👇
<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%" }  }>
  <nav class="px-4 py-4 ">
    <ul>
      <li>Home</li>
      <li>About</li>
      <li>Contact US</li>
      <li>Projects</li>
    </ul>
  </nav>

</div>


→ We use `bg-[#1e293b]` class in the `nav` tag to give background color to our navbar.

••••• Output of the above code 👇
<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%" }  }>
  <nav class="px-4 py-4 bg-[#1e293b]  ">
    <ul>
      <li>Home</li>
      <li>About</li>
      <li>Contact US</li>
      <li>Projects</li>
    </ul>
  </nav>

</div>

→ We use `text-white` class in the `nav` tag to give text color to our navbar.

••••• Output of the above code 👇
<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%" }  }>
  <nav class="px-4 py-4 bg-[#1e293b] text-white">
    <ul>
      <li>Home</li>
      <li>About</li>
      <li>Contact US</li>
      <li>Projects</li>
    </ul>
  </nav>

</div>

→ We use `px-28` class in the `ul` tag to give padding in the horizontal direction.(px means padding left and right)

••••• Output of the above code 👇
<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%" }  }>
  <nav class="px-4 py-4 bg-[#1e293b] text-white">
    <ul class="px-28">
      <li>Home</li>
      <li>About</li>
      <li>Contact US</li>
      <li>Projects</li>
    </ul>
  </nav>

</div>
→ We use `py-4` class in the `ul` tag to give padding in the vertical direction.(py means padding top and bottom)

••••• Output of the above code 👇
<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%" }  }>
  <nav class="px-4 py-4 bg-[#1e293b] text-white">
    <ul class="px-28 py-4" >
      <li>Home</li>
      <li>About</li>
      <li>Contact US</li>
      <li>Projects</li>
    </ul>
  </nav>

</div>
→ We use `flex` class in the `ul` tag to make our list items in a row direction.flex means flexible box. `ul` is a list tag `li` is a list item tag.

••••• Output of the above code 👇
<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%" }  }>
  <nav class="px-4 py-4 bg-[#1e293b] text-white">
    <ul class="px-28 py-4 flex" >
      <li>Home</li>
      <li>About</li>
      <li>Contact US</li>
      <li>Projects</li>
    </ul>
  </nav>

</div>
→ We use `space-x-3` class in the `ul` tag to give space between the list items. space-x means space between the list items in the horizontal direction.

••••• Output of the above code 👇
<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%" }  }>
  <nav class="px-4 py-4 bg-[#1e293b] text-white">
    <ul class="px-28 py-4 flex space-x-3" >
      <li>Home</li>
      <li>About</li>
      <li>Contact US</li>
      <li>Projects</li>
    </ul>
  </nav>

</div>
→ We use `justify-end` class in the `ul` tag to justify the list items in the end of the row. (We use `px-28` class because we don't want the list items to the extreme right of the screen.)

••••• Output of the above code 👇
<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%" }  }>
  <nav class="px-4 py-4 bg-[#1e293b] text-white">
    <ul class="px-28 py-4 flex space-x-3 justify-end">
      <li>Home</li>
      <li>About</li>
      <li>Contact US</li>
      <li>Projects</li>
    </ul>
  </nav>

</div>



<div style={{margin:"2%" }  } class="gradient-border" id="box"> </div>


### Logo Setup

- I create a public folder and inside that folder I use a png image as a logo.(you can use image link also)
- Use image tag inside the nav tag to show the logo.
- For adjusting the logo size use some tailwind classes we will explain all the classes below.
```html filename="landing.html"{11,12}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://cdn.tailwindcss.com"></script>
    <title>Hey I'm a professional blockchain developer  </title>
</head>
<body>
    <nav class="bg-[#1e293b] text-white flex justify-between">
        <img src="./public/blue green.png" class="h-16 pt-3 pb-2 px-4 rounded-3xl border-blue-500"  alt="">
        <ul class="px-28 py-4 flex space-x-3 justify-end">
            <li class=" cursor-pointer">Home</li>
            <li class=" cursor-pointer">About</li>
            <li class=" cursor-pointer">Contact</li>
            <li class=" cursor-pointer">Projects</li>
        </ul>
    </nav>

</body>
</html>
```
••••• Output of the above code 👇
<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%" }  }>
  <nav class="bg-[#1e293b] text-white flex justify-between">
    <img src="https://github.com/Subham-Maity/tailwind-css-tutorial/blob/main/Chapter%202/Experimets/public/blue%20green.png?raw=true" class="h-16 pt-3 pb-2 px-4 rounded-3xl"  />
      <ul class="px-28 py-4 flex space-x-3 justify-end">
        <li class=" cursor-pointer">Home</li>
        <li class=" cursor-pointer">About</li>
        <li class=" cursor-pointer">Contact</li>
        <li class=" cursor-pointer">Projects</li>
      </ul>
  </nav>
</div>
<img width="15%" height="2px" src="https://user-images.githubusercontent.com/97989643/201496986-b2def9d0-a6b2-46dc-94c3-ee0a7c39fd29.gif"></img>
→ If we don't use `flex justify-between` class in the `nav` tag then the logo and the list items will be in a column direction.

••••• Output of the above code 👇

<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%" }  }>
  <nav class="bg-[#1e293b] text-white">
    <img src="https://github.com/Subham-Maity/tailwind-css-tutorial/blob/main/Chapter%202/Experimets/public/blue%20green.png?raw=true" class="h-16"/>
    <ul class="px-28 py-4 flex space-x-3 justify-end">
      <li>Home</li>
      <li>About</li>
      <li>Contact US</li>
      <li>Projects</li>
    </ul>
  </nav>
</div>

this means simply
```css
div {
display: flex;
justify-content: space-between;
}
```
<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%" }  }>
  <div class="flex justify-between">
    <div class="bg-red-500">CodeXam</div>
    <div class="bg-blue-500">CodeXam</div>
    <div class="bg-green-500">CodeXam</div>
  </div>
</div>



→ We use `h-16` class in the `img` tag to give height to our logo. h means height.

••••• Output of the above code 👇

<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%" }  }>
  <nav class="bg-[#1e293b] text-white flex justify-between">
    <img src="https://github.com/Subham-Maity/tailwind-css-tutorial/blob/main/Chapter%202/Experimets/public/blue%20green.png?raw=true" class="h-16"/>
    <ul class="px-28 py-4 flex space-x-3 justify-end">
      <li>Home</li>
      <li>About</li>
      <li>Contact US</li>
      <li>Projects</li>
    </ul>
  </nav>
</div>

→ We use `pt-3` class in the `img` tag to give padding in the top direction. pt means padding top.

••••• Output of the above code 👇

<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%" }  }>
  <nav class="bg-[#1e293b] text-white flex justify-between">
    <img src="https://github.com/Subham-Maity/tailwind-css-tutorial/blob/main/Chapter%202/Experimets/public/blue%20green.png?raw=true" class="h-16 pt-3"/>
    <ul class="px-28 py-4 flex space-x-3 justify-end">
      <li>Home</li>
      <li>About</li>
      <li>Contact US</li>
      <li>Projects</li>
    </ul>
  </nav>
</div>

→ We use `pb-2` class in the `img` tag to give padding in the bottom direction. pb means padding bottom.

••••• Output of the above code 👇


<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%" }  }>
  <nav class="bg-[#1e293b] text-white flex justify-between">
    <img src="https://github.com/Subham-Maity/tailwind-css-tutorial/blob/main/Chapter%202/Experimets/public/blue%20green.png?raw=true" class="h-16 pt-3 pb-2"/>
    <ul class="px-28 py-4 flex space-x-3 justify-end">
      <li>Home</li>
      <li>About</li>
      <li>Contact US</li>
      <li>Projects</li>
    </ul>
  </nav>
</div>

→ We use `px-4` class in the `img` tag to give padding in the left and right direction. px means padding left and right.

••••• Output of the above code 👇

<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%" }  }>
  <nav class="bg-[#1e293b] text-white flex justify-between">
    <img src="https://github.com/Subham-Maity/tailwind-css-tutorial/blob/main/Chapter%202/Experimets/public/blue%20green.png?raw=true" class="h-16 pt-3 pb-2 px-4"/>
    <ul class="px-28 py-4 flex space-x-3 justify-end">
      <li>Home</li>
      <li>About</li>
      <li>Contact US</li>
      <li>Projects</li>
    </ul>
  </nav>
</div>


→ We use `rounded-3xl` class in the `img` tag to give border radius to our logo. rounded means border radius.

••••• Output of the above code 👇

<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%" }  }>
  <nav class="bg-[#1e293b] text-white flex justify-between">
    <img src="https://github.com/Subham-Maity/tailwind-css-tutorial/blob/main/Chapter%202/Experimets/public/blue%20green.png?raw=true" class="h-16 pt-3 pb-2 px-4 rounded-3xl"  />
    <ul class="px-28 py-4 flex space-x-3 justify-end">
      <li>Home</li>
      <li>About</li>
      <li>Contact US</li>
      <li>Projects</li>
    </ul>
  </nav>
</div>

→ We use `cursor-pointer` class in li tag to give cursor pointer to our li tag. cursor means mouse pointer.

••••• Output of the above code 👇
<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%" }  }>
  <nav class="bg-[#1e293b] text-white flex justify-between">
    <img src="https://github.com/Subham-Maity/tailwind-css-tutorial/blob/main/Chapter%202/Experimets/public/blue%20green.png?raw=true" class="h-16 pt-3 pb-2 px-4 rounded-3xl"  />
    <ul class="px-28 py-4 flex space-x-3 justify-end">
      <li class=" cursor-pointer">Home</li>
      <li class=" cursor-pointer">About</li>
      <li class=" cursor-pointer">Contact</li>
      <li class=" cursor-pointer">Projects</li>
    </ul>
  </nav>
</div>





<Callout type="info">
  Note: A title can be added to the navbar instead of the logo. In order to add the title, you simply need to remove the image and add the title text inside the span tag. Additionally, margin, font bold, text colour, and many other properties can be used to enhance the text.
</Callout>


<div style={{margin:"2%" }  } class="gradient-border" id="box"> </div>

### Setting up the content section

#### Body

- Create a container: The content section is the main section of the page. It contains the main content of the page. We will create a container for the content section.
- Adding background colour: We will add a background colour to the content section.
- Add Heading/Paragraph: We will add a heading and a paragraph to the content section by creating another div container and assigning the heading and paragraph to it.
- Add a button: We will add a button to the content section. We will use the button component of tailwind css to add a button to the content section.
- Adding Padding: We will add padding to the content section. We will use the padding classes of tailwind css to add padding to the content section.

```html filename="index.html" {22-37}
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://cdn.tailwindcss.com"></script>
    <title>Hey I'm a professional blockchain developer </title>
</head>

<body>
    <nav class="bg-[#1e293b] text-white flex justify-between">
        <img src="./public/blue green.png" class="h-16 pt-3 pb-2 px-4 rounded-3xl" alt="">
        <ul class="px-28 py-4 flex space-x-3 justify-end">
            <li class=" cursor-pointer">Home</li>
            <li class=" cursor-pointer">About</li>
            <li class=" cursor-pointer">Contact</li>
            <li class=" cursor-pointer">Projects</li>
        </ul>
    </nav>
    <main>
        <div class="main bg-slate-400 py-40 pl-9">
            <div class="text-6xl"> I am a professional blockchain developer </div>
            <p class="py-3 w-1/3">Showcase your knowledge of blockchain, machine learning, OOPs, DSA, and all advanced
                coding skills you desire.</p>
            <div class="my-4">
                <button
                    class="bg-sky-700 px-3 py-2 rounded-3xl text-white hover:text-slate-900 hover:bg-blue-400 mx-2 hover:border-2 hover:border-white"><a
                        href="https://code-xam.vercel.app/" target="_blank">CodeXam Website </a></button>
                <button
                    class="bg-sky-700 px-3 py-2 rounded-3xl text-white hover:text-slate-900  hover:bg-blue-400 mx-2 hover:border-2 hover:border-white"><a
                        href="https://github.com/Subham-Maity/tailwind-css-tutorial" target="_blank">Contact
                        Us</a></button>
            </div>
        </div>
    </main>
</body>

</html>
```

••••• Output of the above code 👇

<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%"   }  }>
<nav class="bg-[#1e293b] text-white flex justify-between">
  <img src="https://github.com/Subham-Maity/tailwind-css-tutorial/blob/main/Chapter%202/Experimets/public/blue%20green.png?raw=true" class="h-16 pt-3 pb-2 px-4 rounded-3xl"  />
  <ul class="px-28 py-4 flex space-x-3 justify-end">
    <li class=" cursor-pointer">Home</li>
    <li class=" cursor-pointer">About</li>
    <li class=" cursor-pointer">Contact</li>
    <li class=" cursor-pointer">Projects</li>
  </ul>
</nav>

  <div class="main bg-slate-400 py-40 pl-9">
    <div class="text-6xl"> I am a professional blockchain developer </div>
    <p class="py-3 w-1/3">Showcase your knowledge of blockchain, machine learning, OOPs, DSA, and all advanced coding skills you desire.</p>
    <div class="my-4">
      <button
        class="bg-sky-700 px-3 py-2 rounded-3xl text-white hover:text-slate-900 hover:bg-blue-400 mx-2 hover:border-2 hover:border-white"><a
        href="https://code-xam.vercel.app/" target="_blank">CodeXam Website </a></button>
      <button
        class="bg-sky-700 px-3 py-2 rounded-3xl text-white hover:text-slate-900  hover:bg-blue-400 mx-2 hover:border-2 hover:border-white"><a
        href="https://github.com/Subham-Maity/tailwind-css-tutorial" target="_blank">Contact
        Us</a></button>
    </div>
  </div>

</div>

<img width="15%" height="2px" src="https://user-images.githubusercontent.com/97989643/201496986-b2def9d0-a6b2-46dc-94c3-ee0a7c39fd29.gif"></img>




→ We use ``<div class="main bg-slate-400 py-40 pl-9">``  to create a container for the content section. here main is the class name and `bg-slate-400` is the background colour of the content section.

→ We use ``py-40`` to add padding to the content section.

→ We use ``pl-9`` to add padding to the left side of the content section. Basically our paragraph will be aligned to the left side of the content section.
<Callout type="info">
  For color codes you can check this website <a href="https://tailwindcss.com/docs/customizing-colors"><strong>Tailwind CSS Color Codes</strong></a>
</Callout>
••••• Output of the above code 👇
<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%"   }  }>
<div class="main bg-slate-400 py-40 pl-9">

</div>

</div>

→ We use `text-6xl` inside the first div container to add a heading to the content section. Here `text-6xl` is the class name and `6xl` is the size of the heading.

••••• Output of the above code 👇
<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%"   }  }>
  <div class="main bg-slate-400 py-40 pl-9">
    <div class="text-6xl"> I am a professional blockchain developer </div>

  </div>

</div>

→ We use `py-3` inside the first div container to add padding to the heading.

→ We use `w-1/3` inside the first div container to set the width of the heading. Here `w-1/3` is the class name and `1/3` is the width of the heading. You can set the width of the heading from 1/12 to 12/12.


••••• Output of the above code 👇
<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%"   }  }>
  <div class="main bg-slate-400 py-40 pl-9">
    <div class="text-6xl"> I am a professional blockchain developer </div>
    <p class="py-3 w-1/3">Showcase your knowledge of blockchain, machine learning, OOPs, DSA, and all advanced
      coding skills you desire.</p>
  </div>

</div>

<div style={{margin:"2%" }  } class="gradient-border" id="box"> </div>

#### Button Make

→ We use `my-4` inside the first div container to add margin to the button. Here `my-4` is the class name and `4` is the margin of the button.

••••• Output of the above code 👇
<div class="my-4">
<button
class="bg-sky-700 px-3 py-2 rounded-3xl text-white hover:text-slate-900 hover:bg-blue-400 mx-2"><a
href="https://code-xam.vercel.app/" target="_blank">CodeXam Website </a></button>
<button
class="bg-sky-700 px-3 py-2 rounded-3xl text-white hover:text-slate-900  hover:bg-blue-400 mx-2"><a
href="https://github.com/Subham-Maity/tailwind-css-tutorial" target="_blank">Contact
Us</a></button>
</div>
→ We use bg-sky-700 inside the button tag to set the background colour of the button. Here `bg-sky-700` is the class name and `sky-700` is the background colour of the button.

••••• Output of the above code 👇
<div class="my-4">
  <button class="bg-sky-700" >Contact
    Us</button>
</div>
→ We use `px-3` inside the button tag to add padding to the button. Here `px-3` is the class name and `3` is the padding of the button.

••••• Output of the above code 👇
<div class="my-4">
  <button class="bg-sky-700 px-3" >Contact
    Us</button>
</div>
→ We use `py-2` inside the button tag to add padding to the button. Here `py-2` is the class name and `2` is the padding of the button.

••••• Output of the above code 👇
<div class="my-4">
  <button class="bg-sky-700 px-3 py-2" >Contact
    Us</button>
</div>
→ We use `rounded-3xl` inside the button tag to add border radius to the button. Here `rounded-3xl` is the class name and `3xl` is the border radius of the button.

••••• Output of the above code 👇
<div class="my-4">
  <button class="bg-sky-700 px-3 py-2 rounded-3xl" >Contact
    Us</button>
</div>
→ We use `text-white` inside the button tag to set the text colour of the button. Here `text-white` is the class name and `white` is the text colour of the button.

••••• Output of the above code 👇
<div class="my-4">
  <button class="bg-sky-700 px-3 py-2 rounded-3xl text-white" >Contact
    Us</button>
</div>
→ We use `hover:text-slate-900` inside the button tag to set the text colour of the button when we hover over it. Here `hover:text-slate-900` is the class name and `slate-900` is the text colour of the button when we hover over it.

••••• Output of the above code 👇
<div class="my-4">
  <button class="bg-sky-700 px-3 py-2 rounded-3xl text-white hover:text-slate-900" >Contact
    Us</button>
</div>
→ We use `hover:bg-blue-400` inside the button tag to set the background colour of the button when we hover over it. Here `hover:bg-blue-400` is the class name and `blue-400` is the background colour of the button when we hover over it.

••••• Output of the above code 👇
<div class="my-4">
  <button class="bg-sky-700 px-3 py-2 rounded-3xl text-white hover:text-slate-900 hover:bg-blue-400" >Contact
    Us</button>
</div>
→ We use `mx-2` inside the button tag to add margin to the button. Here `mx-2` is the class name and `2` is the margin of the button.

••••• Output of the above code 👇
<div class="my-4">
  <button class="bg-sky-700 px-3 py-2 rounded-3xl text-white hover:text-slate-900 hover:bg-blue-400 mx-2" >Contact
    Us</button>
</div>
→ We use `href="https://code-xam.vercel.app/"` inside the button tag to add a link to the button. Here `href="https://code-xam.vercel.app/"` is the link of the button.

••••• Output of the above code 👇
<div class="my-4">
  <button
    class="bg-sky-700 px-3 py-2 rounded-3xl text-white hover:text-slate-900  hover:bg-blue-400 mx-2"><a
    href="https://github.com/Subham-Maity/tailwind-css-tutorial" >Contact
    Us</a></button>
</div>
→ We use `target="_blank"` inside the button tag to open the link in a new tab. Here `target="_blank"` is the attribute of the button.

••••• Output of the above code 👇
<div class="my-4">
  <button
    class="bg-sky-700 px-3 py-2 rounded-3xl text-white hover:text-slate-900  hover:bg-blue-400 mx-2"><a
    href="https://github.com/Subham-Maity/tailwind-css-tutorial" target="_blank">Contact
    Us</a></button>
</div>

→ We use `hover:border-2` inside the button tag to add border to the button when we hover over it. Here `hover:border-2` is the class name and `2` is the border of the button when we hover over it.
••••• Output of the above code 👇
<div class="my-4">
  <button
    class="bg-sky-700 px-3 py-2 rounded-3xl text-white hover:text-slate-900  hover:bg-blue-400 mx-2 hover:border-2"><a
    href="https://github.com/Subham-Maity/tailwind-css-tutorial" target="_blank">Contact
    Us</a></button>
</div>

→ We use `hover:border-white `  inside the button tag to add border colour to the button when we hover over it. Here `hover:border-white` is the class name and `white` is the border colour of the button when we hover over it.

••••• Output of the above code 👇
<div class="my-4">
  <button
    class="bg-sky-700 px-3 py-2 rounded-3xl text-white hover:text-slate-900  hover:bg-blue-400 mx-2 hover:border-2 hover:border-white"><a
    href="https://github.com/Subham-Maity/tailwind-css-tutorial" target="_blank">Contact
    Us</a></button>
</div>

<div class="gradient-border" id="box"> </div>



#### Adding Your Profile Picture

- For now I have added my own photo you can replace it with your own photo. 😉
- Inside the public folder I add bg.png file
- Now I'll explain line by line `22,23,38,39,40`

```html filename="index.html" {22-23 ,38-40}
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://cdn.tailwindcss.com"></script>
    <title>Hey I'm a professional blockchain developer </title>
</head>

<body>
    <nav class="bg-[#1e293b] text-white flex justify-between">
        <img src="./public/blue green.png" class="h-16 pt-3 pb-2 px-4 rounded-3xl" alt="">
        <ul class="px-28 py-4 flex space-x-3 justify-end">
            <li class=" cursor-pointer">Home</li>
            <li class=" cursor-pointer">About</li>
            <li class=" cursor-pointer">Contact</li>
            <li class=" cursor-pointer">Projects</li>
        </ul>
    </nav>
    <main class="main bg-slate-400 flex justify-around">
        <div class="py-40 pl-9">
            <div class="text-6xl"> I am a professional blockchain developer </div>
            <p class="py-3 w-1/3">Showcase your knowledge of blockchain, machine learning, OOPs, DSA, and all advanced
                coding skills you desire.</p>
            <div class="my-4">
                <button
                    class="bg-sky-700 px-3 py-2 rounded-3xl text-white hover:text-slate-900 hover:bg-blue-400 mx-2 hover:border-2 hover:border-white"><a
                        href="https://code-xam.vercel.app/" target="_blank">CodeXam Website </a></button>
                <button
                    class="bg-sky-700 px-3 py-2 rounded-3xl text-white hover:text-slate-900  hover:bg-blue-400 mx-2 hover:border-2 hover:border-white"><a
                        href="https://github.com/Subham-Maity/tailwind-css-tutorial" target="_blank">Contact
                        Us</a></button>
            </div>
        </div>

   <div class = "flex items-center  ">
    <img src = "./public/bg1.png" class="h-64 pt-3 pb-1 px-4 rounded-l-3xl border-2 border-sky-500"/>
   </div>

    </main>
</body>

</html>
```
••••• Output of the above code 👇

<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%"   }  }>
  <nav class="bg-[#1e293b] text-white flex justify-between">
    <img src="https://github.com/Subham-Maity/tailwind-css-tutorial/blob/main/Chapter%202/Experimets/public/blue%20green.png?raw=true" class="h-16 pt-3 pb-2 px-4 rounded-3xl"  />
      <ul class="px-28 py-4 flex space-x-3 justify-end">
        <li class=" cursor-pointer">Home</li>
        <li class=" cursor-pointer">About</li>
        <li class=" cursor-pointer">Contact</li>
        <li class=" cursor-pointer">Projects</li>
      </ul>
  </nav>
  <main class="main bg-slate-400 flex justify-around">
    <div class="py-40 pl-9">
      <div class="text-6xl"> I am a professional blockchain developer </div>
      <p class="py-3 w-1/3">Showcase your knowledge of blockchain, machine learning, OOPs, DSA, and all advanced
        coding skills you desire.</p>
      <div class="my-4">
        <button
          class="bg-sky-700 px-3 py-2 rounded-3xl text-white hover:text-slate-900 hover:bg-blue-400 mx-2 hover:border-2 hover:border-white"><a
          href="https://code-xam.vercel.app/" target="_blank">CodeXam Website </a></button>
        <button
          class="bg-sky-700 px-3 py-2 rounded-3xl text-white hover:text-slate-900  hover:bg-blue-400 mx-2 hover:border-2 hover:border-white"><a
          href="https://github.com/Subham-Maity/tailwind-css-tutorial" target="_blank">Contact
          Us</a></button>
      </div>
    </div>

    <div class = "flex items-center  ">
      <img src = "https://github.com/Subham-Maity/tailwind-css-tutorial/blob/main/Chapter%202/Experimets/public/bg1.png?raw=true" class="h-35 pt-3 pb-1 px-4 rounded-l-3xl border-2 border-sky-500"/>
    </div>

  </main>
</div>

<img width="15%" height="2px" src="https://user-images.githubusercontent.com/97989643/201496986-b2def9d0-a6b2-46dc-94c3-ee0a7c39fd29.gif"></img>

→ We use `img` tag to add our profile picture add this image inside the `public` folder. and add the `src` attribute to the `img` tag and add the path of the image.

→ We use class `h-64` to set the height of the image.  `h-64` means 64px height. You can change the height according to your need.

→ We use class `pt-3` to set the padding top of the image.  `pt-3` means 3px padding top. You can change the padding top according to your need for this check this official documentation [here](https://tailwindcss.com/docs/padding).

→ We use class `pb-1` to set the padding bottom of the image.  `pb-1` means 1px padding bottom. You can change the padding bottom according to your need for this check this official documentation [here](https://tailwindcss.com/docs/padding).

→ We use class `px-4` to set the padding left and right of the image.  `px-4` means 4px padding left and right. You can change the padding left and right according to your need for this check this official documentation [here](https://tailwindcss.com/docs/padding).

→ We use class `rounded-l-3xl` to set the border radius of the image.  `rounded-l-3xl` means 3xl border radius. You can change the border radius according to your need for this check this official documentation [here](https://tailwindcss.com/docs/border-radius).

**We will give you some example of border radius.**

##### rounded class example

###### Type 1
```html
<img class="rounded"  width="15%" src="https://media.giphy.com/media/RsWTBRWrA071LXNMXM/giphy.gif"></img>
```
<img class="rounded"  width="15%" src="https://media.giphy.com/media/RsWTBRWrA071LXNMXM/giphy.gif"></img>

###### Type 2
```html
<img class="rounded-full"  width="15%" src="https://media.giphy.com/media/RsWTBRWrA071LXNMXM/giphy.gif"></img>
```
<img class="rounded-full"  width="15%" src="https://media.giphy.com/media/RsWTBRWrA071LXNMXM/giphy.gif"></img>

###### Type 3
```html
<img class="rounded-tl-3xl"  width="15%" src="https://media.giphy.com/media/RsWTBRWrA071LXNMXM/giphy.gif"></img>
```
<img class="rounded-tl-3xl"  width="15%" src="https://media.giphy.com/media/RsWTBRWrA071LXNMXM/giphy.gif"></img>

###### Type 4
```html
<img class="rounded-br-3xl"  width="15%" src="https://media.giphy.com/media/RsWTBRWrA071LXNMXM/giphy.gif"></img>
```
<img class="rounded-br-3xl"  width="15%" src="https://media.giphy.com/media/RsWTBRWrA071LXNMXM/giphy.gif"></img>

###### Type 5
```html
<img class="rounded-tr-3xl"  width="15%" src="https://media.giphy.com/media/RsWTBRWrA071LXNMXM/giphy.gif"></img>
```
<img class="rounded-tr-3xl"  width="15%" src="https://media.giphy.com/media/RsWTBRWrA071LXNMXM/giphy.gif"></img>

###### Type 6
```html
<img class="rounded-bl-3xl"  width="15%" src="https://media.giphy.com/media/RsWTBRWrA071LXNMXM/giphy.gif"></img>
```
<img class="rounded-bl-3xl"  width="15%" src="https://media.giphy.com/media/RsWTBRWrA071LXNMXM/giphy.gif"></img>

###### Type 7
```html
<img class="rounded-tl-3xl rounded-br-3xl"  width="15%" src="https://media.giphy.com/media/RsWTBRWrA071LXNMXM/giphy.gif"></img>
```
<img class="rounded-tl-3xl rounded-br-3xl"  width="15%" src="https://media.giphy.com/media/RsWTBRWrA071LXNMXM/giphy.gif"></img>

###### Type 8
```html
<img class="rounded-tr-3xl rounded-bl-3xl"  width="15%" src="https://media.giphy.com/media/RsWTBRWrA071LXNMXM/giphy.gif"></img>
```
<img class="rounded-tr-3xl rounded-bl-3xl"  width="15%" src="https://media.giphy.com/media/RsWTBRWrA071LXNMXM/giphy.gif"></img>

###### Type 9
```html
<img class="rounded-tl-3xl rounded-tr-3xl rounded-br-3xl rounded-bl-3xl"  width="15%" src="https://media.giphy.com/media/RsWTBRWrA071LXNMXM/giphy.gif"></img>
```
<img class="rounded-tl-3xl rounded-tr-3xl rounded-br-3xl rounded-bl-3xl"  width="15%" src="https://media.giphy.com/media/RsWTBRWrA071LXNMXM/giphy.gif"></img>

 We simply use this same concept rounded-l-3xl to set the border radius of the image.
```html

<img src = "https://github.com/Subham-Maity/tailwind-css-tutorial/blob/main/Chapter%202/Experimets/public/bg1.png?raw=true" class="h-64 pt-3 pb-1 px-4 rounded-l-3xl border-2 border-sky-500"/>

```
••••• Output of the above code 👇

<img src = "https://github.com/Subham-Maity/tailwind-css-tutorial/blob/main/Chapter%202/Experimets/public/bg1.png?raw=true" class="h-21 pt-3 pb-1 px-4 rounded-l-3xl border-2 border-sky-500"/>

→ We need to place this image inside the main page so we can simply shift the color `bg-slate-400` inside the `div` tag to inside the ``main`` tag
```html {1}
<main class="main bg-slate-400 ">
  <div class="py-40 pl-9">
......
  ....
..
```
if we do this our image will place inside the main page


••••• Output of the above code 👇


<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%"   }  }>
  <nav class="bg-[#1e293b] text-white flex justify-between">
    <img src="https://github.com/Subham-Maity/tailwind-css-tutorial/blob/main/Chapter%202/Experimets/public/blue%20green.png?raw=true" class="h-16 pt-3 pb-2 px-4 rounded-3xl"  />
    <ul class="px-28 py-4 flex space-x-3 justify-end">
      <li class=" cursor-pointer">Home</li>
      <li class=" cursor-pointer">About</li>
      <li class=" cursor-pointer">Contact</li>
      <li class=" cursor-pointer">Projects</li>
    </ul>
  </nav>
  <main class="main bg-slate-400">
    <div class="py-40 pl-9">
      <div class="text-6xl"> I am a professional blockchain developer </div>
      <p class="py-3 w-1/3">Showcase your knowledge of blockchain, machine learning, OOPs, DSA, and all advanced
        coding skills you desire.</p>
      <div class="my-4">
        <button
          class="bg-sky-700 px-3 py-2 rounded-3xl text-white hover:text-slate-900 hover:bg-blue-400 mx-2 hover:border-2 hover:border-white"><a
          href="https://code-xam.vercel.app/" target="_blank">CodeXam Website </a></button>
        <button
          class="bg-sky-700 px-3 py-2 rounded-3xl text-white hover:text-slate-900  hover:bg-blue-400 mx-2 hover:border-2 hover:border-white"><a
          href="https://github.com/Subham-Maity/tailwind-css-tutorial" target="_blank">Contact
          Us</a></button>
      </div>
    </div>

    <div>
      <img src = "https://github.com/Subham-Maity/tailwind-css-tutorial/blob/main/Chapter%202/Experimets/public/bg1.png?raw=true" class="h-35 pt-3 pb-1 px-4 rounded-l-3xl border-2 border-sky-500"/>
    </div>

  </main>
</div>

→ We use `flex justify-around` inside the `main` tag to place the image and text in the center of the page and we use `flex justify-between` inside the `nav` tag to place the image and text in the center of the page

You can check this official documentation for more information about space around [here](https://tailwindcss.com/docs/justify-content#space-around) and for flex you can check [here](https://tailwindcss.com/docs/flex-direction)

```html {1}
<main class="main bg-slate-400 flex justify-around ">
  <div class="py-40 pl-9">
......
  ....
..
```

••••• Output of the above code 👇

<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%"   }  }>
  <nav class="bg-[#1e293b] text-white flex justify-between">
    <img src="https://github.com/Subham-Maity/tailwind-css-tutorial/blob/main/Chapter%202/Experimets/public/blue%20green.png?raw=true" class="h-16 pt-3 pb-2 px-4 rounded-3xl"  />
    <ul class="px-28 py-4 flex space-x-3 justify-end">
      <li class=" cursor-pointer">Home</li>
      <li class=" cursor-pointer">About</li>
      <li class=" cursor-pointer">Contact</li>
      <li class=" cursor-pointer">Projects</li>
    </ul>
  </nav>
  <main class="main bg-slate-400 flex justify-around ">
    <div class="py-40 pl-9">
      <div class="text-6xl"> I am a professional blockchain developer </div>
      <p class="py-3 w-1/3">Showcase your knowledge of blockchain, machine learning, OOPs, DSA, and all advanced
        coding skills you desire.</p>
      <div class="my-4">
        <button
          class="bg-sky-700 px-3 py-2 rounded-3xl text-white hover:text-slate-900 hover:bg-blue-400 mx-2 hover:border-2 hover:border-white"><a
          href="https://code-xam.vercel.app/" target="_blank">CodeXam Website </a></button>
        <button
          class="bg-sky-700 px-3 py-2 rounded-3xl text-white hover:text-slate-900  hover:bg-blue-400 mx-2 hover:border-2 hover:border-white"><a
          href="https://github.com/Subham-Maity/tailwind-css-tutorial" target="_blank">Contact
          Us</a></button>
      </div>
    </div>

    <div>
      <img src = "https://github.com/Subham-Maity/tailwind-css-tutorial/blob/main/Chapter%202/Experimets/public/bg1.png?raw=true" class="h-35 pt-3 pb-1 px-4 rounded-l-3xl border-2 border-sky-500"/>
    </div>

  </main>
</div>

→ We use `flex items-center` inside the `img div` tag to place the image in the center of the page you can check this official documentation for more information about flex items center [here](https://tailwindcss.com/docs/align-items#center)

```html {2}
   <div class = "flex items-center">
    <img src = "./public/bg1.png" class="h-64 pt-3 pb-1 px-4 rounded-l-3xl border-2 border-sky-500"/>
   </div>
```
••••• Output of the above code 👇

<div style={{ border:"solid #888", position: "relative" ,opacity: 1 ,overflow: "hidden" , padding:"2%"   }  }>
  <nav class="bg-[#1e293b] text-white flex justify-between">
    <img src="https://github.com/Subham-Maity/tailwind-css-tutorial/blob/main/Chapter%202/Experimets/public/blue%20green.png?raw=true" class="h-16 pt-3 pb-2 px-4 rounded-3xl"  />
    <ul class="px-28 py-4 flex space-x-3 justify-end">
      <li class=" cursor-pointer">Home</li>
      <li class=" cursor-pointer">About</li>
      <li class=" cursor-pointer">Contact</li>
      <li class=" cursor-pointer">Projects</li>
    </ul>
  </nav>
  <main class="main bg-slate-400 flex justify-around ">
    <div class="py-40 pl-9">
      <div class="text-6xl"> I am a professional blockchain developer </div>
      <p class="py-3 w-1/3">Showcase your knowledge of blockchain, machine learning, OOPs, DSA, and all advanced
        coding skills you desire.</p>
      <div class="my-4">
        <button
          class="bg-sky-700 px-3 py-2 rounded-3xl text-white hover:text-slate-900 hover:bg-blue-400 mx-2 hover:border-2 hover:border-white"><a
          href="https://code-xam.vercel.app/" target="_blank">CodeXam Website </a></button>
        <button
          class="bg-sky-700 px-3 py-2 rounded-3xl text-white hover:text-slate-900  hover:bg-blue-400 mx-2 hover:border-2 hover:border-white"><a
          href="https://github.com/Subham-Maity/tailwind-css-tutorial" target="_blank">Contact
          Us</a></button>
      </div>
    </div>

    <div class = "flex items-center">
      <img src = "https://github.com/Subham-Maity/tailwind-css-tutorial/blob/main/Chapter%202/Experimets/public/bg1.png?raw=true" class="h-34 pt-3 pb-1 px-4 rounded-l-3xl border-2 border-sky-500"/>
    </div>

  </main>
</div>

## Conclusion
You can do many thing using tailwind css and showcase your creativity. I hope you enjoyed this tutorial and learned something new. If you have any doubt or suggestion please contact us. Thank you for reading this tutorial.We will see you in the next tutorial and we will learn about more tailwind css classes and how to use them. Till then stay tuned and keep learning.

## All Files For This Tutorial
You can download all the files from github [here](https://github.com/Subham-Maity/tailwind-css-tutorial/tree/main/Chapter%202)
