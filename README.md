# SmokejsRails

This is a rails implementation of [Smoke-js](http://smoke-js.com/).

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'smokejs_rails'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install smokejs_rails

## Usage
add in `app/assets/javascripts/application.js` after jquery (below jquery)

	//= require smoke

add in `app/assets/stylesheets/application.css` 

	*= require smoke

```javascript
<script type="text/javascript">
    $(function(){

		smoke.confirm('this is still cool, yeah?',function(e){
		  if (e){
		    smoke.alert('OK pressed');
		  }else{
		    smoke.alert('CANCEL pressed');
		  }
		});

    });
</script>
```
###Doc
[smoke-js](http://smoke-js.com/)
*[jque.re](http://www.jque.re/plugins/modals-lightboxes/smoke.js/)*

```javascript
smoke.alert('this is a normal alert');
smoke.signal('this goes away after a sec');
smoke.confirm('behaves like a normal confirm?');
smoke.prompt('behaves like a normal prompt?');
```


## Contributing

1. Fork it ( https://github.com/guinslym/smokejs_rails/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
