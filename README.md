# Levantar proyecto: 

## 1. Instalar dependencias:
```npm install```

## 2. Ejecutar el proyecto:
```npm run dev```


# Configuración de formateo:

Para estandarizar los estilos de formato de código con ESLint + Prettier y evitar cambios innecesarios en el formato cuando múltiples desarrolladores trabajan en un proyecto, se pueden seguir estos pasos:

# 1. Instalar la extensión Prettier.

# 2. Configurar ESlint: Ajustar el archivo .eslint.config.js para incluir Prettier:

```json
{
  "extends": ["eslint:recommended", "plugin:prettier/recommended"],
  "rules": {
    "prettier/prettier": ["error", { "endOfLine": "auto" }]
  }
}
```

# 3. Configurar Prettier: Crear un archivo .prettierrc con las configuraciones de Prettier:

```json
{
  "semi": true,
  "singleQuote": false,
  "printWidth": 80,
  "trailingComma": "es5"
}
```

# 4. Ajustar las reglas de Prettier según las necesidades del proyecto y verificar el formato de código.