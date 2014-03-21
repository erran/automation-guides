# Style
## Ruby
* Avoid metaprogramming (unless using strict prefixes)
* Prefer style from [the Ruby Style Guide](https://github.com/bbatsov/ruby-style-guide#readme)

## Cucumber
* Prefer tagged hooks over global
* Use the keyword `Scenario Template` instead of `Scenario Outline`
* Use the keyword `Scenarios` instead of `Examples`

## Capybara
* Avoid using `all(css)`
  * Prefer using `find(css, text: 'John Doe')` with restrictions
* Avoid using both CSS **and** XPath
* Prefer using CSS over XPath
* Prefer helper methods to reusing CSS IDs/classes
* Prefer navigation using `#click` methods over `#visit`
* Use `within(scope, &block)` when checking for nested elements

## Structure
[Example](structure.md)

* Prefer using the feature name (in `snake_case`) as the file name
* Use separate files for unrelated helpers
* Use separate files for unrelated step definitions
* Use separate files to classify hooks
