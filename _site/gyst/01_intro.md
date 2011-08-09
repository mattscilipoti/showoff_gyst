!SLIDE
# GYST #
## "Grease Your Suite" Toolkit
## ~
### github.com/mattscilipoti/gyst

!SLIDE
# A suite of helpers to aid in speeding up your tests.

!SLIDE
# Inspired by...
## Nick "Grease Your Suite" Gauthier
## Chris "Iron Man" Strom

!SLIDE
# speed up tests

!SLIDE
# drop dead simple

!SLIDE
# Scripts
# Libraries
# Patches
## ~
# Practices

!SLIDE
# Gem
# &
# Project Blog

!SLIDE
# A blog for every dev project
## ~
## Easy to share/find news
## Close to the code
## Simple

!SLIDE
# Project Blog
## ~
## "chain"
## warts and all

!SLIDE
# Project Blog (Gem)
## ~
## BDD of CmdLine
## Gem/Gemfile creation
## deploying bash scripts
## CI (travis)
## ReadmeDD

!SLIDE
# Project Blog (github pages)
## ~
## Create
## Publish
## Maintain
## Monitor

!SLIDE
# Gem
## ~
## Scripts
## Libraries
## Patches

!SLIDE
# rakee
## ~
## configures REE for testing, 
## then runs the task(s)

!SLIDE
# gyst/factory_girl
## ~
## changes default strategy to
## :build

!SLIDE
# full disclosure

!SLIDE
# TATFT &#169;

!SLIDE
# How to do test a script?

!SLIDE
# aruba/cmdline
## ~
    @@@ cucumber
    When I successfully run
    Then the output should contain "abc"
    Then the output should contain /abc/

!SLIDE
# How do you test scripts installed with a gem?

!SLIDE
# aruba/rvm
## ~
    @@@ cucumber
    Given I'm using a new gemset
    And a file named "gyst_factory_girl.rb" with:
      """
      require '../../lib/gyst/factory_girl'
      """

!SLIDE
# rakee
## ~
## configures REE for testing, 
## then runs the task(s)

!SLIDE
# raket
## ~
## `RAILS_ENV=test rakee`

!SLIDE
# gyst/factory_girl
## ~
## changes default strategy to
## :build

!SLIDE
# Future?
## ~
## db_null
## practices

