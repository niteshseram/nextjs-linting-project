### Setting up ESLint, Prettier and Husky with lint-staged in Next.js
This repo is created for the tutorial purpose of my blog post [Setting up ESLint, Prettier, and Husky with lint-staged for your Next.js Project](https://niteshseram.in/blog/setting-up-eslint-prettier-and-husky-with-lint-staged-for-your-nextjs-project).

#### Follow through commits
To follow through the process of setting these configuration, checkout the commits
- Step 1: Adding `next lint` script in `package.json` file. When this script is runned, it will install `eslint` and `eslint-config-next`
- Step 2: To add more eslint rules to the existing one, we add `eslint:recommended` in `.eslintrc.json` file
- Step 3: We install `prettier` and `eslint-config-prettier` and setup the config for prettier in `.prettierrc.json` file. And finally add `prettier` in `.eslintrc.json` file as well
- Step 4: Add a script `format": "prettier --write .` in `package.json` to format all our files in one go
- Step 5: Install `husky` and `lint-staged` and add the script `prepare": "husky install` in the `package.json` file. Then run `npm run prepare` or `yarn prepare` to install some necessary script for huksy to work
- Step 6: Add `lint-staged` script and `precommit` script in `package.json` file
- Step 7: Finally, run `npx husky add .husky/pre-commit "npm run precommit"` to create a precommit hook which will run `precommit` script everytime when we do some commit

Visit the blog [post](https://niteshseram.in/blog/setting-up-eslint-prettier-and-husky-with-lint-staged-for-your-nextjs-project) to follow in details.

Hope this finds you helpful🙂

