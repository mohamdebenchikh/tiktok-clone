# TikTok Clone - Creator Dashboard

A modern, responsive TikTok Creator Dashboard built with React, TypeScript, and Vite. This application provides creators with comprehensive tools to manage their content, track earnings, analyze performance, and handle financial transactions.

## 🚀 Features

### 📊 Dashboard & Analytics
- **Main Dashboard**: Overview of creator statistics and quick access to key features
- **Rewards Analytics**: Detailed performance metrics and earnings analysis
- **Transaction History**: Complete record of all financial transactions
- **Balance Management**: Real-time balance tracking and financial overview

### 💰 Monetization & Earnings
- **Income Plus**: Enhanced earning opportunities and premium features
- **Income Verification**: Secure identity and income verification process
- **Withdraw Money**: Easy withdrawal system with multiple payment options
- **Balance Details**: Comprehensive breakdown of earnings and balances

### 🎥 Content Management
- **TikTok Studio**: Content creation and management tools
- **Profile Management**: User profile customization and settings

### 🔧 Core Features
- **Responsive Design**: Optimized for desktop and mobile devices
- **Real-time Updates**: Live data synchronization
- **Secure Transactions**: Protected financial operations
- **Multi-language Support**: Internationalization ready
- **Dark/Light Theme**: User preference-based theming

## 🛠️ Tech Stack

### Frontend
- **React 19.1.0** - Modern React with latest features
- **TypeScript 5.8.3** - Type-safe development
- **Vite 7.0.0** - Fast build tool and development server
- **React Router 7.6.3** - Client-side routing
- **Redux Toolkit 2.8.2** - State management
- **React Hot Toast 2.5.2** - Toast notifications

### Development Tools
- **ESLint 9.29.0** - Code linting and quality
- **TypeScript ESLint 8.34.1** - TypeScript-specific linting
- **Sass Embedded 1.89.2** - CSS preprocessing (converted to CSS)

### Build & Deployment
- **Vite** - Build optimization and bundling
- **TypeScript Compiler** - Type checking and compilation

## 📁 Project Structure

```
src/
├── components/          # Reusable UI components
│   ├── BalanceCard.tsx     # Balance display component
│   ├── Dashboard.tsx       # Main dashboard component
│   ├── Header.tsx          # Navigation header
│   ├── Loading.tsx         # Loading indicator
│   ├── LoadingOverlay.tsx  # Full-screen loading overlay
│   ├── MonetizationSection.tsx  # Monetization features
│   ├── RechargePackage.tsx # Package purchase component
│   └── ServicesSection.tsx # Services overview
├── pages/               # Application pages
│   ├── BalanceDetailsPage.tsx    # Detailed balance view
│   ├── BalancePage.tsx           # Balance overview
│   ├── IncomePlusPage.tsx        # Premium earning features
│   ├── IncomeVerificationPage.tsx # Identity verification
│   ├── ProfilePage.tsx           # User profile management
│   ├── RewardsAnalyticsPage.tsx  # Analytics dashboard
│   ├── TikTokStudioPage.tsx      # Content management
│   ├── TransactionDetailsPage.tsx # Transaction details
│   ├── TransactionHistoryPage.tsx # Transaction history
│   ├── WithdrawMoneyPage.tsx     # Withdrawal interface
│   └── WithdrawResultPage.tsx    # Withdrawal confirmation
├── store/               # Redux state management
│   ├── slices/             # Redux slices
│   ├── hooks.ts            # Typed Redux hooks
│   └── index.ts            # Store configuration
├── css/                 # Styling (converted from SCSS to CSS)
│   ├── styles/             # Component-specific styles
│   ├── app.css             # Global application styles
│   ├── index.css           # Base styles
│   └── main.css            # Main stylesheet
├── assets/              # Static assets
│   ├── fonts/              # Custom fonts
│   ├── images/             # Image assets
│   └── icons/              # Icon assets
├── hooks/               # Custom React hooks
├── utils/               # Utility functions
└── App.tsx              # Main application component
```

## 🚦 Getting Started

### Prerequisites
- **Node.js** (version 18 or higher)
- **npm** or **yarn** package manager
- **Git** for version control

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd tiktok-clone
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   # or
   yarn dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:5173` to view the application

### Available Scripts

- **`npm run dev`** - Start development server with hot reload
- **`npm run build`** - Build the application for production
- **`npm run preview`** - Preview the production build locally
- **`npm run lint`** - Run ESLint for code quality checks

## 🎨 Styling Architecture

The project uses a modular CSS architecture with the following principles:

### CSS Organization
- **Global Styles**: Base styles and CSS variables in `app.css`
- **Component Styles**: Scoped styles for each component in `css/styles/`
- **Responsive Design**: Mobile-first approach with breakpoints at 768px and 480px
- **CSS Variables**: Consistent color scheme and spacing using CSS custom properties

### Design System
```css
/* Color Palette */
--primary-color: #00d4ff;
--secondary-color: #f5f5f5;
--text-color: #333;
--success-color: #10b981;
--error-color: #ef4444;
--warning-color: #6366f1;

