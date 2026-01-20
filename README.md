# Kittens Boilerplate

A React Native boilerplate with pre-installed and pre-configured libraries to reduce project setup time.

## Requirements

- Node.js >= 20
- React Native CLI
- Xcode (for iOS)
- Android Studio (for Android)

## Installation

```bash
# Clone the repository
git clone https://github.com/javbk201/RN-Kittens-Template.git
cd kittens_boilerplate

# Install dependencies
npm install
# or with bun
bun install

# Install pods (iOS)
cd ios && pod install && cd ..
```

## Available Scripts

```bash
npm run android    # Run on Android
npm run ios        # Run on iOS
npm run start      # Start Metro bundler
npm run lint       # Run ESLint
npm run test       # Run tests with Jest
```

## Included Libraries

### UI Framework
| Library | Version | Description |
|---------|---------|-------------|
| [@ui-kitten/components](https://akveo.github.io/react-native-ui-kitten/) | ^5.3.1 | UI framework based on Eva Design System |
| [@ui-kitten/eva-icons](https://akveo.github.io/eva-icons/) | ^5.3.1 | Eva icons pack |
| [@eva-design/eva](https://eva.design/) | ^2.2.0 | Eva Design System |

### Navigation
| Library | Version | Description |
|---------|---------|-------------|
| [@react-navigation/native](https://reactnavigation.org/) | ^7.1.26 | React Navigation core |
| [@react-navigation/native-stack](https://reactnavigation.org/) | ^7.9.0 | Native stack navigator |
| [@react-navigation/elements](https://reactnavigation.org/) | ^2.9.3 | UI elements for navigation |

### Utilities
| Library | Version | Description |
|---------|---------|-------------|
| [@shopify/flash-list](https://shopify.github.io/flash-list/) | ^2.2.0 | High-performance list component |
| [axios](https://axios-http.com/) | ^1.13.2 | HTTP client |
| [react-native-nitro-modules](https://github.com/margelo/react-native-nitro-modules) | ^0.33.2 | Native modules framework |
| [react-native-reanimated](https://docs.swmansion.com/react-native-reanimated/) | ^4.2.1 | High-performance animations |
| [react-native-screens](https://github.com/software-mansion/react-native-screens) | ^4.19.0 | Optimized native navigation |
| [react-native-safe-area-context](https://github.com/th3rdwave/react-native-safe-area-context) | ^5.6.2 | Safe area handling |
| [react-native-splash-view](https://github.com/nicksenger/react-native-splash-view) | ^0.0.19 | Native splash screen |
| [react-native-svg](https://github.com/software-mansion/react-native-svg) | ^15.15.1 | SVG support |
| [react-native-worklets](https://github.com/margelo/react-native-worklets) | ^0.7.1 | Worklets for background tasks |

### Development
| Library | Version | Description |
|---------|---------|-------------|
| TypeScript | ^5.8.3 | Static typing |
| ESLint | ^8.19.0 | JavaScript/TypeScript linter |
| Prettier | 2.8.8 | Code formatter |
| Jest | ^29.6.3 | Testing framework |
| babel-plugin-module-resolver | ^5.0.2 | Path aliases |

## Path Alias Configuration

The project includes path alias configuration for cleaner imports:

```typescript
// Instead of:
import { Component } from '../../../components/Component';

// You can use:
import { Component } from '@/components/Component';
```

The `@` alias points to the `./src` folder.

## Tech Stack

- **React**: 19.2.0
- **React Native**: 0.83.1
- **TypeScript**: 5.8.3

## Project Structure

```
kittens_boilerplate/
├── android/          # Native Android project
├── ios/              # Native iOS project
├── src/              # Source code (create as needed)
├── __tests__/        # Tests
├── App.tsx           # Main component
├── index.js          # Entry point
└── ...
```

## License

MIT
