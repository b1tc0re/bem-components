# Миграция

## 2.1.0

В блоках `input`, `select` и `textarea` модификатор `width` вынесен из темы `islands`. Это дает возможность использовать его без указания темы. Теперь при динамической генерации BEMJSON нужно добавить модификатор в зависимости:

```
({
    shouldDeps : { block : 'input', mods : { width : 'available' } }
})
```
