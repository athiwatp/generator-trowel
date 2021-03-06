![Friends of Trowel](https://raw.githubusercontent.com/Trowel/Trowel/master/media/dist/banners/friendsoftrowel-black-on-transparent.png)

# Trowel <%= props.names.capitalcase.plural %>
[![npm version](https://badge.fury.io/js/trowel-<%= props.name %>.svg)](https://badge.fury.io/js/trowel)
[![Bower version](https://badge.fury.io/bo/trowel-<%= props.name %>.svg)](https://badge.fury.io/bo/trowel-<%= props.name %>)

<%= props.description %>
<%= props.names.capitalcase.plural %> is a *Trowel Component*, please refer to the [Trowel doc](https://github.com/Trowel/Trowel/blob/master/doc/1-the-concept.md) for more informations about how works *Trowel Components*

## Getting Started
### Download
You can easily install *Trowel <%= props.names.capitalcase.plural %>* by using npm, Yarn or Bower

```bash
# With bower
$ bower install <%= props.packageName %>

# With npm
$ npm install <%= props.packageName %>

# With yarn
$ yarn add <%= props.packageName %>
```

You can also download a zip archive [right here](<%= props.url %>/archive/master.zip).

### Installation
#### *Scss*
The main scss file to include to your main `.scss` file is located at the `./<%= folders.src %>/scss/<%= props.names.kebabcase.plural %>.scss`. As a *Trowel Component*, it also requires two dependencies to compile the *scss* code. Here an *scss* installation snippet.

```
// Trowel Dependencies
@import './path/to/dependencies/trowel-core/src/trowel';

// Trowel Components <%= props.names.capitalcase.plural %>
@import './path/to/dependencies/<%= props.packageName %>/<%= folders.src %>/scss/<%= props.names.kebabcase.plural %>.scss';
```

#### *CSS*
If you don't want to customize the trowel component in `scss` you can use the css file available at `./<%= folders.dest %>/css/<%= props.names.kebabcase.plural %>.css`. A minified version is available at the same location.

<% if (props.javascript) { %>#### *JavaScript*
You have several javascript files for different use cases :
* The browser ready file is available at `./<%= folders.dest %>/javascript/<%= props.names.kebabcase.plural %>.js` (a minified version exists at `<%= folders.dest %>/javascript/<%= props.names.kebabcase.plural %>.min.js`)
* The script written in es2015 and ready to `import` is available at `./<%= folders.src %>/javascript/<%= props.names.kebabcase.plural %>.js`
<% } %>

<% if (props.twig) { %>#### *Twig template*
The twig template is located at the `./<%= folders.src %>/twig/<%= props.names.kebabcase.singular %>.html.twig`.<% } %>

## Usage
to be written

## Contributing
If you want to contribute you can checkout the contribution guide [over here](CONTRIBUTING.md)

## License
MIT © [Trowel](trowel.github.io)
