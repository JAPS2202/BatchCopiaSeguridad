# BatchCopiaSeguridad

@echo off
REM Definir los directorios de origen y destino
set "origen=C:\Users\javie\OneDrive\Documentos\OctavoSemestre"
set "destino=C:\Users\javie\OneDrive\Documentos\CopiaDeSeguridad2"

REM Crear la carpeta de destino si no existe
if not exist "%destino%" mkdir "%destino%"

REM Copiar los archivos al destino
echo Realizando copia de seguridad...
xcopy "%origen%" "%destino%" /s /e /y
echo Copia de seguridad completada.
