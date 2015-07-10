# BrazilJS.org

[![Build Status](http://img.shields.io/travis/braziljs/braziljs.org/master.svg?style=flat)](https://travis-ci.org/braziljs/braziljs.org)
[![Dependency Status](http://img.shields.io/david/braziljs/braziljs.org.svg?style=flat)](https://david-dm.org/braziljs/braziljs.org)
[![DevDependencies Status](http://img.shields.io/david/dev/braziljs/braziljs.org.svg?style=flat)](https://david-dm.org/braziljs/braziljs.org#info=devDependencies)

![Cover](http://braziljs.org/img/projects/braziljsorg.jpg)

A non-profit foundation with a mission to move and unify JavaScript community in Brazil.

> **Maintainer:** [Diogo Moretti](https://github.com/diogomoretti)

## Contributing

There are tons of ways to contribute to this project.

###### Submit an event to [braziljs.org/eventos](http://braziljs.org/eventos/)

This is a list of all brazilian front-end conferences that happened or will
happen this year.

1. Edit the JSON file in [src/files/services/events](https://github.com/braziljs/foundation/tree/master/src/files/services/events).
2. Provide a thumbnail (227x200) in [src/files/services/events/media](https://github.com/braziljs/foundation/tree/master/src/files/services/events/media).

###### Submit a project to [braziljs.org/projetos](http://braziljs.org/projetos/)

1. Create a new HTML file named by name-of-project.html in [src/documents/projetos](https://github.com/braziljs/foundation/tree/master/src/documents/projetos) and fill with the code below changing for yours project infos.

  ```html
  ---
  title: "Title of project"
  description: "Description of project"
  site: "http://link-of-project.com.br"
  github: "your github link (after github.com)"
  image: "http://braziljs.org/img/projects/name-of-image-step2.jpg"
  ---

  <ul>
    <li><a href="http://myurl.com">Description of link</a></li>
    (Add new li>a node to create new links)
  </ul>
  ```

2. Provide a thumbnail (250x200) in [src/files/img/projects](https://github.com/braziljs/foundation/tree/master/src/files/img/projects).


## Dependencies

1. Install [Git](http://git-scm.com/download/), if you don't have it yet.
2. Install [NodeJS](http://nodejs.org/download/), if you don't have it yet.

## Setup

Once you have all [dependencies](#dependencies) installed, you just need to:

1. Open your terminal and clone the project.

  ```sh
  $ git clone git@github.com:braziljs/braziljs.org.git
  ```

2. Then go to the project's folder.

  ```sh
  $ cd braziljs.org
  ```

3. Initialize the submodules.

  ```sh
  $ git submodule update --init
  ```

4. And install local dependencies.

  ```sh
  $ npm install
  ```

## Usage

Execute the command below to generate the website into `out` directory:

```sh
$ npm run build
```

Generate and watch for any changes in `http://localhost:9778`:

```sh
$ npm run watch
```

Generate and deploy to [gh-pages branch](https://github.com/braziljs/braziljs.org/tree/gh-pages):

```sh
$ npm run deploy
```

## License

[MIT License](http://braziljs.mit-license.org/) © BrazilJS Foundation
