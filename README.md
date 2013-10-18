# FuzzyMatchers

A Fuzzy Matcher that helps when checking equality over complex data.

At the moment it just checks for equality.

## Installation

Add this line to your application's Gemfile:

    gem 'fuzzy_matchers'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install fuzzy_matchers

## Usage

An example usage checking equality between two Hashes

```ruby
  a = { a: 1, b: { c: [1, 2] } }
  b = { a: 1, b: { c: [2, 1] } }
  
  FuzzyMatcher.equals?(a,b)
  => true
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
