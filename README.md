# ClaySS

ClaySS is the iotaCSS framework, along with some customizationized settings and components.

The purpose of ClaySS is to provide predefined styling, which can be customized from the entry file you use to compile. ClaySS heaviy uses variables, intended to give you as many options as possible within the current components. ClaySS is the CSS framework used within the (currently proprietary) Clay CMS, but released separately as a standalone product.

### Installation

Note: This is not required within Clay, only if being used outside of Clay

`npm install`

The iotaCSS framework will be installed, as it is the only dependency.

## Required Variables and Settings

ClaySS allows you to override the pre-compiled styling using variables. It also requires you to provide some variables, which are not defined with ClaySS.

The minimum requirements are already in the clayss.scss file.

### Compiling

Node command when used within a Clay theme:

`node-sass main.scss main.css --output-style compressed --include-path ../../.sass`

Live reload (on file change):

`node-sass main.scss main.css --output-style compressed --include-path ../../.sass -w`

ClaySS can also be used without Clay. Simply update clayss.scss as needed and compile it with:

`node-sass clayss.scss main.css`

### Preview

ClaySS is packaged with a preview.html file and a precompiled main.css file. The preview is a work in progress, but gives you an idea of how the styling appears and how your changes affect it.
