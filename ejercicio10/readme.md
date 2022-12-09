## Ejercicio 10- Taller Docker
![image](https://user-images.githubusercontent.com/58433889/206601502-889dab32-50e6-4e20-9971-e8e152acdb05.png)
![image](https://user-images.githubusercontent.com/58433889/206601531-8616bc5d-ac25-46ed-ab25-c11865336bf0.png)

```
// Verifiqué que esté funcionando correctamente 
 docker run -e TELEGRAM_TOKEN= ACOMPLETAR nicopaez/telegrambot:0.0.7
 
// Luego cree el archivo telegrambot.yaml
// Indique el name y la imagen en conjunto con la variable de env.
// Ejecuté el siguiente comando para aplicar
kubectl apply -f .\telegrambot.yaml

// Ejecute el comando para saber si estaba corriendo correctamente
kubectl get pods

// Al final ejecute el log para saber que es lo que hacía cuando en telegram ejecutaba /version
kubectl logs ejercicio10

```
