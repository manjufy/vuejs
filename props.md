# Props - All about Props

`<cat-component :breed="breed" :color="color" :size="size" />`

Can be simplified to 

`<cat-component v-bind="{breed, color, size}" />`


### Passing methods as props

```
// Calling custom fish component
<fish v-bind="{color, size}" @swim="swim" />
// Inside custom fish component
...
<button @click="$emit('swim', data)">
...
```

There is another Succinct way

```
// Calling custom fish component
<fish v-bind="{color, size, swim}" />
// Inside custom fish component
...
<button @click="swim(data)">
...
```

In the above case, props is a simple callback.

Reference: https://medium.com/front-end-hacking/passing-methods-as-props-in-vue-js-d65805bccee
