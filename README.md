# Introduction

This repo is a boilerplate that created for using some useful techs together. The mentioned techs are **Next.js, TailwindCSS, SASS/SCSS, StoryBook, AWS Amplify and TypeScript**.

<hr>

> AWS Amplify helps front-end web and mobile developers build apps faster. It consists of a development framework and a web hosting service to build and deploy secure and scalable mobile and web applications powered by AWS.

With AWS Amplify, you are able to solve authentication/social authentication issues very easily.

The app that you built with AWS Amplify is also a serverless app that uses some services such as AWS AppSync(contains GraphQL schemas etc.), AWS Cognito User Pools, AWS Lambda Functions etc.

TailwindCSS configuration have been done in the files that are [`tailwind.config.js`](tailwind.config.js), [`postcss.config.js`](postcss.config.js), [`.storybook/main.js`](./.storybook/main.js), [`.storybook/preview.js`](./.storybook/preview.js) for using TailwindCSS via SCSS in Next and StoryBook files.

This repo also includes [**Husky**](https://typicode.github.io/husky/), [**Lint-Stage**](https://github.com/okonet/lint-staged), **ESLint** and **Prettier**.

ESLint and Prettier configurations have been done in [`.eslintrc.json`](./.eslintrc.json), [`.prettierrc.json`](./.prettierrc.json) and [`.vscode/settings.json`](./.vscode/settings.json).

Husky/lint-stage configuration have been done in [`.husky/pre-commit`](./.husky/pre-commit) and [`lint-staged.config.js`](./lint-staged.config.js).

I've done all the configuration and test them manually.

<hr>

## Getting Started

> I've been using yarn therefore there is yarn.lock file, I recommend you to use yarn.

### Initialize and deploy the Amplify project

<details>
  <summary>If you've never used amplify before </summary>

#### Install & Configure Amplify

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

```bash
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

<hr>

## Install & Run

```bash
npm install
# or
yarn
```

You need to enable Husky:

```bash
yarn husky install
```

Now you can run development server:

```bash
npm run dev
# or
yarn dev
```

<hr>
Or run the StoryBook:

```bash
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

## About AWS Amplify part

This example shows how to build a server rendered web application with NextJS and AWS Amplify. We use AWS Amplify to generate code and to manage and consume the AWS cloud resources needed for our app. The NextJS app has dynamic and static routes to demonstrate how to load data on the server based on the incoming request.

There are two routes that are implemented :

- `/` : A static route that uses `getStaticProps` to load data from AppSync and renders it on the server (Code in [pages/index(amplify-example).js](./pages/index(amplify-example).js))
- `/todo/[id]` : A dynamic route that uses `getServerSideProps` and the id from the provided context to load a single todo from AppSync and render it on the server. (Code in [pages/todo(amplify-example)/:[id].js](/pages/todo(amplify-example)/[id].js))

<hr>

## Edit GraphQL Schema

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

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.
- [AWS Amplify Docs for React](https://docs.amplify.aws/start/q/integration/react/?sc_icampaign=react-start&sc_ichannel=docs-home) - AWS Amplify Docs for React.
- [AWS Amplify Docs for Next.js](https://docs.amplify.aws/start/q/integration/next/) - AWS Amplify Docs for Next.js.
- [A Next.js and AWS Amplify Blog Post](https://aws.amazon.com/tr/blogs/mobile/host-a-next-js-ssr-app-with-real-time-data-on-aws-amplify/) - A blog post about hosting a Next.js SSR app on AWS Amplify.
- [Review Example Project](https://github.com/vercel/next.js/tree/canary/examples/with-aws-amplify) - an example of Next.js with AWS Amplify.
- [ESLint, Prettier, Husky and lint-staged Configuration](https://paulintrognon.fr/blog/typescript-prettier-eslint-next-js) - an example of using together ESLint, Prettier, Husky and lint-staged for code typing rules and typescript errors.
