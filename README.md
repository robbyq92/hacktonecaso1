# hacktonecaso1
kubectl apply -f fichero.yml
kubectl get pods -n hacktone1
kubectl get svc -n hacktone1

Comprobamos el pod/servicio creado en el namespace hacktone1:

Se hace un port-forward para comprobar los datos.
![image](https://github.com/robbyq92/hacktonecaso1/assets/49034238/afb4cd28-e752-4dce-b781-0f6481d276e0)
Despues se comprueba en el navegador
![image](https://github.com/robbyq92/hacktonecaso1/assets/49034238/b0409cc3-ca5e-438b-99d1-ae57c535e8d4)

Se hace un escalado de 3 replicas al deploy para revisar que se crean 3 Pods en total y balancean el trafico al servicio.
![image](https://github.com/robbyq92/hacktonecaso1/assets/49034238/275ca4ef-76f4-4cbf-b7a2-2fd72436e006)


kubectl get pods -n hacktone1 para revisar los 3 Pods activos
![image](https://github.com/robbyq92/hacktonecaso1/assets/49034238/ba9c524f-623d-4d51-9750-39630311c505)

Se revisa por último el balanceo, en este caso me he conectado a uno, e hice ping al servicio:
![image](https://github.com/robbyq92/hacktonecaso1/assets/49034238/40c57e49-f24f-45c9-8fc1-9241136116a5)
