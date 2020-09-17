# Alterative fusion base page rendering
The alternative page rendering provides a more flexible way for basic document node rendering.

Structure
---------
```
body = Neos.Fusion:Array {
    @position = 'after bodyTag'
    content = Neos.Fusion:Array {
        main = Neos.Neos:PrimaryContent {
            nodePath = 'main'
        }
    }
}
```

`Body` and `Content` are `Neos.Fusion.Array` prototypes wrapping the actual main `Neos.Neos:PrimaryContent` content. This gives you more flexibility for registering some *none* primaory content related prototypes like *modal windows* or navigational elements (eg. scrollToTop).

Additinally it's just fusion based and works without fluid template.

Acknowledgments
---------------
Development sponsored by [web&co](http://webandco.com).

License
----------
Licensed under MIT, see [LICENSE](LICENSE)