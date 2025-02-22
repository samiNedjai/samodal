# 🏆 Samodal-React

**Samodal-React** est un composant **modale personnalisable pour React**, facile à intégrer et réutilisable.

![npm](https://img.shields.io/npm/v/samodal-react?style=flat-square)
![license](https://img.shields.io/npm/l/samodal-react?style=flat-square)
![issues](https://img.shields.io/github/issues/samiNedjai/samodal?style=flat-square)

---

## 📌 Installation

Installe le package via npm :

```sh
npm install samodal-react
```

Ou avec Yarn :

```sh
yarn add samodal-react
```

## 📌 Utilisation

Voici un exemple simple pour afficher une modale :

```jsx
import React, { useState } from "react";
import Modal from "samodal-react";

const App = () => {
  const [isOpen, setIsOpen] = useState(false);

  return (
    <div>
      <button onClick={() => setIsOpen(true)}>Open Modal</button>
      <Modal isOpen={isOpen} onClose={() => setIsOpen(false)} title="My Modal">
        <p>This is a reusable modal component.</p>
      </Modal>
    </div>
  );
};

export default App;
```

## 📌 Props disponibles

| Props    | Type      | Description |
|----------|----------|-------------|
| isOpen   | bool     | Définit si la modale est visible (`true`) ou cachée (`false`). |
| onClose  | func     | Fonction appelée lorsqu'on ferme la modale (ex: `() => setIsOpen(false)`). |
| title    | string   | Titre affiché en haut de la modale. |
| children | ReactNode | Contenu à afficher dans la modale. |

## 📌 Prérequis

Avant d'utiliser **samodal-react**, assure-toi d'avoir :

- **Node.js** : >= 18.0.0
- **React** : >= 19.0.0
- **ReactDOM** : >= 19.0.0

## 📌 Développement

Si tu veux modifier ou contribuer au projet, suis ces étapes :

### Cloner le repo GitHub :

```sh
git clone https://github.com/samiNedjai/samodal.git
```

### Installer les dépendances :

```sh
npm install
```

### Lancer le projet en mode développement :

```sh
npm run dev
```

### Créer une version et publier sur npm :

```sh
npm version patch
npm publish
```

## 📌 Liens utiles

- **npm** : [https://www.npmjs.com/package/samodal-react](https://www.npmjs.com/package/samodal-react)
- **GitHub** : [https://github.com/samiNedjai/samodal](https://github.com/samiNedjai/samodal)
- **Issues** : [Signaler un bug](https://github.com/samiNedjai/samodal/issues)

## 📌 Licence

Ce projet est sous licence **MIT**. 📜

Tu peux l'utiliser et le modifier librement ! 😊
