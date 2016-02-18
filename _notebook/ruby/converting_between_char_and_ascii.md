# Converting between char and ASCII

- `character.ord` : convert charcter to ascii [doc](http://apidock.com/rails/String/ord)
- `ascii.chr`     : convert ascii to charcter [doc](http://apidock.com/ruby/Integer/chr)

```
# character.ord #==> convert charcter to ascii
# ascii.chr     #==> convert ascii to charcter
s = "wklv phvvdjh lv qrw wrr kdug wr euhdn"
a = s.split("")
a.map do |c|
  if c == " "
    " "
  else
    ( c.ord - 3 ).chr
  end
end.join #==> "this message is not too hard to break"
```
