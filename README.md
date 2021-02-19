# Exploding Chickens

[![Build status](https://travis-ci.org/RAK3RMAN/exploding-chickens.svg?branch=main)](https://travis-ci.org/RAK3RMAN/exploding-chickens) ![Language](https://img.shields.io/badge/Language-Node.js-informational.svg?style=flat) ![License](https://img.shields.io/badge/License-MIT-red.svg)

A beautiful, online alternative to the popular kitty-powered version of Russian Roulette, Exploding Kittens. Exploding Chickens is a card game with explosions and of course, chickens — all crafted in the Node.js platform. The rules are simple. Each player takes turns drawing a card or playing a card, rolling the dice of luck so that they can survive for yet another turn. From there, the drawing deck slowly shrinks and the explosions only start to occur. **So, who will be the last one standing?**

- Supports up to **4-5 players**
- Utilizes a **52-card** base deck

##

<p align="center">
<img src="https://github.com/rak3rman/exploding-chickens/blob/main/public/cards/card_back.png?raw=true" width="100">
</p>

### Project under active development!

## Purpose & Structure
Exploding Chickens is an online alternative to the renowned Exploding Kittens card game that draws its strategy based off Russian Roulette. 
Players take turns drawing from a draw pile until someone draws a bit more explosion than they can chew.

## Install
As easy as 1, 2, 3..... boom.
1. Clone the repo and enter the directory: ``git clone https://github.com/rak3rman/exploding-chickens.git && cd exploding-chickens``
2. [Install a MongoDB instance](https://docs.mongodb.com/manual/installation/#mongodb-community-edition-installation-tutorials) locally or point to your own (more in usage)
3. Install packages and run: ``npm install``, ``npm run start``

## Usage
### Configuration
After the first run of exploding-chickens, a config file will be created in the config folder with path ``/config/config.json``. 
This file stores all the environment variables needed for the project, which can be edited when the instance is not running.
The config file will be populated with the following default values:
- ``"webserver_port": 3000`` Port where the webserver will accept incoming connections, of type int
- ``"mongodb_url": "mongodb://localhost:27017/exploding-chickens"`` The url of your mongodb instance (make sure to add "/exploding-chickens" at the end of the url), of type string
- ``"verbose_debug_mode": false`` Whether to output verbose debug output, of type bool

**NOTE:** Make sure to stop the instance of exploding-chickens before changing any of these values. If the file is modified while an instance is active, the changes will be overridden.

### Running the project
The npm package supports multiple ways to run the project.
- ``npm run start`` Runs the project, plain and simple.
- ``npm run develop`` Runs the project and watches for all file changes. Restarts the instance if critical files are updated.
- ``npm run test`` Runs a test suite built using [mocha](https://mochajs.org/), tests can be found in path ``/test`` . Travis-CI also runs these tests.
- ``npm run production`` **UNDER DEVELOPMENT**

Use ``^C`` to exit any of these instances. Currently, there are no exit commands or words.

## Development
Communal development is a key part of this project.
As we all try to make this project the best we can, please adhere to the following style guidelines:
- Preface all text files with the following header comment. If you are editing an item within the file, please add your name to the author section if the contribution was beyond a stylistic nature.
```
/*\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\
Filename : exploding-chickens/services/file.js
Desc     : a couple lines (1-3+) about the purpose of
           the file and what it does
Author(s): RAk3rman
\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\*/
```
- Preface all portions of code with the following header comment. If you are editing a code block, please add your name to the author section if the contribution was beyond a stylistic nature.
```
// Name : global_path.function_name(param1, param2)
// Desc : a brief 1-2 line description
// Author(s) : RAk3rman
```
- Please use underscore separated function names (ex. my_function_is_awesome).
- Make sure in line comments are clear. Use good coding practices...

## Contributors
- **Radison Akerman** / Project Manager
- **Sengdao Inthavong** / Front-end Designer
- **Vincent Do** / Back-end Developer
- **Richard Yang** / Back-end Developer
- **Evan Carlson** / Code Review

*Individual contributions are listed on most functions, for reference*
## License
This project (exploding-chickens) is protected by the MIT License as disclosed in the [LICENSE](https://github.com/rak3rman/exploding-chickens/blob/main/LICENSE). You must adhere to the policies and terms listed. Copyright (c) 2020-2021 Radison Akerman
