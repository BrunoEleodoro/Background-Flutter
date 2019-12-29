# Background-Flutter

Bom, a ideia aqui é simples, executar códigos em background usando flutter.

O código deve fazer a coleta da latitude e longitude do usuario, e tambem conectar a um dispositivo bluetooth e salvar no localstorage.

Show!.

Agora na prática...

## Checklist
- [ ] Executar em background no IOS
- [ ] Conectar bluetooth no IOS
- [ ] Salvar localstorage no IOS
- [ ] Pegar Latitude e Longitude no IOS
- [ ] Executar em background no Android
- [ ] Conectar bluetooth no Android
- [ ] Salvar localstorage no Android
- [ ] Pegar Latitude e Longitude no Android

As libs que vamos usar são.

- https://pub.dev/packages/geolocator
- https://pub.dev/packages/flutter_blue

O melhor dos mundos seria se essa lib aqui tivesse suporte para IOS, como não tem, temos que usar a flutter_blue quando for IOS.
- https://pub.dev/packages/flutter_bluetooth_serial
- https://pub.dev/packages/workmanager
