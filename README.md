VIDPASE V4.2 — VIDEO ALTERNATIVO DE RESPALDO

1. Sube a GitHub los archivos públicos del ZIP.
2. Como cambió validateScreenshot, abre PowerShell en la carpeta descomprimida.
3. Ejecuta:

   cd functions
   npm.cmd install
   cd ..
   firebase.cmd deploy --only functions:validateScreenshot,firestore:rules

FUNCIONAMIENTO:
- En el editor activa “Video alternativo de respaldo”.
- Selecciona otra campaña publicada.
- Si el visitante no encuentra el video principal, podrá usar el alternativo.
- La captura se valida contra el video realmente utilizado.
- El contenido final siempre pertenece al enlace principal.
- Las ideas de comentarios se toman automáticamente de la campaña usada como video alternativo y continúan siendo opcionales.
