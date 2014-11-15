## Viaduct CSS

The Viaduct CSS Framework is a scalable, modular codebase, written in Sass (SCSS).

The framework has been written with both OOCSS and BEM in mind, and particularly focuses on the separation of structure and skin within the UI. This is done by not coupling the styling to a certain aesthetic and building a library of utility classes mainly based on both the box model and formatting model to allow for the quick implementation of layout and prototyping.

Viaduct Core CSS Framework is written with the mobile first strategy in mind, and is completely responsive by default. It uses data attributes and name-spacing to apply styling to a specific set of breakpoints, which are completely customisable and allow for applications to scale very easily.

*We would like to say a special thanks to both [Harry Roberts](https://github.com/csswizardry) & [Nicolas Gallagher](https://github.com/necolas) for their work across multiple projects including [Inuit](https://github.com/inuitcss), [Suit](https://github.com/suitcss/suit) and [Normalize](https://github.com/necolas/normalize.css) to name a few. Viaduct is heavily influenced and uses a lot of techniques specified in these great frameworks and libraries*

### Installation

To use Viaduct, you can either clone this repository, or use the Bower package manager and request the version you require.

#### Bower

To install Viaduct via Bower, it is a case of running a single command of

```bower install viaduct-css```

This will pull the latest version which is stored on the Bower servers. To install a specific release, you can prefix the package name with the release you require, like so;

```bower install viaduct-css#0.0.1```

Once you pull the files, bower will create a ```bower_components``` directory, which will store all of the packages you have installed. You can change where Bower installs its packages by editing the ```.bowerrc``` file. You can find more information about Bower and its configuration settings at [bower.io](http://www.bower.io).

When your packages are stored in the directory of your choice, it is a case of using ```@import``` statements within your primary ```.scss``` for both the ```_settings.scss``` and ```_core.scss``` partials.

**Note - It is required, that you import Viaduct's settings file before the core framework itself, as all default variable values are stored in this file.**

## Why use Viaduct?

Viaduct’s code is **not** the main focus of the framework. The main focus of building Viaduct is to create a project structure and architecture which is maintainable, understandable to developers of any level and highly scalable, as well to make working on RWD projects easier via data attributes.

In a world where web standards is moving so quickly and technologies are allowing developers to produce things on the client which people didn’t think was possible, we all seem to have forgot about project structure.

Before we created Viaduct, we reviewed a lot of existing frameworks and libraries, and three issue’s seemed to arise every time:

- **Flat project structure** (usually frameworks had files in one folder)
- **Extensibility** - Frameworks were being extended by developers by modifying the framework itself and building on top of it. This makes versioning virtually impossible.
- **Naming Conventions** - Directory/file naming conventions seemed overly complex or related to scientific elements which didn’t reflect the contents. To understand where a new file or piece of code should be stored, you had to read articles. This is un-necessary.

### Viaduct is born

I ([Ben](https://github.com/Passenger-Inspired)) was sitting at [Industry Conf](http://2015.industryconf.com/) watching a brilliant talk from Harry entitled [“What is a CSS framework anyway”](http://vimeo.com/95734680). This was a huge lightbulb moment, and listening to Harry talk about the differences between a CSS framework and a UI framework, and how things should be separated, brought me to the following. **A framework should be built in layers**

Viaduct is considered to be the Core layer in your CSS project. To extend or modify Viaduct, you should create a layer/s which mirror the directory/file structure contained in Viaduct and add your changes.

#### An Example

The above description works best as an example, so let's jump in and go through this step by step.
