# Rails Style Guide

This style is based on rules from [Ruby Style Guide](docs/STYLE_GUIDE.md). Also, we enforce rules from [community Rails Style Guide][1].

This is a small list of differences which we have when compared with community and our Ruby style guides:

## Table of contents

* [Style](#Style)

## Style

* <a name="documentation"></a>
  Documentation is requeried for all files except `app` directory.
  <sup>[[link](#documentation)]</sup>

* <a name="nested-style-and-modules"></a>
  Prefer to use nested style of children definitions at classes and modules.
  <sup>[[link](#nested-style-and-modules)]</sup>

```ruby
# bad
class Api::V1::UsersController
end

# good
module Api
  module V1
    class UsersController
    end
  end
end
```

[1]: https://github.com/rubocop-hq/rails-style-guide
