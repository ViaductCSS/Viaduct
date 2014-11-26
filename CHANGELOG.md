## 0.1.9
- Change ```_core.scss``` to ```_viaduct.scss```
- Fix issue to allow developers to use zero based spacing utilities. ```pad-0``` and ```mar-0``` should now work.
- Updated ```calc-em``` and ```calc-rem``` functions, as well as ```rem-sizing``` mixin to be able to take multiple values in their ```$values``` argument.
- Removed ```$from``` param from utilities media queries, to resolve issue where a single data attribute value will cascade down to all smaller viewports. Example - ```data-lap="position-relative"``` will result in just a max-width conditional being set so ```position: relative``` will apply to all viewports within the bounds of ```data-lap``` and ```data-palm```.

## 0.1.8
Removed 100% width from ```grid__item```. Recommendation is to use the ```1x``` utility.

## 0.1.7
Bug fix to change code tags in documentation to emphasis.

## 0.1.6
Continue with documentation. Start to add an example of how to use the architecture.

## 0.1.5
- Updates to commenting contained within the Viaduct Core code.
- Rewrite of Media Query mixin, to allow for additional extensibility. You can now provide both min and max widths/heights along with additional conditionals you would like to target.
- Changed ```media``` partial to ```embedded``` to prevent confusion.
- Removed ```fields``` border from normalise.
- Added private variables to each partial to enable feature toggling.
- Refactored ```rem-sizing``` mixin, to remove unnecessary ```!important``` tagging.
- Removed unnecessary ```!important``` from spacing generation mixins.
- Addition of utility classes as placeholder elements.
- Addition of ```is-visible``` class and placeholder within visibility partial.
- Removal of ```vendor``` directory and all containing partials.

## 0.0.4
Bug fix to remove special characters which were failing build for services internally at Clicksco.

## 0.0.3
Update to README to contain instruction on how to install Viaduct via Bower.

## 0.0.2
Addition of Viaduct Settings File. Also added a README file and began documentation.

## 0.0.1
Addition of Viaduct Core code
