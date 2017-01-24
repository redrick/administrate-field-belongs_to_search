# Administrate::Field::BelongsToSearch

A plugin to search through `belongs_to` associations in [thoughtbot's Administrate](https://github.com/thoughtbot/administrate) Rails engine.

## Usage

Add it to your `Gemfile`:

```ruby
gem 'administrate-field-belongs_to_search', git: 'https://github.com/fishbrain/administrate-field-belongs_to_search.git'
```

Run bundler to install:

```sh
bundle install
```

Add it to your Administrate dashboard, for instance:

```ruby
class PostDashboard < Administrate::BaseDashboard
  ATTRIBUTE_TYPES = {
    author: Field::BelongsToSearch.with_options(class_name: 'User')
  }
end
```

## License

This plugin is Copyright © 2017 Fishbrain AB. It is licensed under the MIT license. See [LICENSE](LICENSE) for details.

========

![Fishbrain AB](http://i.imgur.com/wOMiqE8.png)

This plugin is maintained by [Fishbrain AB](https://fishbrain.com).

At Fishbrain, we're passionate about the outdoors and conservation. Together, we work to bring you the best app for fishing, hands down.

If you love working with amazing and talented people in tight-knit teams, [come work with us](https://fishbrain.com/jobs/)!