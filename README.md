# NVD3 Rails - Reusable charts for Rails 3

## Install

To include nvd3-rails into your rails project add

    gem "nvd3-rails"

To your Projects Gemfile with ``https://rubygems.org`` as your gem source.

To add all nvd3 javascript files into your asset pipeline add:

    //= require nvd3-rails

in ```app/assets/javascripts/application.js```

also add:

    *= require nvd3-rails

in ```app/assets/stylesheets/application.css```

Note as of today nvd3 clutters the model naming e.g. lineWithFisheyeChart.js and lineChart.js export their model both as lineChart.

If you only need a subset of models e.g. lineChart you can add:

    //= require nvd3/lib/d3.v2
    //= require nvd3/src/core
    //= require nvd3/src/tooltip
    //= require nvd3/src/utils.js
    //= require nvd3/src/models/lineChart
    //= require nvd3/src/models/legend.js
    //= require nvd3/src/models/axis.js
    //= require nvd3/src/models/scatter.js
    //= require nvd3/src/models/line.js

to your ```application.js```
