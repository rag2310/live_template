# live_template

## Android Studio

Necesitamos crear el directorio templates en las siguientes rutas dependiendo de tu sistema operativo

- Windows

Sintaxis: %APPDATA%\Google\<product><version>

Ejemplo: C:\Users\YourUserName\AppData\Roaming\Google\AndroidStudio4.1

- macOS

Sintaxis: ~/Library/Application Support/Google/<product><version>

Ejemplo: ~/Library/Application Support/Google/AndroidStudio4.1

- Linux

Sintaxis: ~/.config/Google/<product><version>

Ejemplo: ~/.config/Google/AndroidStudio4.1

#### el siguiente live template para crear un nuevo mutable state data en un viewmodel y colocar la data class
Se crea el archivo Kotlin.xml y se inserta lo siguiente:

```xml
<templateSet group="Kotlin">
  <template name="newstateui" value="private val _$NAME$: MutableStateFlow&lt;$PARAM1$&gt; = MutableStateFlow(&#10;    $PARAM1$()&#10;)&#10;val $NAME$: StateFlow&lt;$PARAM1$&gt; = _$NAME$.asStateFlow()" description="Make State Flow" toReformat="true" toShortenFQNames="true">
    <variable name="NAME" expression="" defaultValue="" alwaysStopAt="true" />
    <variable name="PARAM1" expression="" defaultValue="" alwaysStopAt="true" />
    <context>
      <option name="KOTLIN" value="true" />
    </context>
  </template>
</templateSet>
```
