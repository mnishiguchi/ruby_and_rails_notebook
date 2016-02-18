# String manipulation

## removing line numbers from lines
```ruby
def process(lines)
  lines.map do |line|
    _, *content = line.split
    content.join("\s")
  end.join("\s")
end
```
