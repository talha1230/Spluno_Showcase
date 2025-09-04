<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./public/spluno_white_logo.png">
    <img src="./public/spluno_blac_logo.png" height="120" alt="Spluno Logo">
  </picture>
  
  <h1>🎉 SPLUNO - Nightlife Cost-Sharing Platform</h1>
  
  <p><strong>Revolutionizing Kuala Lumpur's Party Scene</strong></p>
  
  <p>Connect • Split • Party • Repeat</p>
  
  [![Demo](https://img.shields.io/badge/Demo-Live-brightgreen?style=for-the-badge)](https://spluno.vercel.app/)
  [![Next.js](https://img.shields.io/badge/Next.js-15.3.4-black?style=for-the-badge&logo=next.js)](https://nextjs.org/)
  [![TypeScript](https://img.shields.io/badge/TypeScript-5.8.3-blue?style=for-the-badge&logo=typescript)](https://www.typescriptlang.org/)
  [![React](https://img.shields.io/badge/React-19.1.0-61DAFB?style=for-the-badge&logo=react)](https://reactjs.org/)
  
  <img alt="Spluno Platform Preview" src="./public/og.png" width="100%">
</div>

---

## 🚀 About Spluno

**Spluno** is a production-ready nightlife cost-sharing platform that transforms how people experience Kuala Lumpur's vibrant party scene. Our innovative platform connects like-minded party-goers, enables seamless table creation and joining, and provides intelligent cost-splitting solutions for unforgettable nights out.

### 🎯 Problem We Solve
- **High nightlife costs** - Split table expenses fairly among participants
- **Solo party-goers** - Connect with compatible groups for shared experiences  
- **Table coordination** - Streamline communication between hosts and joiners
- **Payment transparency** - Clear, automated cost calculations and tracking

---

## ✨ Key Features

### 🏗️ **Core Platform Features**
- **🎪 Table Creation & Management** - Create, customize, and manage party tables for any KL venue
- **👥 Advanced User Search** - Find compatible party-goers with fuzzy matching and smart filters
- **💰 Intelligent Cost Splitting** - Automatic calculation and fair distribution of table expenses
- **📱 QR Code Integration** - Instant table joining via QR code scanning
- **🔄 Real-time Join Requests** - Bidirectional messaging system between hosts and potential joiners

### 💬 **Communication & Social**
- **⚡ Real-time Chat System** - Powered by Stream Chat with DM and group messaging
- **📢 Smart Notifications** - Real-time updates for requests, approvals, and table activities
- **👤 Rich User Profiles** - Comprehensive profiles with ratings, badges, and social features
- **🔍 Social Discovery** - Find users by username, interests, and party preferences

### 🛡️ **Security & Quality**
- **🔐 Enterprise Authentication** - Clerk-powered secure user management with social login
- **⭐ User Rating System** - Community-driven ratings for safety and reliability
- **📋 Content Moderation** - Reporting system for maintaining platform quality
- **🔒 Privacy Controls** - Granular privacy settings and user preferences

### 📱 **User Experience**
- **🎨 Modern UI/UX** - Clean, intuitive interface with dark/light mode support
- **📱 Mobile-First Design** - Optimized for iOS and Android with responsive layouts
- **🎭 3D Animations** - Immersive table visualizations with React Three Fiber
- **⚡ Real-time Updates** - Live synchronization across all user interfaces

---

## 🛠️ Technology Stack

### **Frontend Architecture**
```
Next.js 15.3.4 (App Router) + React 19 + TypeScript 5.8.3
├── UI Framework: Tailwind CSS + Radix UI Components
├── State Management: TanStack Query + React Hooks
├── 3D Graphics: React Three Fiber + Drei + PostProcessing
├── Animations: GSAP + Tailwind Animate
└── Theme System: Next-themes with custom design tokens
```

### **Backend & Infrastructure**
```
Authentication: Clerk (Social Login + User Management)
├── Database: Appwrite (8 Collections + Real-time Subscriptions)
├── Real-time Chat: Stream Chat SDK + Custom Hooks
├── File Storage: Appwrite Storage (Avatars + Media)
├── API Layer: Next.js API Routes + Zod Validation
└── Deployment: Vercel (Edge Functions + Analytics)
```

### **Database Schema (8 Collections)**
```
users → tables → participants → join_requests
   ↓        ↓         ↓            ↓
ratings  reports  notifications  user_settings
```

### **Key Dependencies**
- **🔧 Core**: `next@15.3.4`, `react@19.1.0`, `typescript@5.8.3`
- **🎨 UI**: `@radix-ui/*`, `tailwindcss@3.4.17`, `lucide-react@0.525.0`
- **🔐 Auth**: `@clerk/nextjs@6.22.0`
- **💾 Database**: `appwrite@18.1.1`, `node-appwrite@17.0.0`
- **💬 Chat**: `stream-chat@9.11.0`, `stream-chat-react@13.2.3`
- **📊 State**: `@tanstack/react-query@5.83.0`
- **🎮 3D**: `@react-three/fiber@9.3.0`, `three@0.178.0`

---

## 📸 Screenshots

> Screenshots will be added to `assets/screenshots/` to showcase the platform's features and user interface.

- 🏠 **Homepage & Landing** - Modern landing page with feature highlights
- 📊 **User Dashboard** - Comprehensive activity overview and quick actions
- 🎪 **Table Creation** - Intuitive table setup with venue selection and cost management
- 🔍 **Search Interface** - Advanced user search with filters and smart matching
- 💬 **Chat System** - Real-time messaging with file sharing and reactions
- 👤 **User Profiles** - Rich profile pages with stats, activity, and social features
- 📱 **QR Integration** - Seamless table joining via QR code scanning
- 🔔 **Notifications** - Real-time notification center with action routing

---

## 🏗️ Architecture Overview

### **Application Structure**
```
app/
├── api/                    # API routes with standardized error handling
│   ├── auth/              # Authentication endpoints
│   ├── tables/            # Table CRUD operations
│   ├── chat/              # Chat token generation and management
│   ├── search/            # User search and suggestions
│   ├── qr/                # QR code generation and scanning
│   └── notifications/     # Real-time notification system
├── dashboard/             # User dashboard and management
├── tables/[id]/           # Table-specific pages with real-time updates
├── chat/                  # Chat interfaces (mobile/desktop optimized)
├── user/[@username]/      # Profile pages with username routing
├── search/                # Advanced user search interface
└── requests/              # Join request management system

components/
├── ui/                    # Radix UI base components
├── chat/                  # Chat UI with real-time features
├── tables/                # Table-specific components
├── notifications/         # Notification system components
└── [feature]/             # Feature-specific component groups

lib/
├── server-side-appwrite.ts    # Server-side database operations
├── stream-chat.ts            # Chat utilities and constants
├── hooks/                    # Custom React hooks
├── services/                 # Business logic services
└── validation/               # Input validation schemas
```

### **Key Design Patterns**
- **🔄 API Route Structure**: 5-step standardized pattern (Auth → Validation → Authorization → Logic → Response)
- **⚡ Real-time Features**: WebSocket connections with optimistic updates and rollback
- **🔒 Security First**: Server-side validation, parameterized queries, and permission checking
- **📱 Mobile-First**: Responsive design with progressive enhancement for desktop
- **🧩 Component Architecture**: Modular, reusable components with consistent design patterns

---

## 🚀 Getting Started

### **Prerequisites**
- Node.js 18+ and npm
- Appwrite instance (cloud or self-hosted)
- Clerk account for authentication
- Stream Chat account for real-time messaging

### **Quick Setup**

1. **Clone and Install**
   ```bash
   git clone https://github.com/talha1230/spluno.git
   cd spluno
   npm install
   ```

2. **Environment Configuration**
   ```bash
   cp .env.example .env.local
   # Configure your API keys (see .env.example for required variables)
   ```

3. **Database Setup**
   ```bash
   npm run db:setup          # Initialize Appwrite collections
   npm run db:create-qr      # Set up QR code system
   npm run test:infra        # Verify infrastructure connectivity
   ```

4. **Development Server**
   ```bash
   npm run dev               # Start development server (http://localhost:3001)
   npm run dev:https         # Start with HTTPS for mobile testing
   ```

### **Available Scripts**
```bash
# Development
npm run dev              # Start with Turbopack for fast development
npm run build           # Production build with optimization
npm run start           # Start production server

# Database Operations  
npm run db:setup        # Initialize database collections
npm run db:cleanup      # Clean orphaned records
npm run validate:qr     # Validate QR system functionality

# Testing & Validation
npm run test:infra      # Test database connectivity
npm run test:health     # Health check for all systems
npm run lint            # ESLint code quality check
npm run type-check      # TypeScript compilation check
```

---

## 🌟 Production Features

### **Performance Optimizations**
- **⚡ Turbopack Integration** - Ultra-fast development builds
- **🎯 Edge Functions** - Optimized API responses with Vercel Edge Runtime
- **📦 Code Splitting** - Automatic route-based code splitting
- **🖼️ Image Optimization** - Next.js Image component with Sharp
- **💾 Smart Caching** - TanStack Query with persistent cache

### **Security Measures**
- **🔐 Authentication**: Multi-provider social login with Clerk
- **🛡️ Authorization**: Role-based access control with permission checking
- **🔒 Input Validation**: Server-side validation with Zod schemas
- **🚫 Rate Limiting**: API rate limiting and abuse prevention
- **📋 Content Moderation**: User reporting and automated content filtering

### **Monitoring & Analytics**
- **📊 Error Tracking**: Comprehensive error boundaries and logging
- **⚡ Performance Metrics**: Real-time performance monitoring
- **👥 User Analytics**: Usage patterns and feature adoption tracking
- **🔍 Debug Tools**: Structured logging with emoji-coded messages

---

## 🎯 Key Business Features

### **For Party-goers**
- **🔍 Discover Tables** - Find tables matching your vibe, budget, and location preferences
- **💬 Connect Safely** - Chat with hosts before committing to join
- **💰 Transparent Costs** - See exact cost breakdowns before joining
- **⭐ Build Reputation** - Earn ratings and badges for reliable participation

### **For Table Hosts**
- **🎪 Easy Setup** - Create tables in minutes with venue and cost details
- **👥 Smart Matching** - Get matched with compatible party-goers
- **📱 QR Integration** - Share tables instantly via QR codes
- **💵 Fair Splitting** - Automatic cost calculation and payment tracking

### **For Venues**
- **📈 Increased Bookings** - Higher table occupancy through our platform
- **👥 Group Facilitation** - Help solo customers find compatible groups
- **💰 Revenue Optimization** - Maximize table revenue through cost-sharing
- **📊 Analytics Dashboard** - Understand customer patterns and preferences

---

## 📚 Documentation

### **📋 Project Documentation**
- **[📊 Employer Showcase](./EMPLOYER_SHOWCASE.md)** - Executive summary for professional evaluation
- **[🎯 Features Overview](./FEATURES.md)** - Comprehensive feature breakdown and roadmap
- **[🛠️ Technology Stack](./TECH_STACK.md)** - Detailed technical architecture and tools
- **[🏗️ Project Overview](./PROJECT_OVERVIEW.md)** - Development philosophy and structure

### **API Documentation**
```
📁 /api/tables          # Table CRUD operations
├── POST /create        # Create new table
├── GET /[id]          # Get table details
├── PUT /[id]          # Update table
└── DELETE /[id]       # Delete table

📁 /api/search          # Search functionality  
├── GET /users         # Search users with filters
└── GET /suggestions   # Get search suggestions

📁 /api/chat           # Chat system
├── POST /token        # Generate chat tokens
└── GET /channels      # List user channels

📁 /api/qr             # QR Code system
├── POST /generate     # Generate table QR codes
├── POST /scan         # Process QR code scans
└── GET /user          # User QR settings
```

### **Component Documentation**
- **UserSearchCard**: Flexible user display component with 3 size variants
- **TableCard**: Comprehensive table information display
- **ChatInterface**: Real-time messaging with file sharing
- **NotificationCenter**: Real-time notification management
- **QRScanner**: Mobile camera integration for table joining
- **3DTableVisualization**: Interactive table representation

---

## 🚀 Deployment

### **Vercel Deployment**
```bash
# Automatic deployment via GitHub integration
git push origin main

# Manual deployment
npm run build
vercel --prod
```

### **Environment Variables**
```bash
# Required for production
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_key
CLERK_SECRET_KEY=your_clerk_secret
NEXT_PUBLIC_APPWRITE_PROJECT_ID=your_appwrite_project
STREAM_API_KEY=your_stream_key
```

### **Health Checks**
- **🔍 Database**: `/api/health` - Test all database connections
- **💬 Chat**: Verify Stream Chat token generation
- **🔐 Auth**: Validate Clerk authentication flow
- **📱 QR System**: Test QR code generation and scanning

---

## 👥 Contributing

We welcome contributions! Here's how you can help:

### **Development Workflow**
1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

### **Code Standards**
- **TypeScript**: Strict mode with comprehensive type safety
- **ESLint**: Follow existing code style and patterns
- **Testing**: Add tests for new features
- **Documentation**: Update docs for API changes

### **Areas for Contribution**
- 🎨 UI/UX improvements and new themes
- 🔧 Performance optimizations
- 🧪 Test coverage expansion
- 📚 Documentation enhancements
- 🌐 Internationalization support

---

## 📊 Project Stats

- **🏗️ Lines of Code**: 50,000+ (TypeScript, JSX, CSS)
- **📦 Components**: 100+ reusable React components
- **🛣️ API Routes**: 40+ endpoints with full CRUD operations
- **💾 Database**: 8 collections with complex relationships
- **🧪 Test Coverage**: Comprehensive infrastructure testing
- **📱 Mobile Support**: Full responsive design with PWA features

---

## 🎉 Live Demo

**🌐 [Experience Spluno Live](https://spluno.vercel.app/)**

Try our platform with test accounts:
- **Host**: `wannago4coffe@gmail.com` (Create and manage tables)
- **Joiner**: `talha935523@gmail.com` (Search and join tables)

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🤝 Connect & Support

- **💼 LinkedIn**: [Connect with the team](https://linkedin.com/in/talha-khan)
- **🐦 Twitter**: [@spluno_kl](https://twitter.com/spluno_kl)
- **📧 Email**: [hello@spluno.com](mailto:hello@spluno.com)
- **💬 Discord**: [Join our community](https://discord.gg/spluno)

---

<div align="center">
  <p><strong>🎉 Ready to revolutionize your nightlife experience?</strong></p>
  <p>Join Spluno and discover the future of party planning in KL!</p>
  
  [![Get Started](https://img.shields.io/badge/Get%20Started-Join%20Now-purple?style=for-the-badge&logo=rocket)](https://spluno.vercel.app/)
  [![Star on GitHub](https://img.shields.io/badge/Star%20on-GitHub-yellow?style=for-the-badge&logo=github)](https://github.com/talha1230/spluno)
</div>

---

## 🚀 Development Progress Summary

### Phase 3 Completion: Advanced User Search & Profile System (July 2025)

#### **Major Features Implemented:**

1. **Comprehensive User Search System**
   - ✅ Real-time search with fuzzy matching and relevance scoring
   - ✅ Advanced filtering (verified users, online status, rating ranges, location)
   - ✅ Multiple sorting options (relevance, rating, activity, newest)
   - ✅ Search suggestions and autocomplete functionality
   - ✅ Grid/List view toggle with responsive design

2. **User Profile & Username System**
   - ✅ Complete username migration (9/9 test users successfully migrated)
   - ✅ Unique username validation and availability checking
   - ✅ Username suggestion system with intelligent recommendations
   - ✅ Profile routes accessible via `/user/@username` URLs
   - ✅ Date of Birth integration with age calculation
   - ✅ Profile image management and avatar system

3. **Advanced UI Components**
   - ✅ Flexible user card component with 3 size variants (compact, standard, expanded)
   - ✅ Horizontal and vertical layout orientations
   - ✅ Three-tier information hierarchy (essential, secondary, contextual)
   - ✅ Loading skeletons matching all card layouts
   - ✅ Empty state with search suggestions and popular searches
   - ✅ Error state with retry functionality

4. **Technical Infrastructure**
   - ✅ Next.js 15 compatibility with async params syntax
   - ✅ TypeScript strict mode compliance
   - ✅ Production build optimization
   - ✅ Database schema enhancements with username fields
   - ✅ API route improvements and error handling

#### **Architecture Highlights:**

- **Search Service**: Advanced user-search-service with fuzzy matching, relevance scoring, and caching
- **Component System**: Modular, reusable components with consistent design patterns
- **Database Integration**: Seamless Appwrite integration with proper type safety
- **Performance**: Optimized with skeleton loading, pagination, and efficient queries
- **User Experience**: Intuitive navigation, responsive design, and comprehensive state management

#### **Files Added/Modified:**

**New Components:**
- `app/search/page.tsx` - Main search results page
- `components/user-search-card.tsx` - Flexible user display component
- `components/user-search-skeleton.tsx` - Loading states
- `components/empty-search-results.tsx` - Empty search state
- `components/error-search-results.tsx` - Error handling
- `components/username-input.tsx` - Username input with validation

**Enhanced Services:**
- `lib/user-search-service.ts` - Advanced search functionality
- `lib/username-service.ts` - Username management
- `lib/user-service.ts` - User profile operations
- Database migration scripts for username implementation

**API Endpoints:**
- `/api/search/users` - User search with filtering
- `/api/search/suggestions` - Search suggestions
- `/api/username/*` - Username validation and management
- `/api/user/[username]` - Profile data by username

#### **Current Status:**
- ✅ Search functionality fully operational and visible
- ✅ User profiles accessible via @username URLs
- ✅ **Enhanced user profile pages with comprehensive UX**
- ✅ Advanced search interface with comprehensive features
- ✅ Production build ready and TypeScript compliant
- ✅ All loading, empty, and error states implemented
- ✅ Database migration complete with 9 test users

#### **Latest Enhancement: User Profile Page UX Overhaul (July 2025)**

**Implemented Features:**
- ✅ **Enhanced Profile Header**: Larger avatars, status indicators, online presence
- ✅ **Comprehensive Stats Dashboard**: 6-metric overview with visual indicators
- ✅ **Tabbed Activity Interface**: Active Tables, Past Tables, Reviews, Achievements
- ✅ **Rich Table Cards**: Visual grid layout with detailed information
- ✅ **Timeline for Past Activities**: Historical view with status indicators
- ✅ **Professional Action Buttons**: Connect, Message, Call, Email options
- ✅ **Responsive Design**: Mobile-first with desktop enhancements
- ✅ **Empty States**: Friendly placeholders for sections without data
- ✅ **Visual Polish**: Shadows, gradients, hover effects, and micro-interactions

**UX Improvements:**
- Three-tier information hierarchy (Identity, Details, Activity)
- Color-coded status indicators and progress bars
- Interactive hover effects and smooth transitions
- Professional gradient avatars with fallbacks
- Comprehensive user stats with icons and descriptions
- Clear call-to-action buttons with proper emphasis

#### **Database Status (July 2025):**
```
✅ Found 9 users with complete username migration:
1. TALHA KHAN (@talha_khan) - talha935523@gmail.com
2. Joshua (@joshua) - joshuajones101010@gmail.com
3. Sunny Khan (@sunny_khan) - userstillunknown@gmail.com
4. SHAHZAIB NAEEM (@shahzaib_naeem) - wannago4coffe@gmail.com
5. Kemo (@kemo) - kareem.bin104arms@gmail.com
6. Melvin Joe (@melvin_joe) - joemelvin14@gmail.com
7. Ali Asghar (@ali_asghar) - fs.aliasghar@gmail.com
8. Umar Khan (@umar_khan) - talha9355232@gmail.com
9. Faheem Khan (@faheem_khan) - faheem@gmail.com

All users have:
- ✅ Unique usernames assigned
- ✅ Active status
- ✅ Profile data ready for search functionality
```

#### **Next Steps for Future Development:**
- Enhanced profile customization options
- Advanced matching algorithms based on preferences
- Real-time notifications and messaging system
- Social features (followers, following, activity feeds)
- Analytics and insights dashboard

## License

This project is licensed under the MIT License.
