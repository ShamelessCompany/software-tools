# software-tools

Repositorio de Shameless Company para el desarrollo de herramientas de software, bots, scrapers y paginas web enfocadas en resolver tareas repetitivas o generar ingresos por afiliados y micro-servicios.

## Objetivo del repositorio
Construir utilidades de software practicas y ligeras que no dependan de servidores costosos. Todo lo que se desarrolle aqui debe correr bajo servicios gratuitos en la nube (como Cloudflare Pages/Workers o servidores propios) y resolver un problema concreto que alguien este dispuesto a pagar o que atraiga trafico util.

---

## Ideas de proyectos y requisitos de MVP

### 1. Portales web de comparacion de precios de software
- Que es: Paginas web que ensenan como cambian los precios de suscripcion de las herramientas digitales segun el pais y proponen alternativas mas baratas o de codigo abierto.
- Como genera dinero: Enlaces de afiliados de servicios de privacidad, VPNs y alternativas de software.
- Requisitos de MVP:
  1. Sitio web estatico construido en Astro y alojado en Cloudflare Pages sin pagar mensualidad.
  2. Archivo de datos en JSON con los precios de al menos 10 herramientas conocidas en 5 paises distintos.
  3. Enlaces funcionales con etiqueta de afiliado y botones para filtrar por categoria.

### 2. Bots de alertas financieras en Telegram
- Que es: Un script en Python que monitorea movimientos de acciones o criptomonedas y avisa al instante por Telegram cuando se cumple una condicion tecnica (como una ruptura de soporte o una caida rapida).
- Como genera dinero: Ofrecer un canal publico gratuito para ganar audiencia y un canal privado con suscripcion mensual para senales instantaneas.
- Requisitos de MVP:
  1. Script en Python que consulte precios de mercado cada minuto usando librerias gratuitas como yfinance o ccxt.
  2. Bot de Telegram configurado que reciba la orden y envie el mensaje con el precio y la grafica basica en menos de 5 segundos.
  3. Poner a correr el script en un servidor propio o instancia gratuita para que no se apague durante el dia.

### 3. Monitor de pasarelas de pago colombianas
- Que es: Un bot con Playwright que entra a tiendas de comercio electronico cada 5 minutos, hace una prueba de compra simulada y revisa si botones como Wompi o PSE estan respondiendo bien.
- Como genera dinero: Cobro de una cuota mensual a duenos de tiendas locales para avisarles por Telegram o WhatsApp si su pasarela se cae antes de que pierdan clientes.
- Requisitos de MVP:
  1. Script que abra un navegador en segundo plano, agregue un producto de prueba al carrito y confirme que la pasarela de pago abre sin errores.
  2. Alerta automatica que mande un mensaje de emergencia si la pasarela tarda mas de 10 segundos en responder o si tira error 500.
  3. Guardar un registro de pruebas exitosas y fallidas en un archivo local o base de datos ligera.

### 4. Micro-APIs de utilidades rapidas
- Que es: Funciones en la nube que hacen una sola cosa en milisegundos, como armar facturas en PDF a partir de datos limpios o verificar si la direccion de un correo de empresa tiene servidor activo.
- Como genera dinero: Publicar los servicios en RapidAPI o vender llaves prepago en paquetes pequenos (por ejemplo: 10 dolares por cada 2,500 consultas).
- Requisitos de MVP:
  1. Funcion en Cloudflare Workers que tome datos en JSON y devuelva un PDF terminado en menos de 100 milisegundos.
  2. Control basico de acceso con una clave para descontar saldo por cada peticion procesada.
  3. Ejemplo claro de codigo en una sola pagina que muestre como conectar la funcion en JavaScript y Python.

### 5. Bots de RPA para procesos de oficina y negocios
- Que es: Scripts que leen datos de hojas de calculo y los pasan automaticamente a sistemas viejos de facturacion o paginas del gobierno que no tienen conexion directa por API.
- Como genera dinero: Cobrar por la creacion e instalacion del bot a pequenas empresas (clinicas, consultorios, firmas contables) que gastan horas metiendo datos a mano.
- Requisitos de MVP:
  1. Script en Python que lea una tabla con 10 filas de prueba y llene los campos de un formulario web sin intervencion humana.
  2. Sistema de control que si una fila falla por datos incompletos, siga con las demas y cree un archivo de texto con las filas que tuvieron problemas.
  3. Archivo ejecutable o script que el cliente pueda correr haciendo doble clic en su computador.
