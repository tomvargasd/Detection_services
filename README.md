# Sistema de reconocimiento

## Estructura del proyecto
- Módulos
  - reconocimiento_facial
    - static
    - templates
    - app.py
    - ...
    - tests
      - test01_create_profile.py
      - test02_asign_capture_to_profile.py
      - test03_recognition_faces.py
      - ...
      - test.py
- Configs
  - database.py
  - settings.py
- Screens
  - login.py
  - register.py
  - profile.py
  - index.py
- scripts
  - create_user.py
- main.py
- .gitignore
- venv
- README.md


## Descripción
main.py levanta una ventana tkinter con un inicio de sesion, luego de entrar se muestran todos los módulos disponibles en orden en forma de cartas en index.

Esta ventana de módulos (index.py) debe de tener un bonton para acceder a perfil, otro para registro y despues todos los modulos disponibles.

Perfil (profile.py) se podrá ver una lista de usuarios y los datos del usuario actual debe haber un boton para registrar usuario.

Registro (register.py) podrá registrar un nuevo usuario y al terminar regresar a index.py.

### Indicaciones
* Cada carta de módulo será como activacion de servicio, al dar clic en una carta de modulo debe consultar si desea iniciar el módulo.
* Cada modulo si esta activo dentro debe haber un boton para acceder al modulo (abre navegador web con el link del modulo activado)
* Cada carta de modulo debe tener un indicador para saber si el servicio esta activo o no.
* Cada carta al dar clic y si el servicio esta activo debe consultar si desea detenerlo.
* El servicio debe levantarse dinamicamente si un puerto esta siendo usado por otro modulo debe intentar con otro puerto hasta que pueda levantarse.
* todos los datos de esta aplicacion tkinter deben almacernarse en una base de datos sqlite.
* Debe permitir cerrar sesion.
* Si se cierra sesion debe confirmarse para detener todos los servicios antes.
* Si se intenta cerrar la aplicacion de cualquier metodo debe pedir confirmacion antes para poder terminar o cerrar todos los procesos activos.

