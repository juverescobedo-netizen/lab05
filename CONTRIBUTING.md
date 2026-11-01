# Guia para contribuir

Gracias por interesarte en mejorar Tienda TECSUP. Este documento explica cómo reportar un problema, proponer una mejora y enviar cambios fáciles de revisar.

## Antes de colaborar

1. Comprueba que puedes abrir `index.html` en un navegador.
2. Revisa los archivos relacionados con tu cambio antes de editar.
3. Si el proyecto está alojado en GitHub, trabaja en tu fork y no hagas cambios directamente en el repositorio original.

## Reportar un error

Abre un Issue e incluye la información necesaria para reproducir el problema:

- **Título:** una frase corta y específica.
- **Comportamiento esperado:** qué debería ocurrir.
- **Comportamiento actual:** qué ocurre en realidad.
- **Pasos para reproducirlo:** instrucciones ordenadas.
- **Entorno:** navegador y sistema operativo, si son relevantes.
- **Evidencia:** captura de pantalla o mensaje de error, cuando ayude.

Ejemplo de título: `El total del carrito no multiplica el precio por la cantidad`.

## Proponer una mejora

Antes de realizar una mejora grande, crea un Issue para explicar el problema que resolvería y discutir la idea. Incluye el beneficio para el usuario y, si es posible, una propuesta concreta. Para cambios pequeños de documentación, puedes abrir directamente un Pull Request.

## Preparar el entorno

Clona tu fork y entra en la carpeta del proyecto:

```bash
git clone https://github.com/TU-USUARIO/tienda-tecsup.git
cd tienda-tecsup
```

Cambia `TU-USUARIO` por tu nombre de usuario de GitHub. Abre `index.html` en un navegador para comprobar el resultado; no se necesita un servidor de aplicaciones para esta práctica.

## Ramas y commits

Crea una rama descriptiva desde la rama principal actualizada. Usa prefijos como `fix/` para corregir errores, `feat/` para nuevas funciones y `docs/` para documentación.

```bash
git switch main
git pull origin main
git switch -c fix/descripcion-breve
```

Usa mensajes de commit claros, preferiblemente con un prefijo:

- `fix: calcula el total según la cantidad`
- `feat: valida la cantidad de productos`
- `docs: mejora las instrucciones de instalacion`

Mantén cada commit enfocado en un solo propósito. Antes de confirmarlo, revisa `git status` y `git diff`.

## Enviar un Pull Request

1. Comprueba el cambio localmente en el navegador.
2. Sube tu rama al fork con `git push -u origin nombre-de-tu-rama`.
3. Abre un Pull Request hacia el repositorio correcto.
4. Explica qué cambiaste, por qué era necesario y cómo lo probaste.
5. Incluye el número del Issue relacionado, si existe.
6. Añade capturas cuando el cambio modifique la apariencia de la página.

## Checklist del Pull Request

Antes de solicitar una revisión, confirma lo siguiente:

- [ ] El cambio resuelve un problema concreto o mejora la documentación.
- [ ] Probé la página en un navegador y comprobé que no aparezcan errores nuevos.
- [ ] Los estilos se cargan correctamente desde `estilos.css`.
- [ ] El total del carrito multiplica cada precio por su cantidad.
- [ ] Revisé `git diff` y solo incluí archivos relacionados con el cambio.
- [ ] Los nombres de archivos, variables y funciones son claros.
- [ ] El Pull Request explica el cambio e incluye el Issue asociado, si corresponde.
- [ ] Actualicé el `README.md` si la modificación cambia la instalación, el uso o las funciones.

## Estilo de trabajo

- Conserva la separación entre HTML, CSS y JavaScript.
- Mantén la indentación y el estilo ya utilizado en cada archivo.
- Evita añadir dependencias innecesarias para una funcionalidad pequeña.
- No incluyas contraseñas, tokens ni otros datos privados en los archivos o commits.
- Sé respetuoso y específico al comentar cambios o sugerencias.
