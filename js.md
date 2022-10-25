**Prueba Reconocimiento de voz**

```js
const recognition = new
webkitSpeechRecognition()

recognition.lang = 'es-ES'

recognition.continous = true

recognition.onresult = event => {
    for (const result of event.results)
        console.log(result[0].transcrip)
}

recognition.start()
```
