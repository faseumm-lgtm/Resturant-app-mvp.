# 🍽️ SAVOR — Fine Dining Restaurant App

A fully functional React Native + Expo restaurant mobile app with a premium red & black theme.

---

## 📁 Project Structure

```
RestaurantApp/
├── App.js
├── package.json
├── babel.config.js
├── constants/ac
│   └── theme.js              # Colors, fonts, sacpacing, shadows
├── context/
│   ├── AuthContext.js        # Global auth state
│   └── CartContext.js        # Global cart state
├── data/
│   └── menuData.js           # Static menu items, categories, today's special
├── navigation/
│   └── AppNavigator.js       # Stack navigator (auth vs app screens)
├── components/
│   ├── Header.js             # Reusable screen header
│   ├── PrimaryButton.js      # Button with variants (primary/outline/ghost)
│   ├── InputField.js         # Styled text input with label & error
│   ├── MenuItemCard.js       # Food item card with add-to-cart
│   └── CartBadge.js          # Cart icon with item count badge
└── screens/
    ├── LoginScreen.js
    ├── SignupScreen.js
    ├── HomeScreen.js
    ├── MenuScreen.js
    ├── TodaysSpecialScreen.js
    ├── CartScreen.js
    ├── ReservationScreen.js
    └── ProfileScreen.js
```

---

## 🚀 Installation & Running

### Prerequisites
- Node.js 18+ installed
- Expo Go app on your phone (latest version from App Store / Play Store)

### Steps

```bash
# 1. Navigate to the project folder
cd RestaurantApp

# 2. Install dependencies
npm install

# 3. Start the development server (use --tunnel if on different network)
npx expo start

# If Expo Go still won't connect, use tunnel mode:
npx expo start --tunnel
```

Then:
- **On your phone**: Scan the QR code with the Expo Go app
- **On Android emulator**: Press `a`
- **On iOS simulator**: Press `i`

### ⚠️ If it keeps loading — try these fixes in order:

1. **Make sure Expo Go is up to date** — update it in the App Store / Play Store
2. **Use tunnel mode**: `npx expo start --tunnel` (installs `@expo/ngrok` automatically)
3. **Same WiFi**: Your phone and computer must be on the same WiFi network
4. **Clear cache**: `npx expo start --clear`
5. **Delete node_modules and reinstall**:
   ```bash
   rm -rf node_modules
   npm install
   npx expo start --clear
   ```

---

## ✨ Features

| Screen | Features |
|--------|---------|
| **Login** | Email/password validation, navigation to Home |
| **Signup** | Full form validation, password confirmation |
| **Home** | Greeting, hero banner, quick-access nav grid |
| **Menu** | Category filter, search, FlatList of items, add/remove/quantity |
| **Today's Special** | Chef's pick with discount badge, add to cart |
| **Cart** | Item list, quantity control, dine-in/takeaway toggle, order summary, place order |
| **Reservation** | Date picker (7-day scroll), time slots, guest count, special requests |
| **Profile** | User info, stats, menu options, logout |

---

## 🎨 Design System

- **Primary**: `#C8102E` (Deep Red)
- **Background**: `#0D0D0D` (True Black)
- **Surface**: `#1E1E1E` (Card Dark)
- **Accent**: `#FFD700` (Gold)

---

## 🔐 Demo Login

Any valid email + password with 6+ characters will work.

Example:
- Email: `demo@savor.com`
- Password: `password123`
