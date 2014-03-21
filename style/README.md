# Style
## Ruby
* Avoid metaprogramming (unless using strict prefixes)
* Prefer style from [the Ruby Style Guide](https://github.com/bbatsov/ruby-style-guide#readme)

## Cucumber
* Prefer tagged hooks over global
* Use the keyword `Scenario Template` instead of `Scenario Outline`
* Use the keyword `Scenarios` instead of `Examples`

## Capybara
* Don't use `all('css')` unless you intend to use assert against several elements
* Prefer CSS over XPath
* Prefer helper methods to reusing CSS IDs/classes
* Prefer navigation using `#click` methods over `#visit`
* Use either CSS or XPath; Avoid using both
* Use `within(scope, &block)` when checking for nested elements

## Structure
[Example](structure.md)

* Use separate files for unrelated helpers
* Use separate files for unrelated step definitions
* Use separate files to classify hooks
