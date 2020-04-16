# Strapless-MHS

This is a custom fork of Strapless (http://www.strapless.io/). The same setup and other instructions 
found there apply equally here.

The generated CSS has been sourced to the repository so that it can be referenced as a dependency 
by downstream projects - using npm-assets (https://github.com/conradz/npm-assets). The command used: 

	npx lessc less/index.less css/strapless-f37d0b.css

Alternatively, all two dozen source .less files could be exposed for reference to be used for builds 
downstream. But, that seems tedious/unnecessary.

## Changelog

### 2020/04/16

Generate a custom property (CSS variable) for each generated color.

#### Before

	.color1 {
	  background-color: #F37D0B;
	  color: #0c0601;
	}

#### After

	.color1 {
	  background-color: #F37D0B;
	  color: #0c0601;
	}
	
	:root {
	  --color1: #F37D0B;
	}
