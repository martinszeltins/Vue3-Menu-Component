# Vue3-Menu-Component

**Usage**

```html
<dropdown-menu
    v-model="show">

    <button @click="show = !show">
        Click to open dropdown
    </button>

    <template v-slot:dropdown>
        <div class="menu-wrapper">
            <div>Action</div>
            <div>Another action</div>
            <div>Something else here blah blah blah</div>
            <div>Something else here</div>
            <div>Something else here</div>
            <div>Something else here</div>
        </div>
    </template>
</dropdown-menu>
```

**Available Props**

````
modelValue: {
    type: Boolean,
    default: false,
},

positionX: {
    type: String,
    default: 'center',
},

positionY: {
    type: String,
    default: 'bottom',
},

transition: {
    type: String,
    default: 'fade',
},

offsetX: {
    type: String,
    default: '0px',
},

offsetY: {
    type: String,
    default: '5px',
},

closeOnClick: {
    type: Boolean,
    default: true,
},
````