# 🛒 SauceDemo - Plataforma de Compras en Línea

![SauceDemo Logo](https://www.saucedemo.com/static/media/logo3x.7e5500cf.png)

## 📄 Descripción

**SauceDemo** es una plataforma de pruebas diseñada para demostrar diferentes escenarios en un entorno de comercio electrónico. Aquí, los usuarios pueden iniciar sesión con varios perfiles, agregar productos al carrito, y realizar simulaciones de compra. Es una excelente herramienta para realizar pruebas de automatización y validación de aplicaciones web.

## 🚀 Características Principales

- 🧑‍💻 **Múltiples Perfiles de Usuario**: Inicia sesión con diferentes perfiles de usuario como `standard_user`, `locked_out_user`, `problem_user`, y `performance_glitch_user`.
- 🛒 **Simulación de Compra**: Agrega productos al carrito y realiza el proceso completo de compra.
- 📦 **Gestión de Carrito**: Revisa y administra los productos en tu carrito de compras.
- 🔍 **Pruebas de Rendimiento**: Evalúa el rendimiento del sitio web bajo diferentes condiciones de usuario.

## 🖥️ Demo en Vivo

Visita la página en vivo en [SauceDemo](https://www.saucedemo.com/).

## 🧑‍🔬 Usuarios de Prueba

A continuación, se proporcionan algunos usuarios de prueba que puedes utilizar para explorar la aplicación:

- **standard_user**
- **locked_out_user**
- **problem_user**
- **performance_glitch_user**

La contraseña para todos los usuarios es: `secret_sauce`.

## 📸 Capturas de Pantalla

### Página de Inicio de Sesión
![Login Page](https://www.saucedemo.com/static/media/sauce-backpack-1200x1500.34e7aa42.jpg)

### Página de Productos
![Inventory Page](https://www.saucedemo.com/static/media/bolt-shirt-1200x1500.c0dae290.jpg)

### Proceso de Checkout
![Checkout Page](https://www.saucedemo.com/static/media/red-onesie-1200x1500.ec61476e.jpg)

## 🛠️ Tecnologías Utilizadas

- **Frontend**: HTML5, CSS3, JavaScript
- **Backend**: Simulación de Backend para pruebas
- **Testing**: Compatible con herramientas de automatización como Cypress, Selenium, y más.

## ⚙️ Instalación y Configuración

Para usar esta plataforma con fines de prueba, simplemente sigue estos pasos:

1. Clona el repositorio de SauceDemo (si es necesario).
   ```bash
   git clone https://github.com/tu-usuario/saucedemo.git

2. Navega al directorio del proyecto.
   ```bash
cd saucedemo

3. Abre index.html en tu navegador para comenzar.

## 🔍 Pruebas y Automatización
SauceDemo es ideal para pruebas de automatización. Puedes usar Cypress, Selenium, u otras herramientas de prueba para simular el proceso de compra. Aquí tienes un ejemplo simple con Cypress:

describe('Prueba de Login', () => {
  it('Debería iniciar sesión correctamente con standard_user', () => {
    cy.visit('https://www.saucedemo.com/');
    cy.get('#user-name').type('standard_user');
    cy.get('#password').type('secret_sauce');
    cy.get('#login-button').click();
    cy.url().should('include', '/inventory.html');
  });
});
