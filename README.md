# Boilerplate and Starter for Next JS 12+, Tailwind CSS 3, StoryBook and TypeScript

🚀 Boilerplate and Starter for **Next.js, Tailwind CSS, StoryBook and TypeScript** ⚡️ Made with: _Next.js, TailwindCSS, SASS/SCSS, PostCSS, Husky, Lint-Staged, VSCode, StoryBook, AWS Amplify and TypeScript_.

Clone this project and use it to create your own Next.js project.

## Features

- 🔥 [Next.js 12](https://nextjs.org/) for Static Site Generator
- 🎨 Integrate with [Tailwind CSS](https://tailwindcss.com/) and [SASS/SCSS](https://sass-lang.com/)
- 💅 [PostCSS](https://postcss.org/) for processing Tailwind CSS
- 🎉 Type checking [TypeScript](https://www.typescriptlang.org/)
- ✅ Strict Mode for TypeScript and React 18
- ✏️ Linter with [ESLint](https://eslint.org/) (default NextJS, NextJS Core Web Vitals, Tailwind CSS and StoryBook configuration)
- 🛠 Code Formatter with [Prettier](https://prettier.io/)
- 🦊 [Husky](https://typicode.github.io/husky/) for Git Hooks
- 🚫 [Lint-Staged](https://github.com/okonet/lint-staged) for running linters on Git staged files
- 🗂 VSCode configuration: Debug, Settings, Tasks and extension for PostCSS, ESLint, Prettier, TypeScript
- 🙌 [StoryBook](https://storybook.js.org/) for streamlining UI development, testing, and documentation
- 🦾 [AWS Amplify](https://docs.amplify.aws/) for providing serverless API easily and faster via [GraphQL](https://graphql.org/).

## Requirements

- Node.js 14+ and yarn or npm

<hr>

# Introduction (TL;DR)

In this section, I'm going to share informations via questions about tech stack of this repo using some useful resources.

## About AWS Amplify

> AWS Amplify helps front-end web and mobile developers build apps faster. It consists of a development framework and a web hosting service to build and deploy secure and scalable mobile and web applications powered by AWS.

### What’s included in AWS Amplify?

> AWS Amplify includes a wide variety of open-source libraries and drag-and-drop UI components developers can use as building blocks for their apps. It also has a built-in CLI you can use to build your backend. And for an additional fee, AWS Amplify Console provides web hosting services for your app.

> AWS Amplify has components for:
>
> - Data storage
>   - Keep your app data synced with the cloud, manage your distributed data, and handle subscriptions and messaging.
> - Analytics
>   - Track user sessions and report on their behavior. Set up custom attributes and analyze conversion funnels.
> - Push notifications
>   - Easily manage your campaigns and send messages to your users across multiple channels, including text, email, and push.
> - Authentication
>   - Access ready-to-use workflows for MFA, single sign-on, forgot password, etc.

### What is AWS Amplify compatible with?

> The framework supports iOS, Android, Web, and React Native mobile apps, and React, Ionic, Angular, and Vue.js for web apps.

### Who should use AWS Amplify?

> AWS Amplify is awesome for people who don’t want to build their backend or other components from scratch. The Amplify components make it easy to set up the building blocks of your app without doing all the legwork yourself.

> That’s a pretty broad use case, but that’s the point—it’s meant to appeal to a large base.

### What companies have used AWS Amplify?

> The [public customer list](https://aws.amazon.com/amplify/customers/) for AWS Amplify isn’t very robust yet. They do have a couple heavy-hitters though, like millennial-favorite fitness app Noom and location tracking cloud service HyperTrack.

> There are a lot of other reviews of the service on the web, too: note this one that says [using Amplify “feels like cheating.”](https://medium.com/@coryschimmoeller/using-aws-amplify-feels-like-cheating-e5eabcaea500)

The app that you built with AWS Amplify is also a serverless app that can use some services such as [AWS AppSync(for GraphQL interface)](https://docs.aws.amazon.com/appsync/latest/devguide/what-is-appsync.html), [AWS Cognito User Pools(for auth)](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-identity-pools.html), [AWS Lambda Functions](https://docs.aws.amazon.com/lambda/latest/dg/welcome.html), [AWS DynamoDB](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html) etc.

## About SASS/SCSS, TailwindCSS and CSS Modules

### What is SASS?

> - SASS stands for Syntactically Awesome Stylesheet
> - SASS is an extension to CSS
> - SASS is a CSS pre-processor
> - SASS is completely compatible with all versions of CSS
> - SASS reduces repetition of CSS and therefore saves time
> - SASS was designed by Hampton Catlin and developed by Natalie Weizenbaum in 2006
> - SASS is free to download and use

### Why Use SASS?

> Stylesheets are getting larger, more complex, and harder to maintain. This is where a CSS pre-processor can help.

> SASS lets you use features that do not exist in CSS, like variables, nested rules, mixins, imports, inheritance, built-in functions, and other stuff.

### What is the difference between SCSS and SASS?

> SASS (Syntactically Awesome Style Sheets) is a pre-processor scripting language that will be compiled or interpreted into CSS. SassScript is itself a scripting language whereas SCSS is the main syntax for the SASS which builds on top of the existing CSS syntax. It makes use of semicolons and brackets like CSS (Cascaded Style Sheets).

> SASS and SCSS can import each other. Sass actually makes CSS more powerful with math and variable support.

> Let’s list down the main difference between SASS and SCSS.
>
> - SASS is used when we need an original syntax, code syntax is not required for SCSS.
> - SASS follows strict indentation, SCSS has no strict indentation.
> - SASS has a loose syntax with white space and no semicolons, the SCSS resembles more to CSS style and use of semicolons and braces are mandatory.
> - SASS file extension is .sass and SCSS file extension is .scss.
> - SASS has more developer community and support than SCSS.

<hr>

### What is TailwindCSS?

> Tailwind CSS is basically a utility-first CSS framework for rapidly building custom user interfaces. It is a highly customizable, low-level CSS framework that gives you all of the building blocks you need to build bespoke designs without any annoying opinionated styles you have to fight to override.

> The beauty of this thing called tailwind is it doesn’t impose design specification or how your site should look like, you simply bring tiny components together to construct a user interface that is unique. What Tailwind simply does is take a ‘raw’ CSS file, processes this CSS file over a configuration file, and produces an output.

### Why Tailwind CSS?

> - Faster UI building process
> - It is a utility-first CSS framework which means we can use utility classes to build custom designs without writing CSS as in traditional approach.

### Advantages of Tailwind CSS

> - No more silly names for CSS classes and Id’s.
> - Minimum lines of Code in CSS file.
> - We can customize the designs to make the components.
> - Makes the website responsive.
> - Makes the changes in the desired manner.
> - CSS is global in nature and if make changes in the file the property is changed in all the HTML files linked to it. But with the help of Tailwind CSS we can use utility classes and make local changes.

<hr>

### What are CSS Modules and why do we need them?

> According to the [repo](https://github.com/css-modules/css-modules), CSS modules are:

> > CSS files in which all class names and animation names are scoped locally by default.

> So CSS Modules is not an official spec or an implementation in the browser but rather a process in a build step (with the help of [Webpack](https://webpack.github.io/) or [Browserify](http://browserify.org/)) that changes class names and selectors to be scoped (i.e. kinda like namespaced).

> CSS Modules takes a different approach. Instead of writing plain HTML, we need to write all of our markup in a JavaScript file, like index.js. Here’s an example of how that might work (we’ll take a look at a more realistic example later):

```js
import styles from './styles.css'

element.innerHTML = `<h1 class="${styles.title}">
     An example heading
   </h1>`
```

> During our build step, the compiler would search through that `styles.css` file that we’ve imported, then look through the JavaScript we’ve written and make the .title class accessible via styles.title. Our build step would then process both these things into new, separate HTML and CSS files, with a new string of characters replacing both the HTML class and the CSS selector class.

> Our generated HTML might look like this:

```html
<h1 class="_styles__title_309571057"> An example heading </h1>
```

> Our generated CSS might look like this:

```css
._styles__title_309571057 {
  background-color: red;
}
```

> The class attribute and selector `.title` is entirely gone, replaced by this entirely new string; Our original CSS is not being served to the browser at all.

> > [the classes] are dynamically generated, unique, and mapped to the correct styles.

> This is what is meant by styles being scoped. They are scoped to particular templates. If we have a `buttons.css` file we would import it only into a buttons.js template and a `.btn` class within would be inaccessible to some other template (e.g. forms.js), unless we imported it specifically there too.

#### Why should we use CSS Modules?

> With CSS Modules, it’s a guarantee that all the styles for a single component:

> - Live in one place
> - Only apply to that component and nothing else

> Plus, any component can have a true dependency, like:

```js
import buttons from './buttons.css'
import padding from './padding.css'

element.innerHTML = `<div class="${buttons.red} ${padding.large}">`
```

> **This approach is designed to fix the problem of the global scope in CSS.**

<hr>

### **In this repo, SCSS and its modules have been used with TailwindCSS for styling. But _webpack5_ and _postcss_ configuration have been done with _sass-loader_, _postcss-loader_ plugins. (So you are also free to use SASS files.)**

<hr>

# Configuration

## Styling Configuration

First, I created [`tailwind.config.js`](./tailwind.config.js) and [`postcss.config.js`](./postcss.config.js) files. Then I added blocks which are below:

```js
// tailwind.config.js

module.exports = {
  content: ['./pages/**/*.{js,ts,jsx,tsx}', './src/**/*.{js,jsx,ts,tsx}'],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

```js
// postcss.config.js

module.exports = {
  plugins: ['tailwindcss', 'autoprefixer', 'tailwindcss/nesting'],
}
```

The most configuration takes my time was StoryBook configuration because I wanted to integrate StoryBook to Tailwind CSS that is able to be compiled in SASS/SCSS files.

Here are `addons` in [`.storybook/main.js`](./.storybook/main.js) file:

```js
addons: [
    '@storybook/addon-links',
    '@storybook/addon-essentials',
    '@storybook/addon-interactions',
    '@storybook/preset-scss', // added later
    { // added later
      name: '@storybook/addon-postcss',
      options: {
        cssLoaderOptions: {
          importLoaders: 1,
        },
        postcssLoaderOptions: {
          implementation: require('postcss'),
        },
      },
    },
  ],
```

And `webpackFinal`:

```js
webpackFinal: async (config) => {
  config.resolve.alias = {
    ...config.resolve?.alias,
    '@': [
      require('path').resolve(__dirname, '../src/'),
      require('path').resolve(__dirname, '../'),
    ],
  }

  config.resolve.roots = [
    require('path').resolve(__dirname, '../public'),
    'node_modules',
  ]

  config.module.rules.push({
    // this rule is for using TailwindCSS in .sass and .scss files.
    test: /\.s[ac]ss$/,
    use: [
      {
        loader: 'postcss-loader',
        options: {
          postcssOptions: {
            plugins: [require('tailwindcss'), require('autoprefixer')],
          },
        },
      },
      {
        loader: 'sass-loader',
        options: {
          implementation: require('sass'),
        },
      },
    ],
    include: require('path').resolve(__dirname, '../'),
  })

  return config
}
```

Here is [`.storybook/preview.js`](./.storybook/preview.js):

```js
import '../src/styles/globals.scss' //For using Tailwind CSS in global scope for StoryBook
import * as NextImage from 'next/image' // For previewing images in StoryBook

const OriginalNextImage = NextImage.default

Object.defineProperty(NextImage, 'default', {
  configurable: true,
  value: (props) => <OriginalNextImage {...props} unoptimized />,
})

export const parameters = {
  actions: { argTypesRegex: '^on[A-Z].*' },
  controls: {
    matchers: {
      color: /(background|color)$/i,
      date: /Date$/,
    },
  },
  previewTabs: {
    'storybook/docs/panel': { index: -1 },
  },
}
```

## ESLint and Prettier Configuration

ESLint and Prettier configurations have been done in [`.eslintrc.json`](./.eslintrc.json), [`.prettierrc.json`](./.prettierrc.json) files and [`.vscode`](./.vscode) folder.

There are not much rules, so you're free to change the rules.

## Husky and Lint-Staged Configuration

You need to enable Husky:

```sh
yarn husky install
```

Then a folder is going to be created under the `.husky` folder named as "`_`".

Husky "`pre commit`" configuration have been done in [`.husky/pre-commit`](./.husky/pre-commit) and lint-stage configuration have been done in [`lint-staged.config.js`](./lint-staged.config.js).

Now, when you use `git commit -m "something"` command, it will run lint-staged scripts according to configuration in [`lint-staged.config.js`](<(./lint-staged.config.js)>) if type checking and/or linting is necessary.

# Getting Started

> I've been using yarn therefore there is yarn.lock file, I recommend you to use yarn for this repo.

## Initialize and deploy the Amplify project

<details>
  <summary>If you've never used amplify before </summary>

### Install & Configure Amplify

1. [Sign up](https://portal.aws.amazon.com/billing/signup#/start) for an AWS account
2. Install the AWS Amplify cli:

```sh
npm install -g @aws-amplify/cli
```

3. Configure the Amplify cli

```sh
amplify configure
```

[Read More](https://aws-amplify.github.io/docs/cli-toolchain/quickstart?sdk=js)

</details>

### Initialize Amplify

```sh
$ amplify init

# <Interactive>
? Enter a name for the project <PROJECT_NAME>
? Enter a name for the environment: dev (or whatever you would like to call this env)
? Choose your default editor: <YOUR_EDITOR_OF_CHOICE>
? Choose the type of app that you're building (Use arrow keys)
  android
  ios
❯ javascript
? What javascript framework are you using react
? Source Directory Path:  src
? Distribution Directory Path: out
? Build Command:  (npm run-script build)
? Start Command: (npm run-script start)
? Do you want to use an AWS profile? Y

# </Interactive>
```

### Add the API

```sh
$ amplify add api
# <Interactive>
? Please select from one of the below mentioned services (Use arrow keys)
❯ GraphQL
  REST
? Provide API name: <API_NAME>
? Choose an authorization type for the API (Use arrow keys)
❯ API key
  Amazon Cognito User Pool
? Do you have an annotated GraphQL schema? (y/N) y
? Provide your schema file path: ./schema.graphql
# </Interactive>
```

### Deploy infrastructure

```sh
$ amplify push
# <Interactive>
? Are you sure you want to continue? Y
? Do you want to generate code for your newly created GraphQL API? Y
? Choose the code generation language target (Use arrow keys)
❯ javascript
  typescript
  flow
? Enter the file name pattern of graphql queries, mutations and subscriptions (src/graphql/**/*.js)
? Do you want to generate/update all possible GraphQL operations - queries, mutations and subscriptions (Y/n) Y
? Enter maximum statement depth [increase from default if your schema is deeply nested] (2)

# </Interactive>
```

# Install & Run

```sh
npm install
# or
yarn
```

Now you can run development server:

```sh
npm run dev
# or
yarn dev
```

<hr>
Or run the StoryBook:

```sh
npm run storybook
# or
yarn storybook
```

If you've run **development server**, open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

If you've run the **StoryBook**, then it's going to open itself automatically on the port 6006.

You can start editing the page by modifying [`pages/index.tsx`](./pages/index.tsx). The page auto-updates as you edit the file.

[API routes](https://nextjs.org/docs/api-routes/introduction) can be accessed on [http://localhost:3000/api/hello](http://localhost:3000/api/hello). This endpoint can be edited in [`pages/api/hello.ts`](./pages/api/hello.ts).

The [`pages/api`](./pages/api/) directory is mapped to `/api/*`. Files in this directory are treated as [API routes](https://nextjs.org/docs/api-routes/introduction) instead of React pages.

<hr>

## About AWS Amplify Part in the Code

This example shows how to build a server rendered web application with NextJS and AWS Amplify. We use AWS Amplify to generate code and to manage and consume the AWS cloud resources needed for our app. The NextJS app has dynamic and static routes to demonstrate how to load data on the server based on the incoming request.

There are two routes that are implemented:

- `/` : A static route that uses `getStaticProps` to load data from AppSync and renders it on the server (Code in [pages/index(amplify-example).js](<./pages/index(amplify-example).js>))
- `/todo/[id]` : A dynamic route that uses `getServerSideProps` and the id from the provided context to load a single todo from AppSync and render it on the server. (Code in [pages/todo(amplify-example)/:[id].js](</pages/todo(amplify-example)/[id].js>))

The folders or files that contain `(amplify-example)` in their names aren't tested yet. These files/folders have taken from [Next.js example which is using aws-amplify](https://github.com/vercel/next.js/tree/canary/examples/with-aws-amplify)

### Edit GraphQL Schema

1. Open `amplify/backend/api/projectname/schema.graphql` and change what you need to.
2. Run `amplify push`
3. 👍

### Use with new Amplify project

Make sure to commit your changes before doing this.

```sh
mv amplify/backend/api/yourprojectname/schema.graphql ./schema.graphql
rm -rf amplify/ src/
amplify init
amplify add api
rm ./schema.graphql
amplify push
```

# Learn More & Resources

To learn more about mentione tech stack, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.
- [AWS Amplify Guide for React](https://docs.amplify.aws/start/q/integration/react/?sc_icampaign=react-start&sc_ichannel=docs-home) - AWS Amplify Guide for React.
- [AWS Amplify Guide for Next.js](https://docs.amplify.aws/start/q/integration/next/) - AWS Amplify Guide for Next.js.
- [A Next.js and AWS Amplify Blog Post](https://aws.amazon.com/tr/blogs/mobile/host-a-next-js-ssr-app-with-real-time-data-on-aws-amplify/) - A blog post about hosting a Next.js SSR app on AWS Amplify.
- [Review Example Project](https://github.com/vercel/next.js/tree/canary/examples/with-aws-amplify) - an example of Next.js with AWS Amplify.
- [ESLint, Prettier, Husky and lint-staged Configuration](https://paulintrognon.fr/blog/typescript-prettier-eslint-next-js) - an example of using together ESLint, Prettier, Husky and lint-staged for code typing rules and typescript errors.
- [How to Use Sass with CSS Modules in Next.js](https://www.freecodecamp.org/news/how-to-use-sass-with-css-modules-in-next-js/#what-are-css-modules) - an example of using together CSS modules, SASS and Next.js.
- [What is AWS Amplify?](https://www.bluematador.com/blog/what-is-aws-amplify#:~:text=AWS%20Amplify%20includes%20a%20wide,hosting%20services%20for%20your%20app.) - A resource of this repo's Readme.md
- [Introduction to Tailwind CSS](https://www.geeksforgeeks.org/introduction-to-tailwind-css/#:~:text=Tailwind%20CSS%20is%20basically%20a,have%20to%20fight%20to%20override.) - A resource of this repo's Readme.md
- [What is SASS?](https://www.w3schools.com/sass/sass_intro.php) - A resource of this repo's Readme.md
- [What is the difference between SCSS and SASS?](https://www.geeksforgeeks.org/what-is-the-difference-between-scss-and-sass/) - A resource of this repo's Readme.md
- [What are CSS Modules and why do we need them?](https://css-tricks.com/css-modules-part-1-need/) - A resource of this repo's Readme.md
- [A litte help](https://github.com/ixartz/Next-js-Boilerplate) - A litte help for creating Readme file for this repo
