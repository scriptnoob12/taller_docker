
## Ejercicio 11- Taller Docker

```
// Primero creé el archivo deployment.yaml
// Agregué la base descripta en la tarea
// Modifique para que tenga el nombre correcto para su funcionamiento y legibilidad
// Ejecute el comando para aplicar el descriptor
kubectl apply -f .\deployment.yaml

// Use el comando get pods para ver si estaba corriendo y su id
kubectl get pods

// Use el comando exec para poder corroborar su correcta ejecución
kubectl exec -it password-api-5f7dc647df-b6hm5 -- bash

// Y por último ejecute el comando curl
curl localhost:3000/password
```
