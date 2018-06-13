<p align="center">
  <img alt="creativeshop" width="350" src="https://d3f8ubrix4l58h.cloudfront.net/static/frontend/Creativestyle/theme-creativeshop/en_US/images/creativeshop-logo.png">
</p>

_A Magento 2 extension escosystem providing UX/performance improvements and many new features._

This is a core metapackage which you should install in order to get creativeshop into your
Magento 2 setup.

Short video presentation of the __creative constructor__ feature:

<p align="center">
	<a href="https://vimeo.com/209752359">
  		<img width="350" src="https://i.vimeocdn.com/video/625378407.webp?mw=960&mh=540">
  	</a>
</p>

A demo installation showing the theme can be found [here](https://demo.creativeshop.io).

## Requirements

All of the packages require Magento 2.2.0+.

The whole ecosystem depends on [elasticsuite](http://elasticsuite.io/) and you need 
[elasticsearch](https://www.elastic.co/products/elasticsearch) in order to use it.

All of the frontend features and improvements are implemented in 
[theme-creativeshop](https://github.com/creativestyle/theme-creativeshop). 
You won't be able to take advantage of them if you use __Luma__ or other custom theme.

## Installation

* `composer require creativestyle/creativeshop ^1.0.0`
* Configure elasticsuite to use your elasticsearch installation
* Build the theme (next chapter)
* Switch theme to __Theme Creativeshop__

## Building theme-creativeshop

Creativeshop theme does not rely on Magento for building the assets, instead it uses *gulp*.

Before you start, make sure you have [nodejs](https://nodejs.org/en/) and 
[yarn](https://yarnpkg.com/lang/en/) installed.

__After__ the theme's composer package is installed to your Magento project, execute:

```bash
cd vendor/creativestyle/theme-creativeshop
yarn
yarn build
```

It will install the build artifacts into `app/design` subfolder.

After the theme is built, clear your Magento cache and you should be able to select it in admin.


Brought to life by<br/>
<a href="https://creativestyle.de">
	<img src="http://www.creativestyle.pl/wp-content/uploads/2014/04/CS-logo-red-creativestyle-gmbh-sp-z-o-o-interactive-agency-krakow-munchen-logo.png" width="150"/>
</a>