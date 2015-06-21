# Search

## Ordering

	` ^ _ - , ; : ! ? . ' "
	( ) [ ] { } @ * / \ & # % + < = > | ~ $
	0 1 2 3 4 5 6 7 8 9
	a A b B c C d D e E f F g G h H i I j J k K l L m M
	n N o O p P q Q r R s S t T u U v V w W x X y Y z Z
	
	["a"]
	["b"]
	["b","c"]
	["b","c", "a"]
	["b","d"]
	["b","d", "e"]
	
	{a:1}
	{a:2}
	{b:1}
	{b:2}
	{b:2, a:1}
	{b:2, c:2}

Object member order **does** matter for collation.
CouchDB preserves member order but doesn't require that clients will.

- [Collation specification in local docs](http://localhost:5984/_utils/docs/couchapp/views/collation.html#collation-specification)

- [ICU](http://site.icu-project.org/)

- [Unicode Collation Algorithm](http://www.unicode.org/reports/tr10/)


## Search by prefix

Use `startkey="abc"&endkey="abc\ufff0"`
instead of `startkey="abc"&endkey="abcZZZZZZZZZ"`.

- [String ranges in local docs](http://localhost:5984/_utils/docs/couchapp/views/collation.html#string-ranges)
