# CipherShare - Secure Your Messages in a Snap

CipherShare is a React Native app that allows users to convert normal messages into numbers to securely share with friends without anyone else understanding the content. The app uses Firebase Authentication to manage user accounts and ensure secure access.

## Features

- **Message Encryption:** Convert text messages into number sequences.
- **User Authentication:** Secure login and registration with Firebase Authentication.
- **Shareable Messages:** Share the encrypted messages with friends.
- **Decryption:** Users can decrypt messages received from friends.

## Getting Started

### Prerequisites

Make sure you have completed the [React Native - Environment Setup](https://reactnative.dev/docs/environment-setup) instructions before proceeding. You'll also need a Firebase project set up.

### Step 1: Clone the Repository

```bash
git clone https://github.com/yourusername/ciphershare.git
cd ciphershare
```

### Step 2: Install Dependencies

```bash
# using npm
npm install

# OR using Yarn
yarn install
```

### Step 3: Firebase Setup

1. Go to the [Firebase Console](https://console.firebase.google.com/).
2. Create a new project or use an existing one.
3. Enable Firebase Authentication with Email/Password.
4. Add Android/iOS apps to your Firebase project and download the \`google-services.json\` (for Android) or \`GoogleService-Info.plist\` (for iOS) and place them in the respective directories:
   - **Android:** \`android/app/google-services.json\`
   - **iOS:** \`ios/CipherShare/GoogleService-Info.plist\`
5. Update your Firebase configuration in \`App.tsx\`:

```javascript
import { initializeApp } from 'firebase/app';

const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_AUTH_DOMAIN",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_STORAGE_BUCKET",
  messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
  appId: "YOUR_APP_ID"
};

initializeApp(firebaseConfig);
```

### Step 4: Start the Metro Server

```bash
# using npm
npm start

# OR using Yarn
yarn start
```

### Step 5: Start Your Application

Open a new terminal from the root of your React Native project and run the following command to start your Android or iOS app:

#### For Android

```bash
# using npm
npm run android

# OR using Yarn
yarn android
```

#### For iOS

```bash
# using npm
npm run ios

# OR using Yarn
yarn ios
```

### Step 6: Modify and Test

1. Open \`App.tsx\` in your text editor.
2. Modify the code to customize the encryption algorithm or UI.
3. For **Android**: Press the <kbd>R</kbd> key twice or select **"Reload"** from the **Developer Menu** (<kbd>Ctrl</kbd> + <kbd>M</kbd> on Windows/Linux) to see your changes.

   For **iOS**: Hit <kbd>Cmd ⌘</kbd> + <kbd>R</kbd> in your iOS Simulator to reload the app and see your changes!

## Congratulations! 🎉

You've successfully set up and run the CipherShare app. 🎉

### Next Steps

- Add more encryption methods for increased security.
- Integrate with cloud storage to save encrypted messages.
- Implement a friends list to easily share encrypted messages within the app.

## Troubleshooting

If you run into any issues, check the [React Native Troubleshooting](https://reactnative.dev/docs/troubleshooting) page or the [Firebase Documentation](https://firebase.google.com/docs).

## Learn More

To learn more about the technologies used in this project, take a look at the following resources:

- [React Native](https://reactnative.dev) - Learn more about React Native.
- [Firebase](https://firebase.google.com/docs) - Firebase documentation for authentication and other services.
- [React Navigation](https://reactnavigation.org) - Routing and navigation for React Native apps.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