/* Typography */
- ProximanovaRegular (Primary font)
- ProximanovaBold (Headings and emphasis)
- ProximanovaLight (Light text)
- CoreSans (Special elements)
```

### Responsive Breakpoints
- **Mobile**: < 480px
- **Tablet**: 480px - 768px
- **Desktop**: > 768px

## 🔄 State Management

The application uses Redux Toolkit for state management with the following structure:

### Store Configuration
- **Centralized State**: Single source of truth for application state
- **Typed Hooks**: Custom hooks for type-safe Redux usage
- **Slice-based Architecture**: Modular state management with Redux slices

### Key State Features
- User authentication and profile data
- Transaction history and balance information
- UI state (loading, notifications, theme)
- Analytics and performance metrics

## 🛣️ Routing

The application uses React Router for navigation with the following routes:

| Route | Component | Description |
|-------|-----------|-------------|
| `/` | ProfilePage | Home/Profile page |
| `/dashboard` | Dashboard | Main dashboard |
| `/balance` | BalancePage | Balance overview |
| `/balance-details` | BalanceDetailsPage | Detailed balance view |
| `/transaction-history` | TransactionHistoryPage | Transaction list |
| `/transaction-details/:id` | TransactionDetailsPage | Transaction details |
| `/withdraw-money` | WithdrawMoneyPage | Withdrawal interface |
| `/withdraw-result` | WithdrawResultPage | Withdrawal confirmation |
| `/income-plus` | IncomePlusPage | Premium features |
| `/income-verification` | IncomeVerificationPage | Identity verification |
| `/tiktok-studio` | TikTokStudioPage | Content management |
| `/rewards-analytics` | RewardsAnalyticsPage | Analytics dashboard |

## 🔧 Development Guidelines

### Code Style
- **TypeScript**: Strict type checking enabled
- **ESLint**: Enforced code quality and consistency
- **Component Structure**: Functional components with hooks
- **File Naming**: PascalCase for components, camelCase for utilities

### Best Practices
- **Type Safety**: Avoid `any` types, use proper TypeScript interfaces
- **Component Design**: Single responsibility principle
- **State Management**: Use Redux for global state, local state for component-specific data
- **Error Handling**: Comprehensive error boundaries and user feedback
- **Performance**: Lazy loading and code splitting where appropriate

### Testing Strategy
- **Unit Tests**: Component and utility function testing
- **Integration Tests**: Page-level functionality testing
- **E2E Tests**: Critical user journey testing
- **Accessibility**: WCAG compliance testing

## 📱 Mobile Optimization

### Responsive Features
- **Touch-friendly Interface**: Optimized button sizes and touch targets
- **Mobile Navigation**: Simplified navigation for mobile devices
- **Performance**: Optimized images and lazy loading
- **PWA Ready**: Service worker and manifest configuration

### Mobile-specific Enhancements
- **Gesture Support**: Swipe navigation and touch interactions
- **Viewport Optimization**: Proper viewport meta tags
- **Font Scaling**: Responsive typography
- **Image Optimization**: WebP format support and responsive images

## 🔐 Security Features

### Data Protection
- **Input Validation**: Client-side and server-side validation
- **XSS Prevention**: Sanitized user inputs
- **CSRF Protection**: Token-based request validation
- **Secure Storage**: Encrypted local storage for sensitive data

### Authentication & Authorization
- **JWT Tokens**: Secure authentication mechanism
- **Role-based Access**: Different permission levels
- **Session Management**: Automatic logout and session refresh
- **Two-factor Authentication**: Enhanced security options

## 🚀 Deployment

### Build Process
```bash
# Production build
npm run build

# Preview production build
npm run preview
```

### Deployment Options
- **Vercel**: Recommended for React applications
- **Netlify**: Static site hosting with CI/CD
- **AWS S3 + CloudFront**: Scalable cloud deployment
- **Docker**: Containerized deployment

### Environment Configuration
```bash
# Environment variables
VITE_API_URL=your_api_url
VITE_APP_NAME=TikTok Clone
VITE_VERSION=1.0.0
```

## 🤝 Contributing

### Development Workflow
1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

### Code Review Process
- All changes require code review
- Automated tests must pass
- ESLint checks must pass
- TypeScript compilation must succeed

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **React Team** - For the amazing React framework
- **Vite Team** - For the fast build tool
- **TypeScript Team** - For type safety
- **Redux Team** - For state management
- **Community Contributors** - For open source packages

## 📞 Support

For support and questions:
- **Issues**: Create an issue on GitHub
- **Documentation**: Check the project wiki
- **Community**: Join our Discord server

---

**Built with ❤️ using React, TypeScript, and Vite**
