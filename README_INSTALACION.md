# 🎨 PACK DE TEXTURAS & MENÚS DE SKILLS (CRAZY SURVIVAL)

Este paquete contiene la suite completa y aislada de interfaces visuales (GUIs), iconos, modelos CustomModelData, glifos de espaciado negativo y menús interactivos para el sistema de Habilidades (Skills) de Crazy Survival.

---

## 📁 ESTRUCTURA DEL PAQUETE

```
textura skills crazy survival.zip/
│
├── 1_DeluxeMenus/
│   ├── config_deluxemenus_addon.yml  <-- Bloque para agregar a config.yml
│   └── gui_menus/
│       └── skills/
│           ├── skills_main.yml        <-- Menú principal de habilidades (/skills)
│           ├── stats.yml              <-- Menú de atributos y estadísticas
│           └── leaderboards.yml       <-- Top y clasificaciones con texturas
│
├── 2_AuraSkills_Menus/                <-- Menús nativos compatibles con AuraSkills
│   ├── skills.yml
│   ├── stats.yml
│   ├── level_progression.yml
│   ├── abilities.yml
│   ├── sources.yml
│   ├── stat_info.yml
│   └── leaderboard.yml
│
├── 3_Java_ResourcePack/
│   └── resource.zip                   <-- Resource Pack aislado para Minecraft Java (1.20 - 1.21+)
│
├── 4_Bedrock_ResourcePack/
│   └── skills_bedrock.mcpack          <-- Resource Pack optimizado para Bedrock / Geyser / Floodgate
│
└── README_INSTALACION.md
```

---

## 🛠️ GUÍA DE INSTALACIÓN

### 1. DeluxeMenus
1. Copia la carpeta `1_DeluxeMenus/gui_menus/skills/` en la ruta de tu servidor:
   `plugins/DeluxeMenus/gui_menus/skills/`
2. Abre `plugins/DeluxeMenus/config.yml` y copia el contenido de `config_deluxemenus_addon.yml` bajo la sección `gui_menus:`.
3. Ejecuta en consola: `/dm reload`.

### 2. AuraSkills (Opcional si usas los menús nativos del plugin)
1. Copia los archivos YAML de `2_AuraSkills_Menus/` en `plugins/AuraSkills/menus/`.
2. Ejecuta en consola: `/skills reload`.

### 3. Java Resource Pack (`resource.zip`)
- **Para jugadores locales:**
  Coloca `resource.zip` en tu carpeta `.minecraft/resourcepacks/` y actívalo en el menú de Recursos.
- **Para servidor (Server Resource Pack):**
  Sube `resource.zip` a tu hosting o CDN (Dropbox, MCPacks, etc.) y configura el enlace y hash SHA-1 en `server.properties` o en tu plugin de ResourcePack (ForcePack, ItemsAdder, etc.).

### 4. Bedrock / Geyser Resource Pack (`skills_bedrock.mcpack`)
- **Para jugadores de Bedrock (móvil, Windows, consolas):**
  Simplemente abre o haz doble clic en `skills_bedrock.mcpack` para que Minecraft Bedrock lo importe automáticamente.
- **Para Geyser / Floodgate en servidor:**
  Coloca `skills_bedrock.mcpack` en `plugins/Geyser-Spigot/packs/` (o la carpeta `packs/` de Geyser Standalone/Velocity) y reinicia Geyser para que se envíe automáticamente a todos los jugadores de Bedrock.

---

## 🔍 CARACTERÍSTICAS TÉCNICAS
- **Glifos Unicode Personalizados:**
  - `\ue0be`: Textura de fondo Menú Principal de Skills.
  - `\ue0bf`: Textura de fondo Estadísticas (Stats).
  - `\ue0c0`: Textura de fondo Clasificación (Leaderboards).
  - `\ue0c1`: Textura de fondo Progresión de Nivel (Level).
  - `\ue0c2`: Textura de fondo Fuentes de XP (Sources).
  - `\ue0c3`: Textura de fondo Habilidades activas/pasivas (Abilities).
  - `七`: Glifo de espaciado negativo (offset de alineación GUI pixel-perfect).
- **CustomModelData:** Asignado en el rango 76 al 116 para todos los iconos de habilidades y controles.
