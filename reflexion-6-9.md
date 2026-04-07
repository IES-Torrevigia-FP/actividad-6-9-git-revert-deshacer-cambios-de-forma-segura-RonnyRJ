git reset es un viaje al pasado: mueve la rama hacia atrás para eliminar commits. Es como si borraras páginas de un libro de historia.

git revert es un parche hacia adelante: crea un commit nuevo que deshace los cambios de uno anterior. Es como añadir una página nueva al libro explicando que el capítulo anterior fue un error.

Situaciones para preferir git revert

En ramas compartidas (main/develop): Cuando el error ya ha sido subido a GitHub y otros compañeros lo han descargado.
Si quieres mantener el rastro: Cuando necesitas que en el historial quede constancia de que hubo un error y cómo se solucionó, sin que desaparezca nada.

Se dice que es un deshacer hacia adelante porque no altera los commits ya existentes; simplemente añade uno nuevo al final de la línea.

Importancia en proyectos compartidos:

Evita conflictos: Al no reescribir la historia, los repositorios de tus compañeros no se "rompen" ni entran en conflicto al hacer git pull.
Sincronización: Es una operación aditiva, lo que garantiza que todos sigan teniendo un historial lineal y coherente sin necesidad de usar comandos forzados o peligrosos.
