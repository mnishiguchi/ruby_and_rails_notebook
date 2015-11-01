# ruby_and_rails_notebook

==

## BasicObject#instance_eval
- Evaluates a string containing Ruby source code, or the given block, within the context of the receiver (obj). 
- [BasicObject#instance_eval](http://ruby-doc.org/core-2.2.0/BasicObject.html#method-i-instance_eval)
- [Writing a Domain-Specific Language in Ruby](https://robots.thoughtbot.com/writing-a-domain-specific-language-in-ruby)

==

## Heredocs
- syntactically, the first delimiter represents the entire heredoc
- http://weblog.jamisbuck.org/2015/9/12/little-things-heredocs.html

```ruby
get "/string" do
  <<-EOS.gsub(/^\s*/, "")  # Strip leading whitespace from each line of the string
    <h1>This is a string directly passed in to the block</h1>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
    <script>alert('Awesome!!!');</script>
  EOS
end
```
