# Caminho das pedras para implementar

## Flutter

Atualizar seu pubspec.yaml com a ultima versão do workmanager, estou usando ^0.1.5.

- https://pub.dev/packages/workmanager

## Android 

Agora é chato...

Estou na master branch, então vou precisar fazer umas gambiarras aqui.

### App.kt

Você vai precisar criar um arquivo chamado `App.kt`, que vai ser o código responsável por colocar a lib do workmanager em background.

Este é o conteudo do arquivo.

**Lembrar de colocar o package no inicio**
```
import be.tramckrijte.workmanager.WorkmanagerPlugin
import io.flutter.app.FlutterActivity
import io.flutter.app.FlutterApplication
import io.flutter.plugin.common.PluginRegistry
import io.flutter.plugins.GeneratedPluginRegistrant

class App : FlutterApplication(), PluginRegistry.PluginRegistrantCallback {
    override fun onCreate() {
        super.onCreate()
        WorkmanagerPlugin.setPluginRegistrantCallback(this)
    }

        override fun registerWith(reg: PluginRegistry?) {
//            GeneratedPluginRegistrant.registerWith(reg)
        }
}
```
