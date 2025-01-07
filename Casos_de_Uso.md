# Prueba Técnica Inlaze – Analista de Requerimientos Funcionales

Este repositorio contiene la solución a la [prueba técnica](https://sportenlace-my.sharepoint.com/personal/y_carmona_inlaze_com/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fy%5Fcarmona%5Finlaze%5Fcom%2FDocuments%2FTalento%20Humano%20%28Contrataci%C3%B3n%29%2FDOCUMENTOS%20EMPLEADOS%2FSPORT%20ENLACE%20%20NUEVOS%20CONTRATOS%2F11%5FPRUEBAS%20Y%20PERFILES%2FPRUEBAS%2FPrueba%20T%C3%A9cnica%20%2D%20Analista%20de%20Requerimientos%2Epdf&parent=%2Fpersonal%2Fy%5Fcarmona%5Finlaze%5Fcom%2FDocuments%2FTalento%20Humano%20%28Contrataci%C3%B3n%29%2FDOCUMENTOS%20EMPLEADOS%2FSPORT%20ENLACE%20%20NUEVOS%20CONTRATOS%2F11%5FPRUEBAS%20Y%20PERFILES%2FPRUEBAS&ga=1&LOF=1), organizada en las siguientes secciones:

## Índice
1. [Requerimientos Funcionales](./Requerimientos.md)
2. [Casos de Uso](./Casos_de_Uso.md)
3. [Propuesta de Herramientas](./Herramientas.md)
4. [Preguntas Conceptuales](./Preguntas_Conceptuales.md)
5. [Correo al Cliente](./Correo_Cliente.md)

## Casos de Uso

A continuación, se presentan dos casos de uso críticos para el funcionamiento de la plataforma:

### 1. Caso de Uso 1: Gestión de Transacciones (Depósitos y Retiros)

- **Nombre:** Gestión de Transacciones (Depósitos y Retiros)
- **Descripción:** Permite a los usuarios realizar depósitos y retiros de manera segura, confiable y cumpliendo con normativas financieras.
- **Actores:** Usuario, Pasarela de Pago, Administrador del Sistema.
- **Flujo Principal:**
    1. El usuario inicia sesión en la plataforma.
    2. Selecciona la opción de depósito o retiro en su cuenta.
    3. Ingresa el monto y método de pago (tarjeta, transferencia, etc.).
    4. El sistema valida la identidad del usuario y los fondos disponibles.
    5. Se redirige a la pasarela de pago para completar la transacción.
    6. El sistema confirma la transacción y actualiza el saldo del usuario.
    7. Notifica al usuario el resultado de la operación.
- **Flujo Alternativo:**
    - Si la pasarela rechaza la transacción, se muestra un mensaje de error y se solicita al usuario corregir sus datos o elegir otro método de pago.

### 2. Caso de Uso 2: Juego en Línea (Ruleta o Blackjack)

- **Nombre:** Juego en Línea (Ruleta o Blackjack)
- **Descripción:** Los usuarios pueden acceder y jugar ruleta o blackjack en tiempo real, generando apuestas y recibiendo resultados instantáneos.
- **Actores:** Usuario, Sistema de Juegos (servidor de juegos), Administrador del Sistema.
- **Flujo Principal:**
    1. El usuario inicia sesión y selecciona el juego (ruleta o blackjack).
    2. El sistema carga la interfaz interactiva (desarrollada en React/JSX, por ejemplo).
    3. El usuario ingresa su apuesta y confirma la jugada.
    4. El sistema valida que el usuario cuente con saldo suficiente.
    5. Se genera un resultado usando un RNG certificado.
    6. Se muestra el resultado al usuario y se actualiza el saldo si hay ganancias/pérdidas.
- **Flujo Alternativo:**
    - Si el usuario no cuenta con suficiente saldo, el sistema alerta y ofrece la opción de depositar fondos antes de continuar.
