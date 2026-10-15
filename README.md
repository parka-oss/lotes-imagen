# lotes-imagen
Cálculo repartido por lotes cifrados en GitHub Actions.
El lote y cada orden viajan cifrados (AES-256, clave fuera del repo); cada trabajo devuelve su salida cifrada como artifact.
El log público solo muestra el código de salida y la duración de cada trabajo.
Se dispara a mano (`workflow_dispatch`) desde una herramienta local; no corre con pull requests ni con otros eventos.
