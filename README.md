# ICAPrb::Server

propellerhat's fork of fabianfrz's ICAPrb-Server. I will be adding some bug fixes and features. Stay tuned.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'icaprb-server'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install icaprb-server

## Usage

Getting your server running is really easy:

```ruby
# require it
require "icaprb/server"

# create an instance of a server
s = ICAPrb::Server::ICAPServer.new

# add your services
s.services['echo'] = ICAPrb::Server::Services::EchoService.new

# and run it
s.run

```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

