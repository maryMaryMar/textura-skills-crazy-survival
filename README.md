# Texturas y Menus de Skills - Crazy Survival

Paquete de recursos visuales y configuraciones para el sistema de habilidades de Crazy Survival.

## Contenido del paquete

1. 1_DeluxeMenus
   - skills_main.yml: Menu principal de habilidades con soporte de glifos.
   - stats.yml: Menu de estadisticas y atributos.
   - leaderboards.yml: Clasificaciones con paginacion.
   - config_deluxemenus_addon.yml: Fragmento para registrar en config.yml.

2. 2_AuraSkills_Menus
   - Menus nativos compatibles con el plugin AuraSkills (skills, stats, level_progression, abilities, sources, stat_info, leaderboard).

3. 3_Java_ResourcePack
   - resource.zip: Resource Pack para Minecraft Java (versiones 1.20 a 1.21+). Incluye fuentes unicode, offsets negativos y modelos CustomModelData (76 al 116).

4. 4_Bedrock_ResourcePack
   - skills_bedrock.mcpack: Pack para Minecraft Bedrock y servidores con Geyser/Floodgate.

5. Archivo comprimido completo
   - textura skills crazy survival.zip: Contiene todos los directorios y archivos anteriores en un solo archivo.

## Instalacion

- DeluxeMenus: Colocar la carpeta 1_DeluxeMenus/gui_menus/skills en plugins/DeluxeMenus/gui_menus/ y agregar el bloque de config_deluxemenus_addon.yml en config.yml. Recargar con /dm reload.
- AuraSkills: Colocar los archivos de 2_AuraSkills_Menus en plugins/AuraSkills/menus/. Recargar con /skills reload.
- Java Resource Pack: Instalar resource.zip en .minecraft/resourcepacks o definirlo en server.properties.
- Bedrock Resource Pack: Abrir skills_bedrock.mcpack directamente en el cliente Bedrock o colocarlo en la carpeta packs de Geyser-Spigot.
