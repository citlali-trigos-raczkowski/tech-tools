# Tech Tools

## Terminal/IDE Setup (VSCode)

- [Code .](https://code.visualstudio.com/setup/mac) - Shortcut from terminal
- [Spotify Manager](https://github.com/hnarayanan/shpotify) - Control Spotify from terminal
- [Bash --> Zsh](https://www.freecodecamp.org/news/jazz-up-your-zsh-terminal-in-seven-steps-a-visual-guide-e81a8fd59a38/) - Nice way to set up terminal to using zsh. Here's what [mine](static/zsh-sample-terminal.md) currently looks like
  > Preview md in Vscode with: `Command + Shift + V` on the file

---

## New Project Setup

- Code Formatting
  - [Prettier](https://prettier.io/en/install.html) - Code Formatter
  - [Eslint](https://eslint.org/user-guide/getting-started) - Code Linter
- Pre-Commit Hooks
  - [Husky](https://typicode.github.io/husky/#/) and [Lint-staged](https://www.npmjs.com/package/lint-staged) - pre-commit hook managers
  - [Set up and sample package.json](./pre-commit-hooks.md) - for pre-commit hook to run prettier + eslint via husky and lint-staged
- Github Branch Protection
  - [Branch Protections](https://docs.github.com/en/enterprise-server@3.0/github/administering-a-repository/managing-a-branch-protection-rule) - Set up rules to protect your branches. Sample set up [here](./branch-protections.md)

---

## Publishing Docs

- [Github Pages](https://pages.github.com/) - publish your static docs with github pages
- [Docsify](https://angry-swanson-b4e47b.netlify.app/quickstart) - customize your github pages using docsify-cli (what this current document uses)

---

## Monorepos

- [Lerna](https://lerna.js.org/) - multi-javascript/typescript package manager. Can build new packages directly or pull from existing repo, bringing in all commit history

---

## Front-End

### Frameworks

- [React](https://reactjs.org/getting-started.html) - Fb-managed JS framework with fast startup (via create react app). Here's a [set up guide](./react-with-typescript.md) for React with Typescript.
- [Angular](https://angular.io/guide/setup-local) - Google-managed TS-based JS framework for mobile/web, using `ng ..` command
- [Vue.js](https://vuejs.org/v2/guide/) - Easiest to pick up

> React has a faster learning curve than Angular with less built-in, but Vue.js has the fastest ramp-up. React expects you to choose the additional libraries to add based on need, where Angular is "ready to go". React only uses JSX; Vue.js utilizes html. Here's is a [comparison](https://academind.com/tutorials/angular-vs-react-vs-vue-my-thoughts/).

### Creating Web Components

- [Open-WC](https://open-wc.org/) - Guides and tools to create Web Components
- [LitElement](https://lit-element.polymer-project.org/guide) - Base class for creating fast, lightweight web components that are framework-agnostic. Creates much lighter packages than a framework can (i.e. Angular, React)
- [Storybook](https://storybook.js.org/) - Open source tool for developing and demoing UI components

> [Sample set up](./lit-element-web-components.md) to create LitElement Web Components using open-wc's init, introducing storybook demoing capabilities and mocha testing

### Responsive Web App Frameworks

- [Material-UI](https://material-ui.com/) - the most popular React UI component library with generous [customization](https://material-ui.com/customization/theming/)
- [React Bootstrap](https://react-bootstrap.github.io/getting-started/introduction) - Extensive Component Library with minimal [customization](https://getbootstrap.com/4.5/utilities/colors/)

> Here's a [comparison](https://uxplanet.org/material-ui-vs-bootstrap-a-detailed-comparison-8fc9151db5ed) of Material UI vs. React Bootstrap

### Design

- [Material Design](https://material.io/design) - system of guidelines, components, and tools supporting best practices of UI design
- [Styled Components](https://styled-components.com/) - library for React and React Native that allows you to use CSS in modern JavaScript. Very quick set up, easy customization
- [coolors.io](https://coolors.co/) - Color scheme generator or explore trending palettes

> Here's a [list of beautiful websites](./website-designs.md) (imo)

---

## Testing

- [Mocha](https://mochajs.org/#installation) - JS-based tests organized in test suites (‘describe’-blocks) and test cases (‘it’-blocks)
- [Cucumber](https://cucumber.io/) - acceptance testing framework organized via Feature/Scenario tests and GIVEN/WHEN/THEN "steps". Very readable for non-programmers
- [Cypress](https://www.cypress.io/) - E2E testing written in JS typically used for frontend or UI testing with ability to fire REST requests via `cy.request`
