---
category: Utilities
---

# useDebounce

Debounce execution of a ref value.

## Usage

```js {4}
import { useDebounce } from '@vueuse/core'

const input = ref('foo')
const debounced = useDebounce(input, 1000)

input.value = 'bar'
console.log(debounced.value) // 'foo'

await sleep(1100)

console.log(debounced.value) // 'bar'
```

## Related Functions

- `useThrottle`
- `useThrottleFn`
- `useDebounce`
- `useDebounceFn`

## Recommended Reading

- [**Debounce vs Throttle**: Definitive Visual Guide](https://redd.one/blog/debounce-vs-throttle)
