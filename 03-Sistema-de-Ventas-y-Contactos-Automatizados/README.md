# ⚡ CRM inteligente y distribuidor de propuestas

## 📄 Descripción general
Un motor de automatización híbrido que convierte una hoja de cálculo estática de Google en un CRM dinámico. Este sistema supervisa el estado de los clientes potenciales en tiempo real y activa secuencias de correos electrónicos personalizados, enviando precios, carteras o seguimientos al instante basándose en puertas lógicas específicas.

## 🎯 El problema
Los equipos de ventas se enfrentan a dos obstáculos operativos principales:
1.  **Velocidad de respuesta:** enviar manualmente una propuesta dos horas después de recibir una solicitud reduce drásticamente las tasas de conversión.
2.  **Caos en las hojas de cálculo:** realizar un seguimiento de «A quién envié el correo electrónico?» y «Qué PDF envié?» en una hoja estática da lugar a errores y contactos duplicados.

## 💡 La solución
He creado un flujo de trabajo condicional en **Make.com** que actúa como un gestor de operaciones de ventas automatizado:

1.  **Supervisa la base de datos:** supervisa una hoja maestra de Google para detectar cambios de estado (por ejemplo, cuando un cliente potencial pasa a *«Cualificado»* o *«Enviar presupuesto»*).
2.  **Aplica la lógica empresarial:** verifica las condiciones antes de actuar (por ejemplo, *Es válido el correo electrónico? ¿Ya se ha enviado la propuesta?*).
3.  **Selección dinámica de activos:** extrae automáticamente el PDF correcto (propuesta A frente a propuesta B) en función del sector del cliente.
4.  **Ejecuta y actualiza:** envía el correo electrónico personalizado a través de Gmail y **marca inmediatamente la hoja de cálculo** con la «fecha del último contacto» para mantener la higiene de los datos.

## 🛠️ Pila tecnológica
* **Make.com** (lógica de enrutamiento y gestión de errores)
* **Hojas de cálculo de Google** (base de datos y fuente de activación)
* **API de Gmail** (envío con alta capacidad de entrega)
* **Notion** (gestión de activos adicionales)

## 📸 Flujo de trabajo y lógica

### 1. El núcleo lógico (Make.com)
El flujo de trabajo utiliza módulos de enrutador para dividir el tráfico. Distingue entre un «nuevo cliente potencial» que necesita un folleto y un «seguimiento» que necesita un recordatorio solo de texto.
<img width="960" height="410" alt="2025-12-06 (10)" src="https://github.com/user-attachments/assets/736c7f97-7623-42bf-b62a-6bcc7a9f51cb" />


### 2. El resultado (bandeja de entrada del cliente)
Un correo electrónico totalmente personalizado con el archivo adjunto correcto, entregado segundos después del desencadenante.
<img width="960" height="407" alt="2025-12-07 (5)" src="https://github.com/user-attachments/assets/ce6589f7-a5f5-4638-8271-0191ee2694ba" />


## 📬 Contact

--Gabriel Elias Flores--
Linkedin: https://www.linkedin.com/in/gabriel-elias-flores-440413342
Email: gabrielias28e@gmail.com


---
