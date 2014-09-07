# Automation framework
This document describes the basic design of what I consider an automation framework (built around BDD/Cucumber).

## Table of Contents
1. [Layout](#layout)
2. [APIs](#apis)
  1. [API clients](#api-clients)
3. [Cucumber](#cucumber)
4. [RSpec](#rspec)
5. [Capybara](#capybara)

##  Layout

## APIs
Tests that use the UI are going to be **much slower**. If you can
implement a test using an API instead **do it**!

### API clients
I'm partial to using a [REST][REST] JSON API here. The logic applies to other API formats though.

```ruby
client = MyApp::Client.new(your_credentials)

wile_e_coyote = client.user('wile_e_coyote')   # GET /users/wile_e_coyote
# => #<MyApp::User @name="Wile E. Coyote" @username="wile_e_coyote"]>

wile_e_coyote.name                             # returns the "name" JSON property
# => "Wile E. Coyote"
wile_e_coyote.username                         # returns the "username" JSON property
# => "wile_e_coyote"

# Notice that our user *has_one* cart. Requests can be relational!
wile_e_coyote.cart                             # GET /users/wile_e_coyote/cart
# => #<MyApp::Cart @items=[#<MyApp::Item @id=1 @name="Dynamite" @owner="wile_e_coyote">]>
```

## Cucumber

## RSpec

## Capybara

[REST]: http://en.wikipedia.org/wiki/Representational_state_transfer "Representational state transfer"
