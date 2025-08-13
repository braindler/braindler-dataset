# React Native Telecommunications Libraries

Welcome to our collection of React Native libraries focused on telecommunications and VoIP functionality. This repository contains a comprehensive set of tools for building modern communication applications.

## 📱 Featured Libraries

### [react-native-sip2](https://github.com/telefon-one/react-native-sip2)
Complete SIP (Session Initiation Protocol) implementation for React Native with support for:
- ✅ iOS and Android platforms
- ✅ Video and audio communication
- ✅ CallKit integration (iOS)
- ✅ Push notifications
- ✅ Background call handling
- ✅ SIP messaging (IM) - iOS
- ✅ Typing indicators - iOS

### [react-native-dialer-replacement](https://github.com/telefon-one/react-native-dialer-replacement)
Android dialer replacement solution based on react-native-tele:
- ✅ Android platform support
- ✅ Modern AndroidX compatibility
- ✅ Custom dialer interface
- ✅ Call management integration

### [react-native-tele](https://github.com/telefon-one/react-native-tele)
Core telephony functionality for React Native applications:
- ✅ Call management
- ✅ Phone state monitoring
- ✅ Contact integration
- ✅ Cross-platform support

### [react-native-foreground-background](https://github.com/telefon-one/react-native-foreground-background)
Background service management for React Native:
- ✅ Foreground service handling
- ✅ Background task management
- ✅ Service lifecycle control

### [react-native-sip2-builder](https://github.com/telefon-one/react-native-sip2-builder)
Build tools and utilities for SIP2 development:
- ✅ Build automation
- ✅ Development utilities
- ✅ Configuration management

### [react-native-replace-dialer](https://github.com/telefon-one/react-native-replace-dialer)
Alternative dialer replacement implementation:
- ✅ Custom dialer UI
- ✅ Call handling
- ✅ User experience optimization

## 🚀 Quick Start

### Installation

```bash
# Install SIP2 library
yarn add react-native-sip2

# For iOS (RN 0.60+)
cd ios && pod install

# For Android
# Ensure AndroidX is enabled in your project
```

### Basic Usage

```javascript
import { Endpoint } from 'react-native-sip2';

// Initialize SIP endpoint
const endpoint = new Endpoint();
const state = await endpoint.start();

// Create SIP account
const account = await endpoint.createAccount({
  name: "John Doe",
  username: "sip_username",
  domain: "pbx.example.com",
  password: "password"
});

// Make a call
const call = await endpoint.makeCall(account, "destination@domain.com");
```

## 🛠️ Development

### Prerequisites
- React Native 0.60+
- iOS: Xcode 12+
- Android: Android Studio with AndroidX support
- Node.js 14+

### Building from Source

```bash
# Clone the repository
git clone https://github.com/telefon-one/libsReactNative.git

# Install dependencies
yarn install

# Build individual libraries
cd react-native-sip2 && yarn build
```

## 📋 Roadmap

### react-native-sip2
- [ ] SIP Messages (IM) for Android
- [ ] Typing indicators for Android
- [ ] Enhanced video call features
- [ ] WebRTC integration

### react-native-dialer-replacement
- [ ] iOS support
- [ ] Advanced call screening
- [ ] Custom themes and UI
- [ ] Integration with native contacts

## 🤝 Contributing

We welcome contributions! Please see our contributing guidelines:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Setup

```bash
# Set up development environment
yarn install
yarn link

# Run tests
yarn test

# Build documentation
yarn docs
```

## 📄 License

This project is licensed under the NativeMindNON-C free for non-commercial use.

## 🆘 Support

- 📧 Email: thai@telefon-one.com
- 💬 Telegram: [Business](https://t.me/ur369)
- 💬 Telegram: [Technical](https://t.me/AntonDodonov)
