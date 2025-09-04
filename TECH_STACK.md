# 🛠️ Spluno Technology Stack

## Frontend Architecture

### Core Framework
- **Next.js 15.3.4** - React framework with App Router and Server Components
- **React 19.1.0** - Latest React with concurrent features and improved performance
- **TypeScript 5.8.3** - Strict type checking with advanced type inference

### UI Framework & Styling
- **Tailwind CSS 3.4.17** - Utility-first CSS framework with custom design tokens
- **Radix UI** - Accessible, unstyled UI primitives for complex components
- **Lucide React 0.525.0** - Modern icon library with consistent design
- **next-themes 0.4.6** - Dark/light mode support with system preference detection

### State Management
- **TanStack Query 5.83.0** - Server state management with caching and synchronization
- **React Hooks** - Built-in state management for component-level state
- **Context API** - Global state for theme, auth, and user preferences

### 3D Graphics & Animation
- **React Three Fiber 9.3.0** - React renderer for Three.js
- **@react-three/drei 10.6.1** - Useful helpers and abstractions for R3F
- **@react-three/postprocessing 3.0.4** - Post-processing effects for enhanced visuals
- **GSAP 3.13.0** - High-performance animation library
- **three 0.178.0** - 3D graphics library for immersive table visualizations

## Backend & Services

### Authentication & User Management
- **Clerk 6.22.0** - Complete authentication solution with social login
  - Multi-provider social authentication (Google, Facebook, GitHub)
  - User management with profiles and metadata
  - Session management and security features
  - Webhook integration for user lifecycle events

### Database & Storage
- **Appwrite 18.1.1** - Backend-as-a-Service with comprehensive features
  - **8 Collections**: users, tables, join_requests, participants, ratings, reports, notifications, user_settings
  - **Real-time Subscriptions**: Live data synchronization
  - **File Storage**: Image uploads and media management
  - **Database Functions**: Server-side business logic
  - **Security Rules**: Fine-grained access control

### Real-time Communication
- **Stream Chat 9.11.0** - Scalable chat infrastructure
  - **stream-chat-react 13.2.3** - React SDK with pre-built components
  - Direct messaging and group chat
  - File sharing and media support
  - Message reactions and threading
  - Moderation tools and content filtering

### Additional Services
- **QR Code Generation**: qrcode 1.5.4 & qrcode.react 4.2.0
- **QR Scanning**: qr-scanner 1.4.2 for mobile camera integration
- **Date Handling**: date-fns 4.1.0 for robust date manipulation
- **Validation**: Zod 4.0.2 for schema validation and type safety

## Development Tools

### Build & Development
- **Turbopack** - Ultra-fast development builds with Hot Module Replacement
- **Vercel** - Deployment platform with Edge Functions and global CDN
- **Sharp 0.34.3** - High-performance image processing for Next.js Image optimization

### Code Quality & Testing
- **ESLint 9.31.0** - Linting with Next.js recommended configuration
- **TypeScript Strict Mode** - Maximum type safety with strict compiler options
- **React Query Devtools** - Development tools for debugging server state

### UI Development
- **Radix UI Components**:
  - Avatar, Dialog, Dropdown Menu, Label, Popover
  - Progress, Scroll Area, Select, Separator, Slider
  - Switch, Tabs, Toast, Tooltip
- **Class Variance Authority** - Type-safe variant API for components
- **Tailwind Merge** - Intelligent Tailwind class merging
- **clsx** - Conditional class name construction

## Performance & Optimization

### Frontend Optimization
- **Code Splitting** - Automatic route-based code splitting with Next.js
- **Image Optimization** - Next.js Image component with Sharp processing
- **Bundle Analysis** - Webpack bundle analyzer for optimization insights
- **Lazy Loading** - Component and route-level lazy loading

### Caching Strategy
- **TanStack Query** - Intelligent server state caching with background updates
- **Next.js Static Generation** - Pre-rendered pages for optimal performance
- **Edge Caching** - Vercel Edge Network for global content delivery
- **Browser Caching** - Optimized cache headers and service worker support

### Real-time Performance
- **WebSocket Connections** - Persistent connections for real-time features
- **Optimistic Updates** - Immediate UI updates with rollback on failure
- **Connection Resilience** - Automatic reconnection and error handling

## Security Implementation

### Authentication Security
- **Multi-factor Authentication** - Enhanced security with optional 2FA
- **Session Management** - Secure session handling with automatic expiration
- **CSRF Protection** - Cross-site request forgery prevention
- **Rate Limiting** - API endpoint protection against abuse

### Data Security
- **Input Validation** - Server-side validation with Zod schemas
- **SQL Injection Prevention** - Parameterized queries and prepared statements
- **XSS Protection** - Content sanitization and CSP headers
- **HTTPS Enforcement** - End-to-end encryption for all communications

### Access Control
- **Role-based Permissions** - Granular access control based on user roles
- **Resource Authorization** - Per-resource permission checking
- **API Security** - Protected endpoints with proper authentication
- **Data Encryption** - Sensitive data encryption at rest and in transit

## Infrastructure & Deployment

### Hosting & CDN
- **Vercel Platform** - Serverless deployment with global edge network
- **Edge Functions** - Server-side logic at the edge for minimal latency
- **Static Assets** - Optimized delivery of images, fonts, and static content
- **Custom Domains** - Professional domain setup with SSL certificates

### Monitoring & Analytics
- **Error Tracking** - Comprehensive error logging and reporting
- **Performance Monitoring** - Real-time application performance metrics
- **User Analytics** - Privacy-compliant usage tracking and insights
- **Uptime Monitoring** - 24/7 service availability monitoring

### Development Workflow
- **Git Integration** - Automatic deployments on Git push
- **Preview Deployments** - Branch-based preview environments
- **Environment Variables** - Secure configuration management
- **Database Migrations** - Version-controlled schema updates

## Third-party Integrations

### Communication
- **Stream Chat API** - Professional chat infrastructure
- **Email Services** - Transactional email delivery
- **Push Notifications** - Mobile and web push notification support
- **SMS Gateway** - SMS verification and notifications

### Payments & Commerce
- **Stripe Integration** - Secure payment processing (planned)
- **Malaysian Payment Gateways** - Local payment method support
- **Subscription Management** - Recurring billing and plan management
- **Revenue Tracking** - Financial analytics and reporting

### Analytics & Marketing
- **Google Analytics** - User behavior and conversion tracking
- **Social Media APIs** - Social sharing and authentication
- **A/B Testing Platform** - Feature flag and experimentation framework
- **Customer Support** - Integrated help desk and chat support

This comprehensive technology stack enables Spluno to deliver a modern, scalable, and secure nightlife platform that meets the demanding requirements of real-time social interactions and complex business logic.