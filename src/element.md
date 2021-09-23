# ELEMENT ( __ )

Elements are the constituent parts of a block that can’t be used outside of it.

A good example is if you have a navigation menu, the items it contains don’t make sense outside the context of the menu. You wouldn’t define a block for a menu item. You’d have a block for the menu itself, and the menu items are child elements.

```css
.card {

}

.card__title {

}
```

```html
<div class="row">
    <div class="card">
        <h1 class=card__title>Title</h1>
    </div>
</div>
```