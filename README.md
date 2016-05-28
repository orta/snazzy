# Snazzy

The younger brother of [Realm's Jazzy](https://github.com/realm/jazzy). Jazzy is a documentation engine for building a site that covers all of the documentation of a Swift/Objective-C project.

Snazzy on the other hand is to help you generate a README from the documentation instead. It aims for brevity, and readbility on a smaller scale, for projects that are not big enough to warrent all the overhead of a separate website.

Snazzy sits on-top of [SourceKitten](https://github.com/jpsim/SourceKitten), and works with the JSON API.

This currently does nothing. This is [README driven development](http://tom.preston-werner.com/2010/08/23/readme-driven-development.html). It's based on some work I [did for RxSwiftCommunity](https://github.com/RxSwiftCommunity/RxSwiftExt/issues/39).

## Installation

Install using

    $ gem install snazzy

then run using `snazzy`

## Usage

Options I'd like to see in Snazzy:

* Choose specific classes to document: `snazzy --whitelist=ORStackView,ORStackType`
* Choose specific subclasses ( or extensions of ) to document `snazzy --related=ARAnalyticsProvider`
* Have options to automatically update a readme by declaring the top and bottom markers: `snazzy --readme=README.md --before="### API" --after="### Contributors"`
* Run from a Podspec: `snazzy --podspec=Specta.podspec`
* Pass in all sorts of crazy xcode options: `snazzy -- --workspace=Artsy.xcworkspace`

Future:

* Handle SPM once it's usable: `snazzy --use-spm`

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/orta/snazzy.

