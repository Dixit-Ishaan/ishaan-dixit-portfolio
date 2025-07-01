# replit.md

## Overview

This is a full-stack web application built with a modern TypeScript stack, featuring a personal portfolio website for Ishaan Dixit. The application uses React for the frontend, Express.js for the backend, and is configured with PostgreSQL database support through Drizzle ORM. The project includes a comprehensive UI component library using shadcn/ui and Tailwind CSS for styling.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript
- **Build Tool**: Vite for fast development and optimized builds
- **Styling**: Tailwind CSS with custom design system
- **UI Components**: shadcn/ui component library with Radix UI primitives
- **State Management**: TanStack React Query for server state management
- **Routing**: Wouter for lightweight client-side routing
- **Font System**: Google Fonts (Poppins and Inter)

### Backend Architecture
- **Runtime**: Node.js with TypeScript
- **Framework**: Express.js for REST API
- **Database ORM**: Drizzle ORM with PostgreSQL dialect
- **Database Provider**: Neon Database (serverless PostgreSQL)
- **Session Management**: connect-pg-simple for PostgreSQL-based sessions
- **Development**: tsx for TypeScript execution in development

### Design System
- **Color Scheme**: Navy blue primary theme with gold accents
- **Typography**: Poppins for headings, Inter for body text
- **Component Style**: New York variant of shadcn/ui
- **Responsive Design**: Mobile-first approach with Tailwind breakpoints

## Key Components

### Frontend Components
1. **Portfolio Sections**:
   - Hero section with professional introduction
   - About section with personal background
   - Experience section showcasing work history
   - Skills section with technical and soft skills
   - Achievements section highlighting certifications
   - Contact section with personal information

2. **UI Infrastructure**:
   - Responsive navigation bar
   - Reusable UI components from shadcn/ui
   - Toast notifications system
   - Mobile-responsive design

### Backend Components
1. **Server Setup**: Express server with middleware for JSON parsing and logging
2. **Storage Interface**: Abstracted storage layer with in-memory implementation
3. **Route Management**: Modular route registration system
4. **Development Tools**: Vite integration for hot module replacement

### Database Schema
- **Users Table**: Basic user structure with username and password fields
- **Drizzle Configuration**: PostgreSQL dialect with migrations support
- **Schema Validation**: Zod integration for type-safe data validation

## Data Flow

1. **Client Requests**: React components make API calls using TanStack React Query
2. **Server Processing**: Express routes handle requests and interact with storage layer
3. **Database Operations**: Drizzle ORM manages database queries and migrations
4. **Response Handling**: Structured JSON responses with error handling middleware
5. **State Management**: React Query manages client-side caching and synchronization

## External Dependencies

### Core Framework Dependencies
- **@neondatabase/serverless**: Serverless PostgreSQL connection
- **drizzle-orm**: Type-safe database operations
- **@tanstack/react-query**: Server state management
- **wouter**: Lightweight routing for React

### UI and Styling Dependencies
- **@radix-ui/***: Comprehensive set of UI primitives
- **tailwindcss**: Utility-first CSS framework
- **lucide-react**: Modern icon library
- **class-variance-authority**: Component variant management

### Development Dependencies
- **vite**: Fast build tool and development server
- **tsx**: TypeScript execution for Node.js
- **esbuild**: Fast JavaScript bundler for production builds

## Deployment Strategy

### Development Environment
- **Development Server**: Vite dev server with HMR
- **Backend Development**: tsx for TypeScript execution
- **Database**: Drizzle Kit for schema management and migrations

### Production Build
- **Frontend Build**: Vite builds optimized static assets to `dist/public`
- **Backend Build**: esbuild bundles server code to `dist/index.js`
- **Database**: Environment-based DATABASE_URL configuration
- **Static Serving**: Express serves built frontend assets in production

### Environment Configuration
- **NODE_ENV**: Controls development/production behavior
- **DATABASE_URL**: Required for database connectivity
- **Build Outputs**: Separate client and server build processes

## User Preferences

Preferred communication style: Simple, everyday language.

## Changelog

Changelog:
- June 30, 2025. Initial setup
- June 30, 2025. Updated portfolio with user's professional headshot, changed contact section to light theme with black text and icons, removed resume download functionality per user request, updated DECA role end date to June 2025
- June 30, 2025. Implemented blue and white color scheme throughout site, added dark navigation background with white text, added blue background container to hero section content, adjusted hero section spacing to prevent navbar overlap, changed about section image to show full face