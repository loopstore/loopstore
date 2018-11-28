---
id: get-started-google-cloud-shell
summary: In this how-to we'll find out how to set up a development environment for our LoopStore purely in the cloud. You can then follow the tutorial from with the Cloud Shell.
status: [draft]
author: LoopStore
categories: LoopBack,Google Cloud Shell
tags: cloudant,gcs,google cloud shell,graphql,ibm cloud,loopback,loopstore,node,openapi,rest
feedback link: https://github.com/loopstore/loopstore-tutorial-v4/issues

---

# Get Started using Google Cloud Shell

[Codelab Feedback](https://github.com/loopstore/loopstore-tutorial-v4/issues)


## Introduction
Duration: 01:00



## Install the LoopBack4 CLI and create our LoopStore app
Duration: 02:00


<aside class="special">

**We're assuming:**

You're running Node.js in a unix environment. In the tutorial **Reference Section** you can find out how to Install Node.js and npm with Node Version Manager. 
</aside>

### What you'll learn

* **How to:** check your  [Node.js](https://nodejs.org) environment supports  [LoopBack 4](https://v4.loopback.io/)
* **How to**: install the  [LoopBack 4](https://v4.loopback.io/) CLI
* **How to**: create a  [LoopBack 4](https://v4.loopback.io/) Application using the CLI Generator
* **How to**: Build and run the app
* **Key Concepts**: CLI, Application, Generator, Build

### Instructions

#### Install the  [LoopBack 4](https://v4.loopback.io/) CLI  [npm package](https://www.npmjs.com/package/@loopback/cli)

    npm i -g @loopback/cli

#### Start the app generator using the "lb4 app" command
[see all CLI options](https://github.com/strongloop/loopback-next/blob/master/packages/cli/README.md)

    lb4 app

#### For "Project name" enter "loopstore"

    loopstore

#### For Project description enter "Building a store with LoopBack 4"

    Building a store with LoopBack 4

#### For "Project root directory" enter "loopstore"

    loopstore

<aside class="special">

**Hint**

This is the name of the directory which will be created below your current working directory to store our LoopStore's code package. This will also be the package name contained in the app package.json file.
</aside>

**Caution!**

You can't enter a path here: see  [this Issue](https://github.com/strongloop/loopback-next/issues/2092).

#### For "Application class name" enter "LoopstoreApplication"

    LoopstoreApplication

#### Leave all the features enabled

<aside class="special">

**Going deeper 🤓**

Here's what we enabling: tslint, prettier, Eable mocha, loopbackBuild, vscode, repositories, services.

We'll be looking into what these all mean later in the tutorial.
</aside>

#### Generate the LoopStore app

**Hit Enter to create the LoopStore!**

After a few seconds, the code for the LoopStore app should be generated in in a subfolder called loopstore.

#### Change into the app code directory using "cd loopstore"

    cd loopstore

#### Build a run the LoopStore app using "npm start"

    npm start

NPM will run the build scripts in the <walkthrough-editor-open-file  filePath="test-cloudshell-tutorial/loopstore/package.json" text="">package.json</walkthrough-editor-open-file> file

```
> loopstore@1.0.0 prestart /home/nigel/loopstore/loopstore
> npm run build
> loopstore@1.0.0 build /home/nigel/loopstore/loopstore
> lb-tsc es2017 --outDir dist> loopstore@1.0.0 start /home/nigel/loopstore/loopstore
```

<aside class="special">

**Going deeper**

If you look closely the **npm start** script actually runs a **prestart** script, which runs the **build **script before finally serving the app. We'll have to change some of these settings and look deeper into the LoopBack **Build **package later.
</aside>

#### That's it!

```
> node .Server is running at http://127.0.0.1:3000
Try http://127.0.0.1:3000/ping
```

Our LoopStore is up and running! (kind of). It's pretty unlikely you won't have checked out those links in the browser yet but we'll be having a look at what exactly we've created and how it works next up...

### Frequently Asked Questions

*  [LoopBack 4 Issues on GitHub](https://github.com/strongloop/loopback-next/issues)


## Deploying our LoopStore to IBM Cloud Free Tier
Duration: 10:00


####  [Deploying Loo](http://how-to-labs_deploy_to_ibm_cloud) [pStore to IBM Cloud Free Tier](http://how-to-labs_deploy_to_ibm_cloud)


## Reference and Further Reading




## Install Node.js and npm with Node Version Manager



<aside class="special">

**We're assuming:**

You're running a recent version of Linux or MacOS and comfortable with using the command line in a   [bash shell](https://en.wikipedia.org/wiki/Bash_(Unix_shell)). 
</aside>

### What you'll learn

* **How to:** install and manage the   [Node.js](https://nodejs.org) environment and  [Node Package Manager (npm)](https://www.npmjs.com) using  [Node Version Manager (nvm)](https://github.com/creationix/nvm)
* **How to**: install and use different versions 

### Instructions

#### Check the  [creationix/nvm](https://github.com/creationix/nvm) GitHub repo for  [latest nvm release](https://github.com/strongloop/loopback-next/blob/master/packages/cli/README.md)

Here we'll be using  [v0.33.11](https://github.com/creationix/nvm/releases/tag/v0.33.11) 

#### Download the nvm install script via cURL

    curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh | bash

#### Check nvm is installed by running **nvm --version**

    nvm --version

nvm --version
0.33.11

#### For **Description** enter **A store built with LoopBack 4**

    A store built with LoopBack 4

#### For **project directory** enter **loopstore**

loopstore

<aside class="special">

**Best Practices**

This is the name of the directory which will be created below your current working directory to store our LoopStore's code
</aside>

#### Change into the package directory

cd package

#### Start the app 

#### Using npm start

npm start

### Frequently Asked Questions

*  [nvm questions on Stack Overflow](https://stackoverflow.com/search?q=NVM)


## LoopBack 4 Best Practices




## LoopBack 4 Key Concepts




## All LoopStore How-To Labs



####  [Deploying LoopStore to IBM Cloud Free Tier](http://how-to-labs_deploy_to_ibm_cloud)


