# Strapless-MHS

This is a custom fork of Strapless (http://www.strapless.io/). The same setup and other instructions found there apply equally here.

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
