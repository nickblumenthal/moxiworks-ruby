# MoxiworksPlatform

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'moxiworks_platform'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install moxiworks_platform

## Usage

```ruby
require 'moxiworks_platform'


platform_identifier = 'abc1234'
platform_secret = 'secretkey'


MoxiworksPlatform::Credentials.new(platform_identifier, platform_secret)

contact = MoxiworksPlatform::Contact.create(moxi_works_agent_id: '123abcd', partner_contact_id: 'my_unique_id')
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/moxiworks-platform/moxiworks-ruby
