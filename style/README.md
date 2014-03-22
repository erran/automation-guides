# Style
## Ruby
* Avoid metaprogramming (unless using strict prefixes)
* Prefer style from [the Ruby Style Guide](https://github.com/bbatsov/ruby-style-guide#readme)
* Use [YARD](http://rubydoc.info/gems/yard/file/docs/GettingStarted.md) for code documentation
  * Don't use RDoc style comments
  * Use the [YARD Tag Overview](http://rubydoc.info/gems/yard/file/docs/Tags.md) 

## Cucumber
* Avoid step definitions with more than two captures
* Prefer tagged hooks over global
* Use alternative keywords were they make sense (`cucumber --i18n en`)
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
* Use Ruby objects to represent [HTML classes](http://www.w3schools.com/css/css_id_class.asp)

## Structure
[Example](structure.md)

* Prefer naming feature files after features in `snake_case`
* Use separate files for unrelated helpers
* Use separate files for unrelated step definitions
* Use separate files to classify hooks
