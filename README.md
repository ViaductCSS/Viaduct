## Viaduct CSS

The Viaduct CSS Framework is a scalable, modular codebase, written in Sass (SCSS).

The framework has been written with both OOCSS and BEM in mind, and particularly focuses on the separation of structure and skin within the UI. This is done by not coupling the styling to a certain aesthetic and building a library of utility classes mainly based on both the box model and formatting model to allow for the quick implementation of layout and prototyping.

Viaduct Core CSS Framework is written with the mobile first strategy in mind, and is completely responsive by default. It uses data attributes and name-spacing to apply styling to a specific set of breakpoints, which are completely customisable and allow for applications to scale very easily.

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