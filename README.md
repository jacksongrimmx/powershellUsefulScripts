Lista todos los archivos dentro de una carpeta sin imporntar en que directorio se encuentren derivado de un parametro.

Get-ChildItem -Recurse -File | Select-String -Pattern "plat" -CaseSensitive:$false | Select-Object Filename, LineNumber, Line
