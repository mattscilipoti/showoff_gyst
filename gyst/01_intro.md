!SLIDE
# GYST #
## "Grease Your Suite" Toolkit
## ~
### github.com/mattscilipoti/gyst

!SLIDE
# A suite of helpers
# to aid in
# speeding up your tests.

!SLIDE
# Inspired by...
## Nick "Grease Your Suite" Gauthier
## Chris "Iron Man" Strom

!SLIDE
# drop dead simple
# to utilize suggestions

!SLIDE
# Scripts
# Libraries
# Patches
## ~
# Practices

!SLIDE
# rakee
## ~
## configures REE for testing, 
## then runs the task(s)

!SLIDE
# gyst/factory_girl
## ~
## changes default strategy
## to :build

!SLIDE
# full disclosure

!SLIDE
# Gem
# &
# Project Blog

!SLIDE
# "Project" Blog for GYST
## ~
## "chain"
## warts and all

!SLIDE
# A blog for every project
## ~
## Someplace for news
## Close to the code
## Simple

!SLIDE
# Project Blog (Gem)
## ~
## BDD of CmdLine
## Gem/Gemfile creation
## gem scripts
## CI (travis)
## ReadmeDD

!SLIDE
# Project Blog (github pages)
## ~
## Create
## Publish
## Maintain
## Monitor
## Tweak

!SLIDE
# Gem
## ~
## Scripts
## Libraries
## Patches

!SLIDE
# TATFT &#169;

!SLIDE
# How to do test a script?

!SLIDE
# aruba/cmdline
## ~
    @@@ cucumber
    When I successfully run `your_cmd`
    Then the output should contain "abc"
    Then the output should match /abc/

!SLIDE code
    @@@ cucumber
    Scenario: rakee pass
        When I successfully run `rakee pass`
        Then the output should contain "Configuring REE"
        And the output should contain "PASS"
        And the output should report timing

!SLIDE
# How do you test scripts installed with a gem?

!SLIDE
# aruba/rvm
## ~
    @@@ cucumber
    Given I'm using a new gemset
    And a file named "<file_name>" with:
      """
      <file contents>
      """

!SLIDE
    @@@ cucumber
    @gemset
    Scenario: friendly loading (no such gem)
  
      Given I'm using a new gemset
      And a file named "gyst_factory_girl.rb" with:
        """
        require '../../lib/gyst/factory_girl'
        """
  
      When I run `ruby gyst_factory_girl.rb`
      Then the output should contain "Could not find 'factory_girl'"


!SLIDE
# scripts

!SLIDE
# rakee
## ~
## configures REE for testing, 
## then runs the task(s)
## ~
    rakee
    rakee test:units

!SLIDE
# raket
## ~
## `RAILS_ENV=test rakee`
## ~
    raket hydra
    raket db:reset

!SLIDE
# libraries/patches

!SLIDE
# require 'gyst/factory_girl'
## ~
## changes default strategy to
## :build

!SLIDE
# Future?
## ~
## db_null
## practices

