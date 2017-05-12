
## Installation

First you need to install react-native-banner:

```javascript
npm install react-native-banner --save

```
##  Properties

name | description
banners | PropTypes.**array**.isRequired,including all the resources like images and title that the banner need
defaultIndex | PropTypes.**num**, the default index that the banner begins
intent  | PropTypes.**func**, the func actives when you click the banner
onMomentumScrollEnd | PropTypes.**func**, the func actives when the banner played the last image

The elements of the array banners are supposed to have the two properties named title and image as an object

## Usage

```javascript
import Banner from 'react-native-banner';

<Banner
    banners={this.banners}
    defaultIndex={this.defaultIndex}
    onMomentumScrollEnd={this.onMomentumScrollEnd.bind(this)}
    intent={this.clickListener.bind(this)}
/>

```

android and ios normal use,
For more details, please see [example code](./example/index.ios.js)

the [Swiper](./Swiper.js)  is from author [@xiaoyangchao](https://github.com/xiaoyangchao)/ [https://github.com/xiaoyangchao/react-native-swiper](https://github.com/xiaoyangchao/react-native-swiper)

(base of [https://github.com/leecade/react-native-swiper](https://github.com/leecade/react-native-swiper))

We could get the info above from the file called `'Banner.js'` in the example

## Screenshot
![](./images/banner_demo_ios.gif)
![](./images/banner_demo_android.gif)


## Run example

```javascript
cd ./example && npm install
react-native run-ios
react-native run-android

```
