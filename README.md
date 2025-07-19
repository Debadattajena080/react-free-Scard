<<<<<<< HEAD
**A lightweight, customizable React scratch card component with random rewards support.**

## Use it to add gamified rewards, engagement boosters, or event-driven scratch cards to your React apps effortlessly.

## 🚀 Features

✅ Easy to integrate in any React app  
✅ Supports **random rewards** for gamified campaigns  
✅ Auto-scratch and manual scratch options  
✅ Lightweight and flexible customization  
✅ Local storage reward caching with expir

---

## 📦 Installation

npm install react-free-scratchcard

or

yarn add react-free-scratchcard

⚡ Quick Usage

import ScratchCard from "react-free-scratchcard";
import scratchImage from "./assets/scratch-surface.jpg";
import prizeImage from "./assets/prize.jpg";

<ScratchCard
      scratchImage={scratchImage}
      prizeImage={prizeImage}
    />

🎁 Random Rewards Example

import ScratchCard from "react-free-scratchcard";
import scratchImage from "./assets/scratch-surface.jpg";
import prize1 from "./assets/prize1.jpg";
import prize2 from "./assets/prize2.jpg";

const rewardOptions = [
{ image: prizeImage1, points: 899 },
{ image: prizeImage2, points: 999 },
];

const [selectedReward, setSelectedReward] = useState(null);

useEffect(() => {
const randomIndex = Math.floor(Math.random() \* rewardOptions.length);
setSelectedReward(rewardOptions[randomIndex]);
}, []);

const handleScratchComplete = (result) => {
console.log("Scratch completed!", result);
};

      <ScratchCard
        scratchImage={Fimage}
        prizeImage={selectedReward.image}
        scratchedPoints={selectedReward.points}
        onScratchComplete={handleScratchComplete}
      />

⚙️ Props Reference
| Prop                  | Type       | Default          | Description                          |
| --------------------- | ---------- | ---------------- | ------------------------------------ |
|  scratchImage         |  string    |   Required       | Scratch surface image                |

|  prizeImage           |  string    |      ---         | Image revealed after scratching      |

|  rewardOptions        |   array    |       []         | Array of rewards `{ image, points }` |

|  onRewardSelected     |   function |      ---         | Callback when a reward is selected   |

|  onScratchComplete    |   function |      ---         | Callback after scratch completes     |

|  scratchedPoints     |    number   |       0          | Points displayed/awarded             |

|  revealButtonText     | string     |  "Scratch Now"   | Text shown on the reveal button      |

|  revealingText        |  string    |  "Revealing..."  | Text shown during auto-scratch       |

|  scratchRadius        |  number    |       20         | Brush radius for scratching          |

|  autoScratchSpeed     |  number    |       1          | Speed of auto-scratch animation      |

|  rewardExpiryMinutes  |  number    |       5          | Minutes before local reward expiry   |

|  storeReward          |  boolean   |     true         | Enable/disable local reward caching  |


🛠️ Use Cases
✅ Gamified learning platforms
✅ E-commerce promotions
✅ Event rewards (festivals, quizzes)
✅ User engagement and retention activities



✨ Author
Debadatta Jena


# react-free-Scard
=======
# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
>>>>>>> b2193d2 (Initialize project using Create React App)
