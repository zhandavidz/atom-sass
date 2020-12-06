# scss-compiler: A SCSS Compiler for Atom

[![apm](https://img.shields.io/apm/v/scss-compiler.svg?maxAge=2592000)](https://atom.io/packages/scss-compiler)
[![apm](https://img.shields.io/apm/dm/scss-compiler.svg?style=flat-square)](https://atom.io/packages/scss-compiler)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/zhandavidz/scss-compiler/master/LICENSE.md)

`scss-compiler` is based on sass Ruby gem. This project is forked from [rehrumesh's atom-sass](https://github.com/rehrumesh/atom-sass) project, and this project draws the majority of the code from that project. Most of this work in [rehrumesh's atom-sass](https://github.com/rehrumesh/atom-sass) project is based on [GomatoX's sass-compile](https://github.com/GomatoX/sass-compiler) project. Huge thanks to both of them for coming up with the initial projects.

## Where do the compiled files go?

This was one reason why I forked the original repo. In this project, proper organization will mean that your `.scss` file should be in a directory, preferably named `sass` or `scss`, and the compiler will go to the parent folder and put the compiled `.css` file in a folder named `css` in the parent directory. In other words, it should look like this:
```
parent-folder:
  ↳ sass
      ↳ files to be compiled
  ↳ css
      ↳ location of compiled files
```

## Dependencies
* Sass Ruby gem https://rubygems.org/gems/sass/versions/3.4.22

To install this dependency, execute `gem install sass`

## Installation

Use atom package manager to install atom-sass.

`apm install scss-compiler`

## Usage

* Open the editor.
  * If you have already installed the package, it should begin automatically. You should see the green notification `Now watching for SASS files`. If you do not, or if you have just installed the package, you may have to do one of the following:
    * reload the editor: `ctrl+shift+F5`
    * start the compiler: `Packages -> SCSS Compiler -> Start Compiler` OR `ctrl+alt+c`
* When editing `.scss` files, whenever you save a changed file, a compiled one should appear.



<!-- ![image](https://cloud.githubusercontent.com/assets/2035004/17414920/18ac3db6-5aa5-11e6-8604-60570794b2ee.png)

* Open any sass file which has `.scss` extension.
* Press `Alt + Ctrl + c` to watch the files for changes.
* Upon modification save, it will automatically compile the scss file and generate `.css` file. -->

## License
  [MIT](LICENSE)
