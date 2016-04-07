# ng-click-toggle
Angular directive that toggles classes on click


Example
=======

```
<button
    data-click-toggle="nav-visible" data-click-toggle-target="body"
    class="nav-trigger">Menu</button>
```

When the above button is clicked it will toggle the class nav-visible on the body element

target attribute is passed as is to jquery, if no target is present the element the directive
is present on is assumed to be the target.


The class to toggle can be multiple classes, the string is passed as is to jquery.toggleClass

click callback returns false if additional attribute `data-prevent-default` is present.
i.e `data-prevent-default="true"`
