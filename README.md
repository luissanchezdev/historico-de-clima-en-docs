# Historico de clima

![Workflow N8N]('./images/workflow.png')

## Credenciales necesarias en n8n:

- Google Outh2:
  - Ir a Google Cloud Console
  - Crear un nuevo proyecto
  - Agregar el permiso de acceso a Drive y Sheets
  - Crear una nueva credencial del tipo OAuth2:
    - Agregar el callback url que indica n8n en el siguiente paso
  - Ir a n8n y agregar una nueva credencial:
    - Seleccionar Google OAuth2 API
    - Copiar el callback url indicado y agregarlo en la configuración de la credencial del proyecto de Google Cloud Console, finalizando así la configuración de la credencial
    - Agregar el 'Id de cliente' de la credencial configurada de Google Cloud Console
    - Agregar el 'Secreto de cliente' de la credencial configurada de Google Cloud Console
    - Agregar el scoope:
```bash
https://www.googleapis.com/auth/spreadsheets
https://www.googleapis.com/auth/drive.file
```

# Api de OpenWeatherMaps
  - Crea una nueva cuenta
  - Confirma el correo
  - Crea una nueva api key desde la cuenta de OpenWeatherMaps
  - En n8n agrega una nueva credencial:
    - Selecciona OpenWeatherMaps y agrega en el campo 'Access Token' la API key suministrada por OpenWeatherMaps
  **Nota**: A veces se demora en estar habilitada la api key, testear varias veces

Disfruta

**By Luissdev**