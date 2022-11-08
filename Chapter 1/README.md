

## Introduction
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

<h3 className="text-center font-extrabold md:text-2xl mt-8">Installation</h3>
<div className="steps-container">
  <style jsx>{`
    .steps-container {
      margin-left: 1rem;
      padding-left: 1.5rem;
      counter-reset: step;
      border-left: 1px solid;
      border-color: rgb(229 231 235/1);
    }
    .steps-container :global(h3) {
      counter-increment: step;
    }
    .steps-container :global(h3):before {
      content: counter(step);
      display: inline-block;
      position: absolute;
      margin-top: 3px;
      margin-left: -41px;
      width: 33px;
      height: 33px;
      text-align: center;
      text-indent: -1px;
      color: #999;
      border-radius: 100%;
      border: 4px solid #fff;
      background: #f3f3f3;
      line-height: 1.5rem;
      font-size: 1rem;
      font-weight: 400;
    }
  `}</style>

  <h3>Install Tailwind CSS</h3>

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
</div>


