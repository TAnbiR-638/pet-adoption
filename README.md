# Pet Adoption App 🐾

A React Native mobile application that connects pet lovers with pets in need of homes. Users can browse available pets, share their own pets for adoption, and share rescue stories with the community.

## Features 📱

### 🔐 Authentication
- User registration and login
- Profile creation with profile pictures
- Secure authentication via Firebase Auth

### 🐕 Pet Adoption
- Browse available pets for adoption
- View detailed pet information including:
  - Pet type (dogs, cats, rabbits, birds)
  - Location/address
  - Contact information (WhatsApp)
  - Health documentation
- Take or upload photos of pets
- Post pets for adoption with complete details

### 📖 Story Sharing
- Share rescue stories with YouTube video links
- Browse community rescue stories
- View full stories with embedded videos

### 👤 Profile Management
- Personal profile with posts and stories
- View other users' profiles
- Profile customization with images

### 📷 Media Features
- Camera integration for taking photos
- Photo gallery access
- Image upload and storage
- Health document downloads

## Tech Stack 🛠️

- **Framework:** React Native with Expo
- **Backend:** Firebase (Firestore, Authentication, Storage)
- **Navigation:** React Navigation 6
- **UI Components:** React Native Elements (RNE UI)
- **Animations:** React Native Animatable
- **Camera:** Expo Camera
- **Media:** Expo Image Picker, Media Library
- **Video:** React Native YouTube iframe

## Prerequisites 📋

Before running this project, make sure you have:

- Node.js (v14 or higher)
- npm or yarn
- Expo CLI (`npm install -g expo-cli`)
- Android Studio (for Android development)
- Xcode (for iOS development, macOS only)
- Firebase project with Firestore and Authentication enabled

## Installation 🚀

1. **Clone the repository**
   ```bash
   git clone https://github.com/TAnbiR-638/pet-adoption.git
   cd pet-adoption
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure Firebase**
   
   Create a Firebase project and add your configuration to environment variables. Create a `.env` file in the root directory:
   
   ```env
   EXPO_PUBLIC_API_URL=your_firebase_api_key
   EXPO_PUBLIC_AUTH_DOMAIN=your_project_id.firebaseapp.com
   EXPO_PUBLIC_PROJECT_ID=your_project_id
   EXPO_PUBLIC_STORAGE_BUCKET=your_project_id.appspot.com
   EXPO_PUBLIC_MESSAGING_SENDER_ID=your_messaging_sender_id
   EXPO_PUBLIC_APP_ID=your_app_id
   ```

4. **Start the development server**
   ```bash
   npm start
   # or
   expo start
   ```

5. **Run on device/simulator**
   - For Android: `npm run android` or scan QR code with Expo Go app
   - For iOS: `npm run ios` or scan QR code with Expo Go app
   - For web: `npm run web`

## Project Structure 📁

```
pet-adoption/
├── App.js                 # Main app component with navigation
├── firebase.js            # Firebase configuration
├── package.json          # Dependencies and scripts
├── app.json              # Expo configuration
├── babel.config.js       # Babel configuration
├── assets/               # Static assets (images, fonts)
├── components/           # Reusable components
│   ├── FeedPost.js       # Pet post component
│   ├── Onboarding.js     # App onboarding
│   ├── TopImage.js       # Header image component
│   └── ...
└── screens/              # App screens
    ├── Landing.js        # Welcome screen
    ├── SignIn.js         # Login screen
    ├── SignUp.js         # Registration screen
    ├── Main.js           # Main app container
    ├── Feed.js           # Pet feed screen
    ├── Add.js            # Camera/photo selection
    ├── Save.js           # Pet posting form
    ├── AddStories.js     # Story creation
    ├── Stories.js        # Stories feed
    ├── Profile.js        # User profile
    └── ...
```

## Key Screens 📺

### Authentication Flow
- **Landing**: Welcome screen with onboarding
- **SignUp**: User registration with profile image
- **SignIn**: User login

### Main App Flow
- **Main**: Bottom tab navigation container
- **Feed**: Browse available pets
- **Add**: Camera interface for taking photos
- **Save**: Form to add pet details for adoption
- **Stories**: Browse and share rescue stories
- **Profile**: User profile and posts management

## Environment Variables 🔧

The app requires the following Firebase configuration variables:

| Variable | Description |
|----------|-------------|
| `EXPO_PUBLIC_API_URL` | Firebase API Key |
| `EXPO_PUBLIC_AUTH_DOMAIN` | Firebase Auth Domain |
| `EXPO_PUBLIC_PROJECT_ID` | Firebase Project ID |
| `EXPO_PUBLIC_STORAGE_BUCKET` | Firebase Storage Bucket |
| `EXPO_PUBLIC_MESSAGING_SENDER_ID` | Firebase Messaging Sender ID |
| `EXPO_PUBLIC_APP_ID` | Firebase App ID |

## Contributing 🤝

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Development Commands 💻

```bash
# Start development server
npm start

# Run on Android
npm run android

# Run on iOS
npm run ios

# Run on web
npm run web

# Clear Expo cache (if needed)
expo start -c
```

## Permissions 📱

The app requires the following permissions:
- Camera access (for taking pet photos)
- Photo library access (for selecting images)
- Media library access (for downloading health documents)

## Firebase Setup 🔥

1. Create a new Firebase project
2. Enable Authentication with Email/Password
3. Create a Firestore database with the following collections:
   - `users` - User profiles
   - `posts` - Pet adoption posts
   - `stories` - Rescue stories
   - `profilePosts` - User's personal posts
   - `images` - Uploaded images

## Support 💬

If you encounter any issues or have questions, please open an issue on GitHub.

## License 📄

This project is open source and available under the [MIT License](LICENSE).

---

Made with ❤️ for pets in need of loving homes 🐾