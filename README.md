### Key Facts
- LLM Orchestrator AGPL licensed (to use as custom-label SaaS, contributing back)
- True community governance
- No single corporate control 
- 5+ years of stability
- Never changed license
- Enterprise-grad
- Hosted locally or Multicloud

## Contributors

<a href="https://github.com/generalbots/botserver/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=generalbots/botserver" />
</a>

## Overview

| Area                         | Status                                                                                             |
|------------------------------|----------------------------------------------------------------------------------------------------|
| Releases                     | [![General Bots](https://img.shields.io/npm/dt/botserver.svg?logo=npm&label=botserver)](https://www.npmjs.com/package/botserver/) [![.gbapp lib](https://img.shields.io/npm/dt/botlib.svg?logo=npm&label=botlib)](https://www.npmjs.com/package/botlib/) [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)|
| Community                    | [![StackExchange](https://img.shields.io/stackexchange/stackoverflow/t/generalbots.svg)](https://stackoverflow.com/search?q=%23generalbots&s=966e24e7-4f7a-46ee-b159-79d643d6b74a)  [![Open-source](https://badges.frapsoft.com/os/v2/open-source.svg)](https://badges.frapsoft.com) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) [![License](https://img.shields.io/badge/license-AGPL-blue.svg)](https://github.com/GeneralBots/BotServer/blob/master/LICENSE.txt)|
| Management                   | [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://gitHub.com/GeneralBots/BotServer/graphs/commit-activity) |
| Security                     | [![Known Vulnerabilities](https://snyk.io/test/github/GeneralBots/BotServer/badge.svg)](https://snyk.io/test/github/GeneralBots/BotServer) |
| Building & Quality           |  [![Coverage Status](https://coveralls.io/repos/github/GeneralBots/BotServer/badge.svg)](https://coveralls.io/github/GeneralBots/BotServer) [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier) |
| Packaging                    | [![forthebadge](https://badge.fury.io/js/botserver.svg)](https://badge.fury.io) [![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/) |
| Samples                      | [BASIC](https://github.com/GeneralBots/BotServer/tree/master/packages/default.gbdialog) or [![TypeScript](https://badges.frapsoft.com/typescript/code/typescript.svg?v=101)](https://github.com/GeneralBots/AzureADPasswordReset.gbapp)
| [Docker Image](https://github.com/lpicanco/docker-botserver)  ![Docker Pulls](https://img.shields.io/docker/pulls/lpicanco/botserver.svg) <br/> *Provided by [@lpicanco](https://github.com/lpicanco/docker-botserver)* |

# General Bots

![General Bot Logo](https://github.com/GeneralBots/BotServer/blob/main/logo.png?raw=true))

General Bot is a strongly typed LLM conversational platform package based chat bot server focused in convention over configuration and code-less approaches, which brings software packages and application server concepts to help parallel bot development.

## What is a Bot Server?

Bot Server accelerates the process of developing a bot. It provisions all code
base, resources and deployment to the cloud, and gives you templates you can
choose from whenever you need a new bot. The server has a database and service 
backend allowing you to further modify your bot package directly by downloading 
a zip file, editing and uploading it back to the server (deploying process) with 
no code. The Bot Server also provides a framework to develop bot packages in a more
advanced fashion writing custom code in editors like Visual Studio Code, Atom or Brackets.

Everyone can create bots by just copying and pasting some files and using their
favorite tools from Office (or any text editor) or Photoshop (or any image
editor). LLM and BASIC can be mixed used to build custom dialogs so Bot can be extended just like VBA for Excel.

## Getting Started

### Prerequisites

Before you embark on your General Bots journey, ensure you have the following tools installed:

- **Node.js (version 20 or later)**: General Bots leverages the latest features of Node.js to provide a robust and efficient runtime environment. Download it from [nodejs.org](https://nodejs.org/en/download/).
- **Git (latest stable version)**: Essential for version control and collaborating on bot projects. Get it from [git-scm.com](https://git-scm.com/downloads).

### Quick Start Guide

Follow these steps to get your General Bots server up and running:

1. Clone the repository:
   ```bash
   git clone https://github.com/GeneralBots/BotServer
   ```
   This command creates a local copy of the General Bots server repository on your machine.

2. Navigate to the project directory:
   ```bash
   cd BotServer
   ```
   This changes your current directory to the newly cloned BotServer folder.

3. Install dependencies and start the server:
   ```bash
   npm install
   npm run start
   ```
   The `npm install` command installs all necessary dependencies for the project. `npm run start` builds your bot server locally and serves it through a development server.

### Accessing Your Bot

Once the server is running, you can access your bot at `http://localhost:4242/`. This local server allows you to interact with your bot and test its functionality in real-time. If you want to publish
without password, define [ADMIN_OPEN_PUBLISH](https://github.com/GeneralBots/BotBook/master/docs/chapter-07-gbot-reference#enviroment-variables-reference) as true in BotServer .env file.

To publish bot packages and initiate a conversation with the bot, use the command:

```
/publish
```
This command prepares your bot packages for use and allows you to start interacting with your bot immediately.

## Development Workflow

### 1. Project Structure

The General Bots server follows a modular architecture designed for flexibility and scalability. Here's an overview of the main directories:

```
BotServer/
├── packages/
│   ├── core.gbapp/         # Core bot functionality
│   ├── kb.gbapp/           # Knowledge base packages
├── src /             # Main entry point
└── package.json      # Project configuration
```

This structure allows for easy navigation and management of different aspects of your bot project.

### 2. Creating Custom Packages

One of the strengths of General Bots is its extensibility. You can create custom packages to enhance your bot's capabilities:

- **.gbkb (Knowledge Base packages)**: Store and manage your bot's knowledge and responses.
- **.gbtheme (Theme packages)**: Customize the visual appearance of your bot interface.
- **.gbapp (Application packages)**: Add new features and functionalities to your bot.

Each package type has its own structure and purpose, which we'll explore in depth in their respective chapters.

## Samples

Several samples, including a Bot for AD Password Reset, are avaiable on the [repository list](https://github.com/GeneralBots).

### Using complete General Bots Conversational Data Analytics

![](https://user-images.githubusercontent.com/14840374/178154826-8188029e-b4f4-48aa-bc0d-126307ce5121.png)

```
TALK  "General Bots Labs presents FISCAL DATA SHOW BY BASIC" 

TALK "Gift Contributions to Reduce the Public Debt API (https://fiscaldata.treasury.gov/datasets/gift-contributions-reduce-debt-held-by-public/gift-contributions-to-reduce-the-public-debt)" 
 
result = GET "https://api.fiscaldata.treasury.gov/services/api/fiscal_service/v2/accounting/od/gift_contributions?page[size]=500" 
data = result.data 
data = SELECT YEAR(record_date) as Yr, SUM(CAST(contribution_amt AS NUMBER)) AS Amount FROM data GROUP BY YEAR(record_date) 

TALK "Demonstration of Gift Contributions with AS IMAGE keyword" 
SET THEME dark 
png = data as IMAGE  
SEND FILE png 

DELAY 5 
TALK " Demonstration of Gift Contributions CHART keyword" 
 img = CHART "bar", data  
SEND FILE img 
```

## Guide

[Read the General Bots BotBook Guide](https://docs.pragmatismo.cloud)

# Videos

 7 AI General Bots LLM Templates for Goodness
 [https://www.youtube.com/watch?v=KJgvUPXi3Fw](https://www.youtube.com/watch?v=KJgvUPXi3Fw)
  
# Contributing

This project welcomes contributions and suggestions. 
See our [Contribution Guidelines](https://github.com/pragmatismo-io/BotServer/blob/master/CONTRIBUTING.md) for more details.

# Reporting Security Issues

Security issues and bugs should be reported privately, via email, to the pragmatismo.cloud Security
team at [security@pragmatismo.cloud](mailto:security@pragmatismo.cloud). You should
receive a response within 24 hours. If for some reason you do not, please follow up via
email to ensure we received your original message. 

# License & Warranty

General Bot Copyright (c) pragmatismo.cloud. All rights reserved.
Licensed under the AGPL-3.0.       
                                                            
According to our dual licensing model, this program can be used either
under the terms of the GNU Affero General Public License, version 3,
or under a proprietary license.   
                                                        
The texts of the GNU Affero General Public License with an additional
permission and of our proprietary license can be found at and 
in the LICENSE file you have received along with this program.
                                                       
This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU Affero General Public License for more details.
                                                        
"General Bot" is a registered trademark of pragmatismo.cloud.
The licensing of the program under the AGPLv3 does not imply a
trademark license. Therefore any rights, title and interest in
our trademarks remain entirely with us.

<a href="https://stackoverflow.com/questions/ask?tags=generalbots">:speech_balloon: Ask a question</a> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <a href="https://github.com/GeneralBots/BotBook">:book: Read the Docs</a>
Team pictures made with [contrib.rocks](https://contrib.rocks).
General Bots Code Name is [Guaribas](https://en.wikipedia.org/wiki/Guaribas), the name of a city in Brazil, state of Piaui.
[Roberto Mangabeira Unger](http://www.robertounger.com/en/): "No one should have to do work that can be done by a machine".
