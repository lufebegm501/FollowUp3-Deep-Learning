# FollowUp3 de Deep Learning

Imágenes para el ejercicio académico de ataques adversarios.

- `cat.png` y `cat_attack.png`: imágenes suministradas en el material del curso, procedentes de https://github.com/jrballesteros/adversarial_attacks. Se conservan sin modificación.
- `original.png`: baseline RGB de 224 × 224 empleado en el bono.
- `adversarial.png`: resultado generado con L-BFGS-B contra ResNet50 de Keras, con objetivo `ostrich` (avestruz). El éxito se verificó después de guardar y recargar el PNG.

## Pruebas

En el portal Keras.js, Inception v3 predijo gato persa (86 %) para cat.png y tostadora (91 %) para cat_attack.png. Los porcentajes son los valores redondeados mostrados por la interfaz.

El ataque del bono consiguió avestruz con probabilidad 0.6332 en el modelo local atacado. Esto no garantiza transferencia a otras redes ni equivalencia con los pesos o el preprocesamiento del portal.

Portal: https://transcranial.github.io/keras-js/#/inception-v3

Referencia metodológica: Szegedy et al., Intriguing properties of neural networks, https://arxiv.org/abs/1312.6199.
