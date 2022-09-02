1. Tailwind not working
  - Content config in tailwind.config.js
  - @tailwind in global.css & link global.css to _app.tsx
2. Prettier config sort import order
  - Run command `yarn add -D @trivago/prettier-plugin-sort-imports@2.0.4`
  - Add to .prettierrc: 
  `{
  "parser": "typescript",
  "printWidth": 120,
  "semi": true,
  "singleQuote": true,
  "trailingComma": "es5",
  "tabWidth": 2,
  "bracketSpacing": true,
  "bracketSameLine": true,
  "arrowParens": "avoid",
  "importOrder": [
    "^react/",
    "^next/",
    "^[base, model, theme, consts, hook, utils]",
    "^[component]",
    "^[./]"
  ],
  "importOrderSeparation": true
}`
