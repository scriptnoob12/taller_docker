## Ejercicio 03 - Taller Docker

Utilizando el comando docker inspect, y dandole un formato pude obtener los layers listados.
```
  docker inspect -f ' {{range .RootFS.Layers}} {{ println .}} {{end}}' 22e1f6ea60af
```

###### nicopaez/passwordapi-java:java8-fabric:
- 9 Layers.
###### nicopaez/passwordapi-java:java8-alpine:
- 4 Layers.

#### El único layer en común:
![image](https://user-images.githubusercontent.com/58433889/202052143-730fc3e5-a800-4792-a5ef-4f51245573c8.png)
