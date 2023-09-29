::: column
# Syntaxe SFC 

```html
<template>
    <!-- HTML -->
</template>

<script>
// JS
</script>

<style>
/* CSS */
</style>
```

# Syntaxe Options API

```html
<template>
    <div> {{message}} </div>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
    props: {
        message: String
    },
})
</script>

<style>
div{
    color: red;
}
</style>
```

# Syntaxe Composition API

```html
<template>
    <div> {{message}} </div>
</template>

<script>
import { defineComponent, ref } from 'vue'

export default defineComponent({
    props: {},
    setup(){
        const message = ref('Hello World')
    }
})
</script>
```

# Syntaxe Script Setup + TS

```html
<template>
    <div> {{message}} </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

defineProps<Props>()
const message = ref('Hello world')
</script>
```