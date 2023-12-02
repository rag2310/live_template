# live_template

## Android Studio

#### el siguiente live template para crear un nuevo mutable state data en un viewmodel y colocar la data class

```xml
<template name="newstate" value="private val _$NAME$: MutableStateFlow&lt;$PARAM1$&gt; = MutableStateFlow(&#10;    $PARAM1$()&#10;)&#10;val $NAME$: StateFlow&lt;$PARAM1$&gt; = _$NAME$.asStateFlow()" description="Make State Flow" toReformat="true" toShortenFQNames="true" useStaticImport="true">
  <variable name="NAME" expression="" defaultValue="" alwaysStopAt="true" />
  <variable name="PARAM1" expression="" defaultValue="" alwaysStopAt="true" />
  <context>
    <option name="OTHER" value="true" />
  </context>
</template>
```
