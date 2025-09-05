# Monotree Marketing Website

## Overview

This is a modern marketing website for Monotree, a mobile-first employee experience platform targeting hourly teams. The application is built as a full-stack TypeScript application featuring a React frontend with server-side Express.js backend, designed to showcase Monotree's communication, onboarding, operations, and wellbeing features through an interactive landing page with demo request functionality.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript using Vite as the build tool
- **UI Framework**: Shadcn/ui components built on Radix UI primitives for accessibility
- **Styling**: Tailwind CSS with custom design system using CSS variables for theming
- **State Management**: TanStack Query (React Query) for server state management
- **Routing**: Wouter for lightweight client-side routing
- **Form Handling**: React Hook Form with Zod validation for type-safe form management

### Backend Architecture
- **Runtime**: Node.js with Express.js framework
- **Database ORM**: Drizzle ORM with PostgreSQL dialect for type-safe database operations
- **API Design**: RESTful endpoints with JSON responses
- **Validation**: Zod schemas shared between frontend and backend for consistent validation
- **Development**: Hot module replacement via Vite integration in development mode

### Data Storage Solutions
- **Primary Database**: PostgreSQL configured through Drizzle ORM
- **Connection**: Neon Database serverless PostgreSQL for cloud hosting
- **Schema Management**: Drizzle Kit for migrations and schema management
- **Fallback Storage**: In-memory storage implementation for development/testing

### Database Schema
- **Users Table**: Basic user authentication with username/password
- **Demo Requests Table**: Captures lead information including name, email, company, and employee count
- **UUID Generation**: PostgreSQL native UUID generation for primary keys
- **Timestamps**: Automatic timestamp tracking for demo request creation

### Authentication and Authorization
- **Session Management**: Express sessions with PostgreSQL session store via connect-pg-simple
- **Password Security**: Basic password storage (ready for bcrypt integration)
- **CORS Configuration**: Configured for cross-origin requests with credentials

### Development and Build Process
- **Build System**: Vite for frontend bundling with React plugin
- **Backend Building**: ESBuild for server-side bundling to ESM format
- **Development Server**: Integrated Vite dev server with Express API proxy
- **Type Safety**: Shared TypeScript types between frontend and backend via workspace setup

### Design System
- **Color Palette**: Dark theme with blue/green gradient accents
- **Typography**: Inter font family for consistent branding
- **Component Library**: Comprehensive UI component system with variants
- **Responsive Design**: Mobile-first approach with desktop optimization
- **Accessibility**: WCAG compliant components via Radix UI primitives

## External Dependencies

### Database and Hosting
- **Neon Database**: Serverless PostgreSQL hosting platform
- **Database URL**: Environment variable configuration for database connections

### UI and Design
- **Google Fonts**: Inter font family hosted via Google Fonts CDN
- **Radix UI**: Comprehensive primitive component library for accessibility
- **Tailwind CSS**: Utility-first CSS framework for styling
- **Shadcn/ui**: Pre-built component system built on Radix UI

### Development Tools
- **Replit Integration**: Development environment integration with error handling and debugging tools
- **Vite Plugins**: Hot reload, runtime error overlay, and development tooling
- **TypeScript**: Full type safety across frontend and backend

### Form and Validation
- **Zod**: Runtime type validation and schema definition
- **React Hook Form**: Performant form library with minimal re-renders
- **Hookform Resolvers**: Integration between React Hook Form and Zod

### State Management and API
- **TanStack Query**: Server state management with caching and synchronization
- **Wouter**: Lightweight routing library for single-page application navigation

### Development and Build
- **ESBuild**: Fast JavaScript/TypeScript bundler for production builds
- **PostCSS**: CSS processing with Tailwind CSS integration
- **TSX**: TypeScript execution for development server