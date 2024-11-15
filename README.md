# Portif-lioportfolio/
├── public/                # Arquivos estáticos (favicon, imagens)
├── src/
│   ├── assets/            # Imagens, ícones, etc.
│   ├── components/        # Componentes reutilizáveis
│   │   ├── Header.jsx
│   │   ├── Footer.jsx
│   │   ├── PortfolioCard.jsx
│   ├── pages/             # Páginas principais
│   │   ├── Home.jsx
│   │   ├── About.jsx
│   │   ├── Projects.jsx
│   ├── styles/            # CSS ou SASS
│   │   ├── global.css
│   │   ├── theme.css
│   ├── utils/             # Helpers ou funções utilitárias
│   ├── App.jsx
│   ├── index.jsx
├── .gitignore
├── package.json
├── README.md

import React from "react";
import "./PortfolioCard.css";

const PortfolioCard = ({ title, description, image }) => (
  <div className="portfolio-card">
    <img src={image} alt={title} className="portfolio-image" />
    <h3>{title}</h3>
    <p>{description}</p>
  </div>
);

export default PortfolioCard;
