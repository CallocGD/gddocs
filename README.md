<div align="center">
    <img src="https://github.com/gd-programming/gddocs/blob/main/assets/gddocs-icon.png?raw=true" height="128" width="128" alt="book">
</div>

# GDDocs

**Some documentation for Geometry Dash's servers, and the game itself. This is a detached fork of GDDocs**

----

## Why I forked it 

- There are many things wrong with it even things that others should know about and it's more awful than you think just how much is being actually hidden from you
  and also broken enpoints due to that fact. =(
- loginGJAccount.php is just one example that I had to go in and fix. Many will soon follow as I discover more shit and problems within in gd's code.
- to develop a better gdpy library in the future and one that will acutally be healthy and have a better lifetime than the previous version
- Renamed parameters that are made to try and stop you from using certain endpoints. (I'm fixing that)
- I am Copying and pasting the urls into all documented enpoints where no code examples are being given (your welcome)


**GDDocs** is a project built to openly give advanced information and readable information for aspiring developers looking to interface with Geometry Dash. Primarily, we aim to create this as a website for people to learn more about the inner workings of geometry dash, along with it's data.

The GDDocs website can be found [here](https://wyliemaster.github.io/gddocs/#/)

## Running/Building
**You will require Node.js `>=12` to debug and run this project.**

GDDocs is built off of the `docsify` engine, outputted to a generator file to be able to work well on server environments, rather than GitHub pages. This is primarily to allow for easy domain usage and development in a place where it can always update, and be hosted upon locally rather than over GitHub's servers.

As such, rather than having to install using the package.json; (which we would recommended doing anyways using `npm install`,) the installation and such has been included in `generator.js`.

```plain
node generator.js
```

To debug it, you will need to properly clone or pull this repository.

## Contributing

Contributions are preferably made to the documentation, rather than the simple `generator.js` file; unless need be. Contributions to all aspects of this project are preferred to be made over pull requests and issues. Ideas on what to contribute or read over can be read in the [issues](https://github.com/gd-programming/gddocs/issues) section of this repository.

