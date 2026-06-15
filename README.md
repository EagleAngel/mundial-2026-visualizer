# 🌍 Mundial 2026 - Visualizador de Resultados con Quiniela

Una aplicación web interactiva para visualizar resultados del Mundial 2026 con sistema de quiniela integrado y generador de chistes como bonus.

## ✨ Características Principales

### 🎯 Quiniela
- 12 participantes con equipos asignados
- Ranking en vivo actualizado automáticamente
- Sistema de puntuación en tiempo real
- Seguimiento de equipos eliminados
- Interfaz visual atractiva

### ⚽ Partidos
- Visualización de partidos del Mundial 2026
- Partidos en vivo con actualizaciones automáticas
- Filtrado por grupo y fase
- Información detallada de cada partido

### 😂 Generador de Chistes
- API externa integrada (JokeAPI)
- Múltiples categorías (General, Programación, Knock-Knock, Aleatorio)
- Copiar chistes al portapapeles
- Contador de chistes generados
- Animaciones suaves

## 👥 Participantes de la Quiniela

| # | Participante | Equipos |
|---|---|---|
| 1 | 👨 Jose Primo | Ghana, Algeria, England, Uruguay |
| 2 | 👴 Tío Pepe | Côte d'Ivoire, Senegal, Sweden, Argentina |
| 3 | 🎓 Maestro Asel | Curaçao, Croatia, Brazil, Saudi Arabia |
| 4 | 👩 Marialaura | South Africa, Norway, New Zealand, Iran |
| 5 | 😇 Angel | Spain, Australia, Tunisia, Cabo Verde |
| 6 | 👩 Laura | Bosnia and Herzegovina, Ecuador, Iraq, Switzerland |
| 7 | 👩 Vane | South Korea, Portugal, Democratic Republic of the Congo, Colombia |
| 8 | 👩 Andrea | Egypt, Canada, Austria, Mexico |
| 9 | 👩 Sofi | Jordan, Uzbekistan, Panama, Scotland |
| 10 | 👩 Meche | Belgium, Haiti, Paraguay, United States |
| 11 | 👨 Uriel | Turkey, Germany, Qatar, Morocco |
| 12 | 👩 Karla | France, Czech Republic, Japan, Netherlands |

**🏆 REGLA**: ¡Gana quien tenga uno de sus equipos que gane el Mundial!

## 🚀 Inicio Rápido

### Requisitos
- Node.js 16+
- npm o yarn

### Instalación

```bash
# Clonar repositorio
git clone https://github.com/EagleAngel/mundial-2026-visualizer.git
cd mundial-2026-visualizer

# Instalar dependencias
npm install

# Configurar variables de entorno
cp .env.example .env

# Obtener API Key (opcional)
# Ve a: https://rapidapi.com/api-sports/api/api-football
# Copia tu API Key en .env

# Iniciar servidor de desarrollo
npm run dev

# Abre: http://localhost:5173
```

## 🛠️ Tecnologías

- **React 18** - Framework UI
- **TypeScript** - Tipado estático
- **Vite** - Build tool
- **Tailwind CSS** - Estilos
- **Framer Motion** - Animaciones
- **Zustand** - State management
- **Axios** - HTTP client
- **JokeAPI** - API de chistes
- **API-Football** - Datos del fútbol

## 📁 Estructura del Proyecto

```
src/
├── components/
│   ├── Header.tsx
│   ├── QuinielaRanking.tsx
│   └── JokeGenerator.tsx
├── data/
│   └── participants.ts
├── services/
│   └── api.ts
├── store/
│   └── gameStore.ts
├── types/
│   └── index.ts
├── App.tsx
├── main.tsx
└── index.css
```

## 📊 Cómo Funciona

### Sistema de Puntuación

Cada participante gana puntos según el desempeño de sus equipos:
- **Victoria**: +3 puntos
- **Empate**: +1 punto
- **Derrota**: 0 puntos

### Ranking

- Se actualiza automáticamente después de cada partido finalizado
- Muestra posición, puntos y victorias
- Indica equipos eliminados con línea a través
- El líder brilla con animaciones especiales

## 🎮 Uso del Generador de Chistes

1. Selecciona una categoría (Aleatorio, General, Programación, Knock-Knock)
2. Haz clic en "Nuevo Chiste"
3. Lee y disfruta del chiste 😂
4. Usa "Copiar" para compartir con amigos

## 🚀 Build para Producción

```bash
npm run build
npm run preview
```

## 📝 Variables de Entorno

```env
# .env
VITE_RAPIDAPI_KEY=tu_api_key_aqui
VITE_RAPIDAPI_HOST=api-football-v1.p.rapidapi.com
```

## ⚙️ Configuración

### Agregar más participantes
Edita `src/data/participants.ts` y agrega nuevos participantes al array `PARTICIPANTS`.

### Cambiar categorías de chistes
Modifica las categorías en `src/components/JokeGenerator.tsx` en el array de botones.

## 📱 Responsive Design

- ✅ Desktop (1920px+)
- ✅ Tablet (768px - 1024px)
- ✅ Mobile (< 768px)

## 🌐 Deployment

### Vercel
```bash
npm i -g vercel
vercel
```

### Netlify
```bash
npm i -g netlify-cli
netlify deploy --prod --dir=dist
```

## 🐛 Troubleshooting

### Problemas con la API de fútbol
- Verifica que tu API Key sea válida
- Comprueba el límite de llamadas (free tier tiene límite)
- Los datos mock se mostrarán si la API falla

### Chistes no cargan
- Verifica tu conexión a internet
- JokeAPI puede estar temporalmente fuera de servicio
- Intenta con una categoría diferente

## 🤝 Contribuir

```bash
git checkout -b feature/amazing-feature
git commit -m 'Add amazing feature'
git push origin feature/amazing-feature
```

## 📄 Licencia

MIT © 2026

## 👨‍💻 Autor

Creado por **EagleAngel** 🦅

## 🙏 Agradecimientos

- [API-Football](https://www.api-football.com/)
- [JokeAPI](https://jokeapi.dev/)
- [Framer Motion](https://www.framer.com/motion/)
- [Tailwind CSS](https://tailwindcss.com/)

---

⭐ Si te gusta, ¡dale una estrella!

**¡Que gane el mejor! 🎉⚽🏆**