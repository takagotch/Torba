### Torba
---
https://github.com/torba-rb/torba

```
gem 'torba'


```

```ruby
zip "name", url: "..." [, import: %w(...)]
zip "scroll_magic", url: "http://github.com/janpaepke/ScrollMagic/archive/v2.0.0.zip"
targz "name", "..." [, import: %w(...)]
targz "scroll_magic", url: "http://github.com/janpaepke/ScrollMagic/archive/v2.0.0.tar.gz"
gh_release "name", source: "...", tag: "..." [, import: %w(...)]
gh_release "scroll_magic", source: "janpaepke/ScrollMagic", tag: "v.2.0.0"
gh_release source: 'janpaepke/ScrollMagic', tag: "v.2.0.0"
npm "name", package: "...", version: "..." [, import: %w(...)]
npm "coffee", package: "coffee-script", version: "1.9.2"
npm package: "coffee-script", version: "1.9.2"

```

```css
// application.js
//= require 'underscore/underscore'

//= require_directory 'underscore'

/* application.css */
@import 'lightslider/dist/css/lightslider';

gh_release "lightslider", source: "sachinchoolur/lightslider", tag: "1.1.2", import: %w[
  dist/css/lightslider.css
]

@import 'lights/lightslider';

gh_release "lightslider", source: "sachinchoolur/lightslider", tag: "1.1.2", import: %w[
  dist/css/lightslider.css
  dist/img/*.png
]
```

