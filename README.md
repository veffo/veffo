<p align="center">
	<a href="https://thehassantahir.me" target="_blank"><img src="https://github.com/thehassantahir/thehassantahir/blob/main/github-banner.png"></a>
</p>

# react-simple-pull-to-refresh

[![npm version](https://badge.fury.io/js/react-simple-pull-to-refresh.svg)](https://badge.fury.io/js/react-simple-pull-to-refresh)
[![license](https://img.shields.io/github/license/thmsgbrt/react-simple-pull-to-refresh.svg)](https://github.com/thmsgbrt/react-simple-pull-to-refresh/blob/master/LICENSE)
![](https://badgen.net/npm/types/react-simple-pull-to-refresh)
![](https://badgen.net/badge/maintained/yes/green)

A Simple Pull-To-Refresh Component for React Application with 0 dependency.
Works for Mobile and Desktop.

## Contributing

⚠️ I don't have much time to take care of the issues at the moment.

🙏 Any help and contribution is greatly appreciated.

## Demo

[Click here 👍](https://thmsgbrt.github.io/react-simple-pull-to-refresh)

## Installation

`npm i react-simple-pull-to-refresh`

## Usage

```jsx
import PullToRefresh from 'react-simple-pull-to-refresh';
```

Pull To Refresh only

```jsx
// ...

return (
  <PullToRefresh onRefresh={handleRefresh}>
    <ul>
      {list.map((item, index) => (
        <li key={index}>{item}</li>
      ))}
    </ul>
  </PullToRefresh>
);

// ...
```

Pull To Refresh and Fetch More enabled

```jsx
// ...

return (
  <PullToRefresh onRefresh={handleRefresh} canFetchMore={true} onFetchMore={handleFetchMore}>
    <ul>
      {list.map((item, index) => (
        <li key={index}>{item}</li>
      ))}
    </ul>
  </PullToRefresh>
);

// ...
```

## Props Matrix

|        Name         |         Type          | Required |        Default        | Description                                                                  |
| :-----------------: | :-------------------: | :------: | :-------------------: | ---------------------------------------------------------------------------- |
|     isPullable      |        boolean        |  false   |         true          | Enable or disable pulling feature                                            |
|      onRefresh      |  () => Promise<any>   |   true   |                       | Function called when Refresh Event has been trigerred                        |
|  pullDownThreshold  |        number         |  false   |          67           | Distance in pixel to pull to trigger a Refresh Event                         |
| maxPullDownDistance |        number         |  false   |          95           | Maximum transitionY applied to Children when dragging                        |
|     resistance      |        number         |  false   |           1           | Scale of difficulty to pull down                                             |
|  refreshingContent  | JSX.Element or string |  false   | <RefreshingContent /> | Content displayed when Pulling or Fetch more has been trigerred              |
|   pullingContent    | JSX.Element or string |  false   |  <PullingContent />   | Content displayed when Pulling                                               |
|    canFetchMore     |        boolean        |  false   |         false         | Enable or disable fetching more feature                                      |
|     onFetchMore     |  () => Promise<any>   |  false   |                       | Function called when Fetch more Event has been trigerred                     |
| fetchMoreThreshold  |        number         |  false   |          100          | Distance in pixel from bottom of the container to trigger a Fetch more Event |
|   backgroundColor   |        string         |  false   |                       | Apply a backgroundColor                                                      |
|      className      |        string         |  false   |                       |                                                                              |

## Changelog

1.3.3: Update package.json peerDependencies to support react 18 - (From: [@mjauernig](https://github.com/mjauernig))

1.3.2: Fix build issue encountered with 1.3.1

1.3.1: Fix issue preventing fixed elements to work properly - (From: [@ManuDoni](https://github.com/ManuDoni))

1.3.0: Add a _resistance_ prop, that allows to adjust the pull down difficulty - (From: [@joshuahiggins](https://github.com/joshuahiggins))

1.2.5: Fix event listenter leaks - (From: [@d-s-x](https://github.com/d-s-x))

1.2.4: Fix overscroll on iOS Safari - (From: [@d-s-x](https://github.com/d-s-x))

1.2.3: Add React 17+ as valid peer dependencies - (From: [@Felixmosh](https://github.com/felixmosh))

1.2.2: Remove non-null assertion operators from ref.current + TouchEvent check for Mozilla - (From: [@HamAndRock](https://github.com/HamAndRock))

1.2.1: Remove unnecessary z-index

1.2.0: onRefresh and onFetchMore now require to be of type () => Promise<any>

1.1.2: Bind Scroll event to Window

1.1.0: Check for "canFetchMore" value for each scroll events.

1.1.0: Add a Fetch More feature















<h1><img src="https://emojis.slackmojis.com/emojis/images/1531849430/4246/blob-sunglasses.gif?1531849430" width="30"/> Hey! Nice to see you.</h1>


<p>Welcome to my page! </br> I'm Thomas, Fullstack developer from <img src="https://cdn-icons-png.flaticon.com/512/197/197560.png" width="13"/> <b>Lorient, France</b>, currently living in <img src="https://cdn-icons-png.flaticon.com/512/197/197564.png" width="13"/> <b>Stockholm, Sweden</b>. </p>
<h3>Things I code with</h3>
<p>
  <img alt="React" src="https://img.shields.io/badge/-React-45b8d8?style=flat-square&logo=react&logoColor=white" />
  <img alt="Webpack" src="https://img.shields.io/badge/-Webpack-8DD6F9?style=flat-square&logo=webpack&logoColor=white" /> 
  <img alt="Docker" src="https://img.shields.io/badge/-Docker-46a2f1?style=flat-square&logo=docker&logoColor=white" />
  <img alt="github actions" src="https://img.shields.io/badge/-Github_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white" />
  <img alt="Google Cloud Platform" src="https://img.shields.io/badge/-Google_Cloud_Platform-1a73e8?style=flat-square&logo=google-cloud&logoColor=white" />
  <img alt="TypeScript" src="https://img.shields.io/badge/-TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white" />
  <img alt="Insomnia" src="https://img.shields.io/badge/-Insomnia-5849BE?style=flat-square&logo=insomnia&logoColor=white" />
  <img alt="Apollo" src="https://img.shields.io/badge/-Apollo%20GraphQL-311C87?style=flat-square&logo=apollo-graphql&logoColor=white" />
  <img alt="Heroku" src="https://img.shields.io/badge/-Heroku-430098?style=flat-square&logo=heroku&logoColor=white" />
  <img alt="redux" src="https://img.shields.io/badge/-Redux-764ABC?style=flat-square&logo=redux&logoColor=white" />
  <img alt="ReactiveX" src="https://img.shields.io/badge/-RxJs-B7178C?style=flat-square&logo=reactivex&logoColor=white" />
  <img alt="GraphQL" src="https://img.shields.io/badge/-GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" />
  <img alt="Sass" src="https://img.shields.io/badge/-Sass-CC6699?style=flat-square&logo=sass&logoColor=white" />
  <img alt="Styled Components" src="https://img.shields.io/badge/-Styled_Components-db7092?style=flat-square&logo=styled-components&logoColor=white" />
  <img alt="git" src="https://img.shields.io/badge/-Git-F05032?style=flat-square&logo=git&logoColor=white" />
  <img alt="NestJs" src="https://img.shields.io/badge/-NestJs-ea2845?style=flat-square&logo=nestjs&logoColor=white" />
  <img alt="angular" src="https://img.shields.io/badge/-Angular-DD0031?style=flat-square&logo=angular&logoColor=white" />
  <img alt="npm" src="https://img.shields.io/badge/-NPM-CB3837?style=flat-square&logo=npm&logoColor=white" />
  <img alt="html5" src="https://img.shields.io/badge/-HTML5-E34F26?style=flat-square&logo=html5&logoColor=white" />
  <img alt="Brave browser" src="https://img.shields.io/badge/-Brave_Browser-FB542B?style=flat-square&logo=brave&logoColor=white" />
  <img alt="Rollup" src="https://img.shields.io/badge/-Rollup-EC4A3F?style=flat-square&logo=rollup.js&logoColor=white" />
  <img alt="d3js" src="https://img.shields.io/badge/-D3.js-F9A03C?style=flat-square&logo=d3.js&logoColor=white" />
  <img alt="Prettier" src="https://img.shields.io/badge/-Prettier-F7B93E?style=flat-square&logo=prettier&logoColor=white" />
  <img alt="MongoDB" src="https://img.shields.io/badge/-MongoDB-13aa52?style=flat-square&logo=mongodb&logoColor=white" />
  <img alt="Nodejs" src="https://img.shields.io/badge/-Nodejs-43853d?style=flat-square&logo=Node.js&logoColor=white" />
</p>
<h3>Open source projects</h3>
<table>
  <thead align="center">
    <tr border: none;>
      <td><b>🎁 Projects</b></td>
      <td><b>⭐ Stars</b></td>
      <td><b>📚 Forks</b></td>
      <td><b>🛎 Issues</b></td>
      <td><b>📬 Pull requests</b></td>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><a href="https://github.com/thmsgbrt/react-simple-pull-to-refresh"><b>React PullToRefresh component</b></a></td>
      <td><img alt="Stars" src="https://img.shields.io/github/stars/thmsgbrt/react-simple-pull-to-refresh?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Forks" src="https://img.shields.io/github/forks/thmsgbrt/react-simple-pull-to-refresh?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Issues" src="https://img.shields.io/github/issues/thmsgbrt/react-simple-pull-to-refresh?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Pull Requests" src="https://img.shields.io/github/issues-pr/thmsgbrt/react-simple-pull-to-refresh?style=flat-square&labelColor=343b41"/></td>
    </tr>
	  <tr>
      <td><a href="https://github.com/thmsgbrt/Chrome-Extension-with-React-and-Typescript-Starter-Pack"><b>Typescript & React Chrome Extension Starter</b></a></td>
      <td><img alt="Stars" src="https://img.shields.io/github/stars/thmsgbrt/Chrome-Extension-with-React-and-Typescript-Starter-Pack?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Forks" src="https://img.shields.io/github/forks/thmsgbrt/Chrome-Extension-with-React-and-Typescript-Starter-Pack?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Issues" src="https://img.shields.io/github/issues/thmsgbrt/Chrome-Extension-with-React-and-Typescript-Starter-Pack?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Pull Requests" src="https://img.shields.io/github/issues-pr/thmsgbrt/Chrome-Extension-with-React-and-Typescript-Starter-Pack?style=flat-square&labelColor=343b41"/></td>
    </tr>
    <tr>
      <td><a href="https://github.com/thmsgbrt/nodejs-typescript-express-apollo-graphql-starter"><b>NodeJs Express TypeScript GraphQL Starter</b></a></td>
      <td><img alt="Stars" src="https://img.shields.io/github/stars/thmsgbrt/nodejs-typescript-express-apollo-graphql-starter?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Forks" src="https://img.shields.io/github/forks/thmsgbrt/nodejs-typescript-express-apollo-graphql-starter?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Issues" src="https://img.shields.io/github/issues/thmsgbrt/nodejs-typescript-express-apollo-graphql-starter?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Pull Requests" src="https://img.shields.io/github/issues-pr/thmsgbrt/nodejs-typescript-express-apollo-graphql-starter?style=flat-square&labelColor=343b41"/></td>
    </tr>
  </tbody>
</table>
<h3>My latest posts</h3>
<ul>
  <li><a href="https://medium.com/better-programming/create-your-first-ethereum-smart-contract-with-remix-ide-667e46e81901"><b><img src="https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/240/apple/237/fire_1f525.png" width="20" alt="new" /> Create Your First Ethereum Smart Contract With Remix IDE</b></a><br/><i>Build a Blockchain-powered chat from your browser!.</i></li>
  <li><a href="https://medium.com/@th.guibert/how-to-create-a-self-updating-readme-md-for-your-github-profile-f8b05744ca91"><b><img src="https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/240/apple/237/fire_1f525.png" width="20" alt="new" /> How to Create a Self-Updating README.md for Your GitHub Profile</b></a><br/><i>A good tutorial to do your first steps with GitHub Actions</i></li>
    <li><a href="https://medium.com/better-programming/how-you-should-structure-your-react-applications-e7dd32375a98"><b><img src="https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/240/apple/237/fire_1f525.png" width="20" alt="new" /> How You Should Structure Your React Applications</b></a><br/><i>A matter of taste, sure, but here is an approach that scales.</i></li>
  <li><a href="https://medium.com/better-programming/pro-tips-to-help-you-get-started-with-your-side-project-15d01b76e0d8"><b>Pro Tips to Help You Get Started With Your Side Project</b></a><br/><i>Begin with solid foundations to keep the excitement kicking in...</i></li>
  <li><a href="https://medium.com/better-programming/how-to-take-care-of-your-personal-branding-as-a-programmer-2d3aeba56cb9"><b>How to Take Care of Your Personal Branding as a Programmer</b></a><br/><i>It’s more than just refreshing your resume</i></li>
  <li><a href="https://medium.com/better-programming/8-new-features-shipping-with-es2020-7a2721f710fb"><b>7 New Features Shipping With ES2020</b></a><br/><i>GlobalThis, optional chaining, private fields in classes, the nullish coalescing operator, and more</i></li>
</ul>
<h3>Välkommen till <img src="https://cdn-icons-png.flaticon.com/512/197/197564.png" width="13"/> Stockholm!</h3>
<p><img width="200" src="" /> <img width="200" src="" /> <img width="200" src="" /></p>
<p>Above are the last 3 pictures posted by <a href="https://www.instagram.com/visitstockholm/" target="_blank"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e7/Instagram_logo_2016.svg/1024px-Instagram_logo_2016.svg.png" width="20"/> @visitstockholm!</a><br/>Currently, the weather is: <b> 3°C, <i>overcast clouds</i></b></br>Today, the sun rises at <b>08:43</b> and sets at <b>14:47</b>.</p>
<h3>Where to find me</h3>
<p><a href="https://github.com/thmsgbrt" target="_blank"><img alt="Github" src="https://img.shields.io/badge/GitHub-%2312100E.svg?&style=for-the-badge&logo=Github&logoColor=white" /></a> <a href="https://twitter.com/Guibz16" target="_blank"><img alt="Twitter" src="https://img.shields.io/badge/twitter-%231DA1F2.svg?&style=for-the-badge&logo=twitter&logoColor=white" /></a> <a href="https://www.linkedin.com/in/thomas-guibert" target="_blank"><img alt="LinkedIn" src="https://img.shields.io/badge/linkedin-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white" /></a> <a href="https://medium.com/@th.guibert" target="_blank"><img alt="Medium" src="https://img.shields.io/badge/medium-%2312100E.svg?&style=for-the-badge&logo=medium&logoColor=white" /></a>
</p>

------------
<p align="center">This <i>README</i> file is generated <b>every 3 hours</b>!</br>Last refresh: Friday, 20 December, 01:03 CET<br /><a href="https://medium.com/@th.guibert/how-to-create-a-self-updating-readme-md-for-your-github-profile-f8b05744ca91">Create your own here!</a></p>
<p align="center"><img src="https://github.com/thmsgbrt/thmsgbrt/workflows/README%20build/badge.svg" /> <img alt="Stars" src="https://img.shields.io/github/stars/thmsgbrt/thmsgbrt?style=flat-square&labelColor=343b41"/> <img alt="Forks" src="https://img.shields.io/github/forks/thmsgbrt/thmsgbrt?style=flat-square&labelColor=343b41"/></p>













## Hi there 👋

<!--
**veffo/veffo** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->


Whoami 👤
Tools of Trade 🛠️
Experience 👨‍💼💼
Languages 📝🗣️
Volunteering 🙋‍♂️

## Table of contents
## Tools of Trade
- Web: Node.js, React.js, TailwindCSS
- Database: PostgreSQL, MySQL, MongoDB
- Containerization: Docker, Kubernetes, Rancher
- Cloud Computing: Digital Ocean, MVPS, Microsoft Azure, AWS
- CI/CD: TravisCI, CircleCI, Jenkins
- Scripting/Automation: Shell, CMD, Python, Ansible
- IAC: CloudFormation
- Server Administration: Linux, Windows, Nginx, Apache
- Computer Vision: Intel® OpenVINO Toolkit, OpenCV
- Artificial Intelligence: Microsoft Azure Studio

## Experience
My professional experience cuts across computer engineering, networking, systems administration and software development. See my Linkedin profile for more info.

## Languages
English (Professional)
Yoruba (Native)

<p align="center">
  <a href="https://getbootstrap.com/">
    <img src="https://getbootstrap.com/docs/5.3/assets/brand/bootstrap-logo-shadow.png" alt="Bootstrap logo" width="200" height="165">
  </a>
</p>

<h3 align="center">Bootstrap</h3>

<p align="center">
  Sleek, intuitive, and powerful front-end framework for faster and easier web development.
  <br>
  <a href="https://getbootstrap.com/docs/5.3/"><strong>Explore Bootstrap docs »</strong></a>
  <br>
  <br>
  <a href="https://github.com/twbs/bootstrap/issues/new?assignees=-&labels=bug&template=bug_report.yml">Report bug</a>
  ·
  <a href="https://github.com/twbs/bootstrap/issues/new?assignees=&labels=feature&template=feature_request.yml">Request feature</a>
  ·
  <a href="https://themes.getbootstrap.com/">Themes</a>
  ·
  <a href="https://blog.getbootstrap.com/">Blog</a>
</p>


## Bootstrap 5

Our default branch is for development of our Bootstrap 5 release. Head to the [`v4-dev` branch](https://github.com/twbs/bootstrap/tree/v4-dev) to view the readme, documentation, and source code for Bootstrap 4.


## Table of contents

- [Quick start](#quick-start)
- [Status](#status)
- [What's included](#whats-included)
- [Bugs and feature requests](#bugs-and-feature-requests)
- [Documentation](#documentation)
- [Contributing](#contributing)
- [Community](#community)
- [Versioning](#versioning)
- [Creators](#creators)
- [Thanks](#thanks)
- [Copyright and license](#copyright-and-license)


## Quick start

Several quick start options are available:

- [Download the latest release](https://github.com/twbs/bootstrap/archive/v5.3.3.zip)
- Clone the repo: `git clone https://github.com/twbs/bootstrap.git`
- Install with [npm](https://www.npmjs.com/): `npm install bootstrap@v5.3.3`
- Install with [yarn](https://yarnpkg.com/): `yarn add bootstrap@v5.3.3`
- Install with [Composer](https://getcomposer.org/): `composer require twbs/bootstrap:5.3.3`
- Install with [NuGet](https://www.nuget.org/): CSS: `Install-Package bootstrap` Sass: `Install-Package bootstrap.sass`

Read the [Getting started page](https://getbootstrap.com/docs/5.3/getting-started/introduction/) for information on the framework contents, templates, examples, and more.


## Status

[![Build Status](https://img.shields.io/github/actions/workflow/status/twbs/bootstrap/js.yml?branch=main&label=JS%20Tests&logo=github)](https://github.com/twbs/bootstrap/actions/workflows/js.yml?query=workflow%3AJS+branch%3Amain)
[![npm version](https://img.shields.io/npm/v/bootstrap?logo=npm&logoColor=fff)](https://www.npmjs.com/package/bootstrap)
[![Gem version](https://img.shields.io/gem/v/bootstrap?logo=rubygems&logoColor=fff)](https://rubygems.org/gems/bootstrap)
[![Meteor Atmosphere](https://img.shields.io/badge/meteor-twbs%3Abootstrap-blue?logo=meteor&logoColor=fff)](https://atmospherejs.com/twbs/bootstrap)
[![Packagist Prerelease](https://img.shields.io/packagist/vpre/twbs/bootstrap?logo=packagist&logoColor=fff)](https://packagist.org/packages/twbs/bootstrap)
[![NuGet](https://img.shields.io/nuget/vpre/bootstrap?logo=nuget&logoColor=fff)](https://www.nuget.org/packages/bootstrap/absoluteLatest)
[![Coverage Status](https://img.shields.io/coveralls/github/twbs/bootstrap/main?logo=coveralls&logoColor=fff)](https://coveralls.io/github/twbs/bootstrap?branch=main)
[![CSS gzip size](https://img.badgesize.io/twbs/bootstrap/main/dist/css/bootstrap.min.css?compression=gzip&label=CSS%20gzip%20size)](https://github.com/twbs/bootstrap/blob/main/dist/css/bootstrap.min.css)
[![CSS Brotli size](https://img.badgesize.io/twbs/bootstrap/main/dist/css/bootstrap.min.css?compression=brotli&label=CSS%20Brotli%20size)](https://github.com/twbs/bootstrap/blob/main/dist/css/bootstrap.min.css)
[![JS gzip size](https://img.badgesize.io/twbs/bootstrap/main/dist/js/bootstrap.min.js?compression=gzip&label=JS%20gzip%20size)](https://github.com/twbs/bootstrap/blob/main/dist/js/bootstrap.min.js)
[![JS Brotli size](https://img.badgesize.io/twbs/bootstrap/main/dist/js/bootstrap.min.js?compression=brotli&label=JS%20Brotli%20size)](https://github.com/twbs/bootstrap/blob/main/dist/js/bootstrap.min.js)
[![Backers on Open Collective](https://img.shields.io/opencollective/backers/bootstrap?logo=opencollective&logoColor=fff)](#backers)
[![Sponsors on Open Collective](https://img.shields.io/opencollective/sponsors/bootstrap?logo=opencollective&logoColor=fff)](#sponsors)


## What's included

Within the download you'll find the following directories and files, logically grouping common assets and providing both compiled and minified variations.

<details>
  <summary>Download contents</summary>

  ```text
  bootstrap/
  ├── css/
  │   ├── bootstrap-grid.css
  │   ├── bootstrap-grid.css.map
  │   ├── bootstrap-grid.min.css
  │   ├── bootstrap-grid.min.css.map
  │   ├── bootstrap-grid.rtl.css
  │   ├── bootstrap-grid.rtl.css.map
  │   ├── bootstrap-grid.rtl.min.css
  │   ├── bootstrap-grid.rtl.min.css.map
  │   ├── bootstrap-reboot.css
  │   ├── bootstrap-reboot.css.map
  │   ├── bootstrap-reboot.min.css
  │   ├── bootstrap-reboot.min.css.map
  │   ├── bootstrap-reboot.rtl.css
  │   ├── bootstrap-reboot.rtl.css.map
  │   ├── bootstrap-reboot.rtl.min.css
  │   ├── bootstrap-reboot.rtl.min.css.map
  │   ├── bootstrap-utilities.css
  │   ├── bootstrap-utilities.css.map
  │   ├── bootstrap-utilities.min.css
  │   ├── bootstrap-utilities.min.css.map
  │   ├── bootstrap-utilities.rtl.css
  │   ├── bootstrap-utilities.rtl.css.map
  │   ├── bootstrap-utilities.rtl.min.css
  │   ├── bootstrap-utilities.rtl.min.css.map
  │   ├── bootstrap.css
  │   ├── bootstrap.css.map
  │   ├── bootstrap.min.css
  │   ├── bootstrap.min.css.map
  │   ├── bootstrap.rtl.css
  │   ├── bootstrap.rtl.css.map
  │   ├── bootstrap.rtl.min.css
  │   └── bootstrap.rtl.min.css.map
  └── js/
      ├── bootstrap.bundle.js
      ├── bootstrap.bundle.js.map
      ├── bootstrap.bundle.min.js
      ├── bootstrap.bundle.min.js.map
      ├── bootstrap.esm.js
      ├── bootstrap.esm.js.map
      ├── bootstrap.esm.min.js
      ├── bootstrap.esm.min.js.map
      ├── bootstrap.js
      ├── bootstrap.js.map
      ├── bootstrap.min.js
      └── bootstrap.min.js.map
  ```
</details>

We provide compiled CSS and JS (`bootstrap.*`), as well as compiled and minified CSS and JS (`bootstrap.min.*`). [Source maps](https://web.dev/articles/source-maps) (`bootstrap.*.map`) are available for use with certain browsers' developer tools. Bundled JS files (`bootstrap.bundle.js` and minified `bootstrap.bundle.min.js`) include [Popper](https://popper.js.org/docs/v2/).


## Bugs and feature requests

Have a bug or a feature request? Please first read the [issue guidelines](https://github.com/twbs/bootstrap/blob/main/.github/CONTRIBUTING.md#using-the-issue-tracker) and search for existing and closed issues. If your problem or idea is not addressed yet, [please open a new issue](https://github.com/twbs/bootstrap/issues/new/choose).


## Documentation

Bootstrap's documentation, included in this repo in the root directory, is built with [Hugo](https://gohugo.io/) and publicly hosted on GitHub Pages at <https://getbootstrap.com/>. The docs may also be run locally.

Documentation search is powered by [Algolia's DocSearch](https://docsearch.algolia.com/).

### Running documentation locally

1. Run `npm install` to install the Node.js dependencies, including Hugo (the site builder).
2. Run `npm run test` (or a specific npm script) to rebuild distributed CSS and JavaScript files, as well as our docs assets.
3. From the root `/bootstrap` directory, run `npm run docs-serve` in the command line.
4. Open `http://localhost:9001/` in your browser, and voilà.

Learn more about using Hugo by reading its [documentation](https://gohugo.io/documentation/).

### Documentation for previous releases

You can find all our previous releases docs on <https://getbootstrap.com/docs/versions/>.

[Previous releases](https://github.com/twbs/bootstrap/releases) and their documentation are also available for download.


## Contributing

Please read through our [contributing guidelines](https://github.com/twbs/bootstrap/blob/main/.github/CONTRIBUTING.md). Included are directions for opening issues, coding standards, and notes on development.

Moreover, if your pull request contains JavaScript patches or features, you must include [relevant unit tests](https://github.com/twbs/bootstrap/tree/main/js/tests). All HTML and CSS should conform to the [Code Guide](https://github.com/mdo/code-guide), maintained by [Mark Otto](https://github.com/mdo).

Editor preferences are available in the [editor config](https://github.com/twbs/bootstrap/blob/main/.editorconfig) for easy use in common text editors. Read more and download plugins at <https://editorconfig.org/>.


## Community

Get updates on Bootstrap's development and chat with the project maintainers and community members.

- Follow [@getbootstrap on Twitter](https://twitter.com/getbootstrap).
- Read and subscribe to [The Official Bootstrap Blog](https://blog.getbootstrap.com/).
- Ask questions and explore [our GitHub Discussions](https://github.com/twbs/bootstrap/discussions).
- Discuss, ask questions, and more on [the community Discord](https://discord.gg/bZUvakRU3M) or [Bootstrap subreddit](https://www.reddit.com/r/bootstrap/).
- Chat with fellow Bootstrappers in IRC. On the `irc.libera.chat` server, in the `#bootstrap` channel.
- Implementation help may be found at Stack Overflow (tagged [`bootstrap-5`](https://stackoverflow.com/questions/tagged/bootstrap-5)).
- Developers should use the keyword `bootstrap` on packages which modify or add to the functionality of Bootstrap when distributing through [npm](https://www.npmjs.com/browse/keyword/bootstrap) or similar delivery mechanisms for maximum discoverability.


## Versioning

For transparency into our release cycle and in striving to maintain backward compatibility, Bootstrap is maintained under [the Semantic Versioning guidelines](https://semver.org/). Sometimes we screw up, but we adhere to those rules whenever possible.

See [the Releases section of our GitHub project](https://github.com/twbs/bootstrap/releases) for changelogs for each release version of Bootstrap. Release announcement posts on [the official Bootstrap blog](https://blog.getbootstrap.com/) contain summaries of the most noteworthy changes made in each release.


## Creators

**Mark Otto**

- <https://twitter.com/mdo>
- <https://github.com/mdo>

**Jacob Thornton**

- <https://twitter.com/fat>
- <https://github.com/fat>


## Thanks

<a href="https://www.browserstack.com/">
  <img src="https://live.browserstack.com/images/opensource/browserstack-logo.svg" alt="BrowserStack" width="192" height="42">
</a>

Thanks to [BrowserStack](https://www.browserstack.com/) for providing the infrastructure that allows us to test in real browsers!

<a href="https://www.netlify.com/">
  <img src="https://www.netlify.com/v3/img/components/full-logo-light.svg" alt="Netlify" width="147" height="40">
</a>

Thanks to [Netlify](https://www.netlify.com/) for providing us with Deploy Previews!


## Sponsors

Support this project by becoming a sponsor. Your logo will show up here with a link to your website. [[Become a sponsor](https://opencollective.com/bootstrap#sponsor)]

[![OC sponsor 0](https://opencollective.com/bootstrap/sponsor/0/avatar.svg)](https://opencollective.com/bootstrap/sponsor/0/website)
[![OC sponsor 1](https://opencollective.com/bootstrap/sponsor/1/avatar.svg)](https://opencollective.com/bootstrap/sponsor/1/website)
[![OC sponsor 2](https://opencollective.com/bootstrap/sponsor/2/avatar.svg)](https://opencollective.com/bootstrap/sponsor/2/website)
[![OC sponsor 3](https://opencollective.com/bootstrap/sponsor/3/avatar.svg)](https://opencollective.com/bootstrap/sponsor/3/website)
[![OC sponsor 4](https://opencollective.com/bootstrap/sponsor/4/avatar.svg)](https://opencollective.com/bootstrap/sponsor/4/website)
[![OC sponsor 5](https://opencollective.com/bootstrap/sponsor/5/avatar.svg)](https://opencollective.com/bootstrap/sponsor/5/website)
[![OC sponsor 6](https://opencollective.com/bootstrap/sponsor/6/avatar.svg)](https://opencollective.com/bootstrap/sponsor/6/website)
[![OC sponsor 7](https://opencollective.com/bootstrap/sponsor/7/avatar.svg)](https://opencollective.com/bootstrap/sponsor/7/website)
[![OC sponsor 8](https://opencollective.com/bootstrap/sponsor/8/avatar.svg)](https://opencollective.com/bootstrap/sponsor/8/website)
[![OC sponsor 9](https://opencollective.com/bootstrap/sponsor/9/avatar.svg)](https://opencollective.com/bootstrap/sponsor/9/website)


## Backers

Thank you to all our backers! 🙏 [[Become a backer](https://opencollective.com/bootstrap#backer)]

[![Backers](https://opencollective.com/bootstrap/backers.svg?width=890)](https://opencollective.com/bootstrap#backers)


## Copyright and license

Code and documentation copyright 2011–2024 the [Bootstrap Authors](https://github.com/twbs/bootstrap/graphs/contributors). Code released under the [MIT License](https://github.com/twbs/bootstrap/blob/main/LICENSE). Docs released under [Creative Commons](https://creativecommons.org/licenses/by/3.0/).








































# A collection of `.gitignore` templates

This is GitHub’s collection of [`.gitignore`][man] file templates.
We use this list to populate the `.gitignore` template choosers available
in the GitHub.com interface when creating new repositories and files.

For more information about how `.gitignore` files work, and how to use them,
the following resources are a great place to start:

- The [Ignoring Files chapter][chapter] of the [Pro Git][progit] book.
- The [Ignoring Files article][help] on the GitHub Help site.
- The [gitignore(5)][man] manual page.

[man]: http://git-scm.com/docs/gitignore
[help]: https://help.github.com/articles/ignoring-files
[chapter]: https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository#_ignoring
[progit]: http://git-scm.com/book

## Folder structure

We support a collection of templates, organized in this way:

- The root folder contains templates in common use, to help people get started
  with popular programming languages and technologies. These define a meaningful
  set of rules to help get started, and ensure you are not committing
  unimportant files into your repository.
- [`Global`](./Global) contains templates for various editors, tools and
  operating systems that can be used in different situations. It is recommended
  that you either [add these to your global template](https://docs.github.com/en/get-started/getting-started-with-git/ignoring-files#configuring-ignored-files-for-all-repositories-on-your-computer)
  or merge these rules into your project-specific templates if you want to use
  them permanently.
- [`community`](./community) contains specialized templates for other popular
  languages, tools and project, which don't currently belong in the mainstream
  templates. These should be added to your project-specific templates when you
  decide to adopt the framework or tool.

## What makes a good template?

A template should contain a set of rules to help Git repositories work with a
specific programming language, framework, tool or environment.

If it's not possible to curate a small set of useful rules for this situation,
then the template is not a good fit for this collection.

If a template is mostly a list of files installed by a particular version of
some software (e.g. a PHP framework), it could live under the `community`
directory. See [versioned templates](#versioned-templates) for more details.

If you have a small set of rules, or want to support a technology that is not
widely in use, and still believe this will be helpful to others, please read the
section about [specialized templates](#specialized-templates) for more details.

Include details when opening pull request if the template is important and visible. We
may not accept it immediately, but we can promote it to the root at a later date
based on interest.

Please also understand that we can’t list every tool that ever existed.
Our aim is to curate a collection of the _most common and helpful_ templates,
not to make sure we cover every project possible. If we choose not to
include your language, tool, or project, it’s not because it’s not awesome.

## Contributing guidelines

We’d love for you to help us improve this project. To help us keep this collection
high quality, we request that contributions adhere to the following guidelines.

- **Provide a link to the application or project’s homepage**. Unless it’s
  extremely popular, there’s a chance the maintainers don’t know about or use
  the language, framework, editor, app, or project your change applies to.

- **Provide links to documentation** supporting the change you’re making.
  Current, canonical documentation mentioning the files being ignored is best.
  If documentation isn’t available to support your change, do the best you can
  to explain what the files being ignored are for.

- **Explain why you’re making a change**. Even if it seems self-evident, please
  take a sentence or two to tell us why your change or addition should happen.
  It’s especially helpful to articulate why this change applies to _everyone_
  who works with the applicable technology, rather than just you or your team.

- **Please consider the scope of your change**. If your change is specific to a
  certain language or framework, then make sure the change is made to the
  template for that language or framework, rather than to the template for an
  editor, tool, or operating system.

- **Please only modify _one template_ per pull request**. This helps keep pull
  requests and feedback focused on a specific project or technology.

In general, the more you can do to help us understand the change you’re making,
the more likely we’ll be to accept your contribution quickly.

## Versioned templates

Some templates can change greatly between versions, and if you wish to contribute
to this repository we need to follow this specific flow:

- the template at the root should be the current supported version
- the template at the root should not have a version in the filename (i.e.
  "evergreen")
- previous versions of templates should live under `community/`
- previous versions of the template should embed the version in the filename,
  for readability

This helps ensure users get the latest version (because they'll use whatever is
at the root) but helps maintainers support older versions still in the wild.

## Specialized templates

If you have a template that you would like to contribute, but it isn't quite
mainstream, please consider adding this to the `community` directory under a
folder that best suits where it belongs.

The rules in your specialized template should be specific to the framework or
tool, and any additional templates should be mentioned in a comment in the
header of the template.

For example, this template might live at `community/DotNet/InforCRM.gitignore`:

```
# gitignore template for InforCRM (formerly SalesLogix)
# website: https://www.infor.com/product-summary/cx/infor-crm/
#
# Recommended: VisualStudio.gitignore

# Ignore model files that are auto-generated
ModelIndex.xml
ExportedFiles.xml

# Ignore deployment files
[Mm]odel/[Dd]eployment

# Force include portal SupportFiles
!Model/Portal/*/SupportFiles/[Bb]in/
!Model/Portal/PortalTemplates/*/SupportFiles/[Bb]in
```

## Contributing workflow

Here’s how we suggest you go about proposing a change to this project:

1. [Fork this project][fork] to your account.
2. [Create a branch][branch] for the change you intend to make.
3. Make your changes to your fork.
4. [Send a pull request][pr] from your fork’s branch to our `main` branch.

Using the web-based interface to make changes is fine too, and will help you
by automatically forking the project and prompting to send a pull request too.

[fork]: https://help.github.com/articles/fork-a-repo/
[branch]: https://help.github.com/articles/creating-and-deleting-branches-within-your-repository
[pr]: https://help.github.com/articles/using-pull-requests/

## License

[CC0-1.0](./LICENSE).




















# Hi [<img src="https://github.com/dlirA01/dlirA01/blob/main/wave.gif" width="28px"/>][youtube], I'm Arild or as i'm known on here, [Alien][youtube] [<img src="https://github.com/dlirA01/dlirA01/blob/main/wink-tounge.gif" width="28px"/>][youtube]

<br />

## Graphic designer, programmer & photographer

- 🌼 Currently studying digital media and design

<br />

## Connect with me

[<img src="https://github.com/dlirA01/dlirA01/blob/main/youtube.svg" height="12px"/>][youtube] [YouTube][youtube] &nbsp;&nbsp;
[<img src="https://github.com/dlirA01/dlirA01/blob/main/twitter.svg" height="12px"/>][twitter] [Twitter][twitter] &nbsp;&nbsp;
[<img src="https://github.com/dlirA01/dlirA01/blob/main/instagram.svg" height="12px"/>][instagram] [Instagram][instagram] &nbsp;&nbsp;
[<img src="https://github.com/dlirA01/dlirA01/blob/main/codepen.svg" height="12px"/>][codepen] [Codepen][codepen]

<br />
<br />

---

<details>
<summary>:star: Github Stats</summary>

  <br />
  
  <!-- start -->
  [![dlirA01's github stats](https://github-readme-stats.vercel.app/api?username=dlirA01&count_private=true&show_icons=true&theme=omni)](https://github.com/dlirA01/github-readme-stats)
  <!-- end -->

</details>

[youtube]: https://youtube.com/ArealAlien
[twitter]: https://twitter.com/Areal_Alien
[instagram]: https://instagram.com/areal_alien
[codepen]: https://codepen.io/areal_alien







<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains over 2000 video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.

## Laravel Sponsors

We would like to extend our thanks to the following sponsors for funding Laravel development. If you are interested in becoming a sponsor, please visit the Laravel [Patreon page](https://patreon.com/taylorotwell).

### Premium Partners

- **[Vehikl](https://vehikl.com/)**
- **[Tighten Co.](https://tighten.co)**
- **[Kirschbaum Development Group](https://kirschbaumdevelopment.com)**
- **[64 Robots](https://64robots.com)**
- **[Cubet Techno Labs](https://cubettech.com)**
- **[Cyber-Duck](https://cyber-duck.co.uk)**
- **[Many](https://www.many.co.uk)**
- **[Webdock, Fast VPS Hosting](https://www.webdock.io/en)**
- **[DevSquad](https://devsquad.com)**
- **[Curotec](https://www.curotec.com/services/technologies/laravel/)**
- **[OP.GG](https://op.gg)**
- **[WebReinvent](https://webreinvent.com/?utm_source=laravel&utm_medium=github&utm_campaign=patreon-sponsors)**
- **[Lendio](https://lendio.com)**

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
















<!--
repo name: Md-Template
description: An awesome readme Template extension to quickstart your project
github name:  oGranny
link: https://github.com/oGranny/readme-template-extension
logo path: assets/logo.png
screenshot: 
twitter: your_username
email: example@email.com
-->

<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
<!-- [![LinkedIn][linkedin-shield]][linkedin-url] -->



<!-- PROJECT LOGO -->
<br />
<p align="center">
    <a href="https://github.com/oGranny/readme-template-extension">
        <img src="icon.png" alt="Logo" width="80" height="80">
    </a>
<h3 align="center"><a href="https://github.com/oGranny/readme-template-extension">readme-template-extension</a></h3>
    <p align="center">
        An awesome readme Template extension to quickstart your project
        <br />
        <a href="https://marketplace.visualstudio.com/items?itemName=oGranny.md-template"><strong>Visual studio market place 📃</strong></a>
        <br />
        <br />
        <a href="//github.com/Md-Template/ oGranny">View Demo</a>
        •
        <a href="https://github.com/oGranny/readme-template-extension/issues">Report Bug</a>
        •
        <a href="https://github.com/oGranny/readme-template-extension/issues">Request Feature</a>
    </p>
</p>



<!-- TABLE OF CONTENTS -->
## Table of Contents

- [Table of Contents](#table-of-contents)
- [About The Project](#about-the-project)
  - [Built With](#built-with)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)



<!-- ABOUT THE PROJECT -->
## About The Project

There are many great README templates available on GitHub, however, I didn't find one that really suit my needs so I created this enhanced one. I want to create a README template so amazing that it'll be the last one you ever need.

Here's why:
* Your time should be focused on creating something amazing. A project that solves a problem and helps others
* You shouldn't be doing the same tasks over and over like creating a README from scratch
* You should element DRY principles to the rest of your life 😄:

Of course, no one template will serve all projects since your needs may be different. So I'll be adding more in the near future. You may also suggest changes by forking this repo and creating a pull request or opening an issue.

A list of commonly used resources that I find helpful are listed in the acknowledgements.

### Built With
* [yo]()
* [vsce]()


<!-- GETTING STARTED -->
## Getting Started
* Download the extension
* write `!!!` and click on the first option (make sure you are editing a markdown file)

### Prerequisites

* [VS Code](https://code.visualstudio.com)

### Installation

download this extension directly from VS code [marketplace](https://marketplace.visualstudio.com/vscode)



<!-- USAGE EXAMPLES -->
## Usage

vscode extension for github readme snippet to quick start your project



<!-- ROADMAP -->
## Roadmap

See the [open issues](https://github.com/oGranny/readme-template-extension/issues) for a list of proposed features (and known issues).



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.



<!-- CONTACT -->
## Contact

oGranny - ogranny.github.io@gmail.com

Project Link: [https://github.com/oGranny/readme-template-extension](https://github.com/oGranny/readme-template-extension)



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/oGranny/readme-template-extension.svg?style=flat-square
[contributors-url]: https://github.com/oGranny/readme-template-extension/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/oGranny/readme-template-extension.svg?style=flat-square
[forks-url]: https://github.com/oGranny/readme-template-extension/network/members
[stars-shield]: https://img.shields.io/github/stars/oGranny/readme-template-extension.svg?style=flat-square
[stars-url]: https://github.com/oGranny/readme-template-extension/stargazers
[issues-shield]: https://img.shields.io/github/issues/oGranny/readme-template-extension.svg?style=flat-square
[issues-url]: https://github.com/oGranny/readme-template-extension/issues
[license-shield]: https://img.shields.io/github/license/oGranny/readme-template-extension.svg?style=flat-square
[license-url]: https://github.com/oGranny/readme-template-extension/blob/master/LICENSE.txt
[product-screenshot]: images/screenshot.png



















<!--
**Ileriayo/ileriayo** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.
--->  

<h1 align="center"> 👋 </h1>
<div align="center">
  <img src="https://github.com/Ileriayo/ileriayo/blob/master/images/header.gif" alt="header"/>
</div>
<p align="center"> (Open for Hiring)</p>

<h2 align="center"> 👨‍💻 Whoami</h2>
<p align="center">
  <samp>A highly resourceful computer programmer and well-rounded IT professional with over five years of computing experience, possessing expert knowledge of the software development lifecycle and a solid understanding of technologies required for the development and deployment of highly available and scalable applications, including their networks and infrastructure.
  </samp>
  <br> <br>
  <img src="https://komarev.com/ghpvc/?username=ileriayo" alt="https://github.com/ileriayo" />
</p>

<hr>

<h2 align="center"> 🔭 Tools of Trade</h2>
<p align="center">
  <img src="https://img.shields.io/badge/node.js%20-%2343853D.svg?&style=for-the-badge&logo=node.js&logoColor=white" />&nbsp;&nbsp;&nbsp;
  <img src="https://img.shields.io/badge/react%20-%2300D9FF.svg?&style=for-the-badge&logo=react&logoColor=white" />&nbsp;&nbsp;&nbsp;
  <img src="https://img.shields.io/badge/tailwind-css%20-%231572B6.svg?&style=for-the-badge&logo=tailwind-css&logoColor=white" />&nbsp;&nbsp;
</p>
<p align="center">TailwindCSS, Python, Docker, Kubernetes, Rancher, TravisCI, Git, Github, Bitbucket, Apache, Nginx, Vagrant, Ansible, Jenkins, Azure.</p>

<hr>

<h2 align="center">💬 My Blog Articles</h2>
<p align="center" align='right'>
  <a target="_blank"href="https://dev.to/ileriayo"><img src="https://img.shields.io/badge/dev.to-%2312100E.svg?&style=for-the-badge&logo=dev.to&logoColor=white" /></a>&nbsp;&nbsp;&nbsp;
  <a target="_blank"href="https://medium.com/@ileriayoadebiyi"><img src="https://img.shields.io/badge/Medium%20-%231572B6.svg?&style=for-the-badge&logo=medium&logoColor=white" /></a>&nbsp;&nbsp;&nbsp;
</p>

<hr>

<h2  align="center">📫 Reach me on</h2>
<p align="center">
  <a target="_blank"href="https://www.linkedin.com/in/ileriayo-adebiyi-0328b1101/"><img src="https://img.shields.io/badge/linkedin-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white" /></a>&nbsp;&nbsp;&nbsp;&nbsp;
  <a target="_blank"href="https://twitter.com/ileriayooo"><img src="https://img.shields.io/badge/twitter-%231DA1F2.svg?&style=for-the-badge&logo=twitter&logoColor=white" /></a>&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="mailto:ileriayoadebiyi@gmail.com?subject=Hello%20Ileri,%20From%20Github"><img src="https://img.shields.io/badge/gmail-%23D14836.svg?&style=for-the-badge&logo=gmail&logoColor=white" /></a>&nbsp;&nbsp;&nbsp;&nbsp;
</p>

<hr>

<h2  align="center">💻 Check Out My Repos ⬇️ </h2>

















<p align="center"><a href="https://anuraghazra.github.io"><img width="80%" alt="Hello, I'm Anurag. I do open source!" src="./assets/gh-readme-header.png" /></a></p>

<br />

I'm a self-taught passionate FrontEnd developer from India 🇮🇳

**About me**

- 💼 FrontEnd Engineer at [Razorpay](http://razorpay.com/)

- 📈 Built github-readme-stats, verlyjs and more, **50m+** hits • **50K** stars on GitHub

- ❤️ I love writing TypeScript, and building fun experiments on type-level

- 💬 Ask me about anything [here](https://github.com/anuraghazra/anuraghazra/issues)

<code><img height="20" alt="javascript" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/javascript/javascript.png"></code>
<code><img height="20" alt="typescript" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/typescript/typescript.png"></code>
<code><img height="20" alt="react" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/react/react.png"></code>
<code><img height="20" alt="graphql" src="https://raw.githubusercontent.com/github/explore/5c058a388828bb5fde0bcafd4bc867b5bb3f26f3/topics/graphql/graphql.png"></code>
<code><img height="20" alt="nodejs" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/nodejs/nodejs.png"></code>    


| <a href="https://github.com/anuraghazra/github-readme-stats"><img align="center" src="https://github-readme-stats.vercel.app/api?username=anuraghazra&show_icons=true&include_all_commits=true&theme=buefy&hide_border=true" alt="Anurag's github stats" /></a> | <a href="https://github.com/anuraghazra/github-readme-stats"><img align="center" src="https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra&layout=compact&theme=buefy&hide_border=true" /></a> |
| ------------- | ------------- |

#### Top Repositories


<a href="https://github.com/anuraghazra/github-readme-stats">
  <img align="center" src="https://github-readme-stats.vercel.app/api/pin/?username=anuraghazra&repo=github-readme-stats&theme=buefy" />
</a>
<a href="https://github.com/anuraghazra/anuraghazra.github.io">
  <img align="center" src="https://github-readme-stats.vercel.app/api/pin/?username=anuraghazra&repo=anuraghazra.github.io&theme=buefy" />
</a>

<br />
<br />

<a href="https://twitter.com/anuraghazru">
  <img align="right" alt="Anurag Hazra | Twitter" width="21px" src="https://raw.githubusercontent.com/anuraghazra/anuraghazra/master/assets/twitter.svg" />
</a>
<a href="https://codesandbox.io/u/anuraghazra">
  <img align="right" alt="Anurag Hazra | CodeSandbox" width="20px" src="https://raw.githubusercontent.com/anuraghazra/anuraghazra/master/assets/codesandbox.svg" />
</a>
