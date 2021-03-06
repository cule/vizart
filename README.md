# vizart

> It is recommended to use vizart components.

## Usage: Components

1. Install a vizart component:

```
npm install vizart-basic --save
```

2. import and use

```
import 'vizart-basic/dist/vizart-basic.css';
import { bar } from 'vizart-basic';

const chart = barar(domId, opt)....
```

## Usage: vizart
With this approach, all charts are available.

1. Install VizArt in your project
```
npm install vizart --save
```

2. import and use

```
import 'vizart/dist/vizart.css';
import { bar } from 'vizart';

const chart = bar(domId, opt)....
```

## Three steps to use a chart
1. initialize a chart with domId and declarative options
```
const opt = {
  ...
};
const chart = bar('#chart', opt)
```
You only need to provide essential options. [Demo](https://vizartjs.github.io/demo.html) is a good place to check essential options for all charts. You may check up Documentation of each component for full option spec so as to control more chart behaviours.

2. Render a chart with data
```
chart.render(data) // this should be called only once
```
3. Change a chart on the fly
```
// copy and update full options
const opt = chart.options();
opt.plots.opacityArea = o.4

// or in minimum
const opt = { plots: {opacityArea: 0.2 }};

// update options
chart.options(opt);
chart.update();
```



## Resources

* [Demo](https://vizartjs.github.io/demo.html): quick reference with source code
* [Documentation](https://github.com/VizArtJS/vizart/wiki)

## Components
Production ready:
* [vizart-basic](https://github.com/VizArtJS/vizart-basic)
* [vizart-path](https://github.com/VizArtJS/vizart-path)
* [vizart-core](https://github.com/VizArtJS/vizart-core)
* [vizart-hierarchy](https://github.com/VizArtJS/vizart-hierarchy)
* [vizart-geo](https://github.com/VizArtJS/vizart-geo)

## Credits
My work is based on/inspired by other people's works. You can find links and author names of originals works at each sub module's home page
as well as at vizart's demo page.

Thanks to Mike Bostock, the creator of [d3.js](www.d3js.org). I create vizart on top of d3 modules. I also study [d3 examples](https://github.com/d3/d3/wiki/Gallery) extensively.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details



