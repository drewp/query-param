# query-param
`<query-param>` is a polymer element for syncing a JS property to a url query parameter.

Demo: https://bigasterisk.com/query-param/demo.html

Example:
```
    <input type="checkbox" checked="{{enableSort::change}}">
    <query-param key="es" prop="enableSort"></query-param>
    ...
    Polymer({
     properties: {
       enableSort: {type: Boolean, value: false, notify: true},
```

The `<query-param>` element arranges a two-way sync between the polymer
property `enableSort` and a new url query parameter that will look like
`?es=1`.
