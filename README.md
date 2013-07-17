# asset

> The best project ever.

## Getting Started
Before anything taking its part, you should install [node](http://nodejs.org) and "cortex".

#### Install Node

Visit [http://nodejs.org](http://nodejs.org), download and install the proper version of nodejs.

#### Install Cortex

    # maybe you should use `sudo`
    npm install -g cortex

## Using asset In Your Project

First, install 'asset' directly with `ctx install` (recommended)
	
	ctx install asset --save
	
or, you could update your package.json manually
    
    dependencies: {
        'asset': '<version-you-want>'
    }
    
and install dependencies
	
	ctx install
    
Then, use `require` method in your module
    
    var asset = require('asset');
    
Finally, start cortex server
    
    ctx server
    
Then cortex will care all the rest.


## API Documentation

### asset: constructor
': constructor' means the `module.exports` of module 'asset' is a constructor that we should use it with the `new` keyword

	new asset(options)
	
#### options
- options.name {String}



### asset.\<method-name\>(arguments)
Means this is a static method of `module.exports`

#### arguments
// arguments description here

### .\<method-name\>(arguments)
Mean this is a method of the instance

#### arguments
// arguments description here