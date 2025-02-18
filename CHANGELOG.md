## HEAD (unreleased)

Authors: doits, jstoks

* Adds: Support for Ruby 3.0 keyword arguments
* Removes: Support for Ruby 2.6 and lower

## 2.0.1 (29th Aug 2019)

Authors: David Wilkie, hosseintoussi, Maxim Polunin, Tristan
Harmer, Bartosz Żurkowski, Kris Leech

* fix: support nested temporary global listeners
* docs: add threadsafe notes to README for global and temporary listeners
* docs: fix spelling mistakes in README
* fix: safely get signing key in gemspec when HOME is not set
* adds: add console to aid experiments and REPL driven development
* adds: Latest Ruby to CI

## 2.0.0 (7th Mar 2017)

Authors: Sergey Mostovoy, Andrew Kozin, Kyle Tolle, Martin, Rob Miller, Mike
Dalto, orthographic-pedant, Drew Ulmer, Mikey Hogarth, Attila Domokos, Josh
Miltz, Pascal Betz, Vasily Kolesnikov, Julien Letessier, Kris Leech

* Fix: logger raises exception if hash is passed as an argument to a listener #133, #136
* Fix: deprecation warnings #120
* Doc improvements: #106, #111, #116, #122, #128, #130, #147, #149, #150, #151
* Adds: Allow configuration of default prefix when using `prefix: true`. #105
* Adds: Allow unsubscribing of global listeners #118
* Adds: Helpful error message when passing a block to `#subscribe` of `#on` #125
* Adds: raise an error message when `#on` is not passed a block #146
* Adds: Support for JRuby 9.x #148
* Adds: Support for MRI 2.4.0 #155
* Refactor specs #126, #131

## 2.0.0.rc1 (17 Dec 2014)

Authors: Kris Leech

* remove: deprecated methods
* remove: rspec matcher and stubbing (moved to [wisper-rspec](https://github.com/krisleech/wisper-rspec))
* feature: add regexp support to `on` argument
* remove: announce alias for broadcasting
* docs: add Code of Conduct
* drop support for Ruby 1.9

## 1.6.0 (25 Oct 2014)

Authors: Kris Leech

* deprecate: add_listener, add_block_listener and respond_to
* internal: make method naming more consistent

## 1.5.0 (6th Oct 2014)

Authors: Kris Leech

* feature: allow events to be published asynchronously
* feature: broadcasting of events is plugable and configurable
* feature: broadcasters can be aliased via a symbol
* feature: logging broadcaster

## 1.4.0 (8th Sept 2014)

Authors: Kris Leech, Marc Ignacio, Ahmed Abdel Razzak, kmehkeri, Jake Hoffner

* feature: matcher for rspec 3
* fix: temporary global listeners are cleared if an exception is raised
* refactor: update all specs to rspec 3 expect syntax
* docs: update README to rspec 3 expect syntax
* feature: combine global and temporary listener methods as `Wisper.subscribe`
* deprecate: `Wisper.add_listener` and `Wisper.with_listeners,` use `Wisper.subscribe` instead

## 1.3.0 (18th Jan 2014)

Authors: Kris Leech, Yan Pritzker, Charlie Tran

* feature: global subscriptions can be scoped to a class (and sub-classes)
* upgrade: use rspec 3
* feature: allow prefixing of events with 'on'
* feature: Allow stubbed publisher method to accept arbitrary args

## 1.2.1 (7th Oct 2013)

Authors: Kris Leech, Tomasz Szymczyszyn, Alex Heeton

* feature: global subscriptions can be passed options
* docs: improve README examples
* docs: add license to gemspec

## 1.2.0 (21st July 2013)

Authors: Kris Leech, Darren Coxall

* feature: support for multiple events at once
* fix: clear global listeners after each spec

## 1.1.0 (7th June 2013)

Authors: Kris Leech, chatgris

* feature: add temporary global listeners
* docs: improve ActiveRecord example
* refactor: improve specs
* upgrade: add Ruby 2.0 support
* fix: make listener collection immutable
* remove: async publishing and Celluloid dependency
* fix: Make global listeners getter and setter threadsafe [9]

## 1.0.1 (2nd May 2013)

Authors: Kris Leech, Yan Pritzker

* feature: add async publishing using Celluloid
* docs: improve README examples
* feature: `stub_wisper_publisher` rspec helper
* feature: global listeners
* refactor: improve specs

## 1.0.0 (7th April 2013)

Authors: Kris Leech

* refactor: specs
* refactor: registrations
* feature: Add `with` argument to `subscribe`
* docs: improve README examples
* feature: Allow subscriptions to be chainable
* feature: Add `on` syntax for block subscription
* remove: Remove support for Ruby 1.8.7
* docs: Add badges to README

## 0.0.2 (30th March 2013)

Authors: Kris Leech

* remove: ActiveSupport dependency
* docs: fix syntax highlighting in README

## 0.0.1 (30th March 2013)

Authors: Kris Leech

* docs: add README
* feature: registration of objects and blocks
