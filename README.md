# Spree Recently Viewed

[![Build Status](https://travis-ci.org/spree-contrib/spree_recently_viewed.svg?branch=master)](https://travis-ci.org/spree-contrib/spree_recently_viewed)
[![Code Climate](https://codeclimate.com/github/spree-contrib/spree_recently_viewed/badges/gpa.svg)](https://codeclimate.com/github/spree-contrib/spree_recently_viewed)

This extension maintains and displays a list of the products a user has recently viewed.

## Installation

1. Add this extension to your Gemfile with this line:
  ```ruby
  gem 'spree_recently_viewed', github: 'spree-contrib/spree_recently_viewed'
  ```

2. Install the gem using Bundler:
  ```ruby
  bundle install
  ```

3. Copy & run migrations
  ```ruby
  bundle exec rails g spree_recently_viewed:install
  ```

4. Restart your server

  If your server was running, restart it so that it can find the assets properly.

---

## Customization

 Change max count of products vieweds

 Add this line in `config/initializers/spree.rb`:
  ```ruby
  Spree::RecentlyViewed::Config.preferred_recently_viewed_products_max_count = 10
  ```

---


## Contributing

See corresponding [guidelines][4]

---

Copyright (c) 2009-2015 [Roman Smirnov][6], [Brian Quinn][7] and other [contributors][8], released under the [New BSD License][3]

[1]: http://www.fsf.org/licensing/essays/free-sw.html
[2]: https://github.com/spree-contrib/spree_recently_viewed/issues
[3]: https://github.com/spree-contrib/spree_recently_viewed/blob/master/LICENSE.md
[4]: https://github.com/spree-contrib/spree_recently_viewed/blob/master/CONTRIBUTING.md
[6]: https://github.com/romul
[7]: https://github.com/BDQ
[8]: https://github.com/spree-contrib/spree_recently_viewed/graphs/contributors
