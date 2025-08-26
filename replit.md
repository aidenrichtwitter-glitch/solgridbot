# Solana Grid Trading Bot

## Overview
A sophisticated automated trading platform built specifically for Solana blockchain that implements grid trading strategies. The application enables users to create and manage multiple grid bot strategies for automated trading on Solana DEXs, with real-time monitoring, Telegram notifications, and comprehensive trade history tracking.

## User Preferences
Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React with TypeScript using Vite as the build tool
- **Styling**: Tailwind CSS with shadcn/ui component library for consistent design system
- **State Management**: TanStack Query (React Query) for server state management and caching
- **Routing**: Wouter for lightweight client-side routing
- **UI Components**: Comprehensive set of Radix UI primitives wrapped in custom components

### Backend Architecture
- **Runtime**: Node.js with Express.js framework
- **Language**: TypeScript with ESM modules
- **Database ORM**: Drizzle ORM with PostgreSQL dialect
- **Architecture Pattern**: RESTful API with service layer architecture
- **Development Setup**: Hot reloading with Vite integration in development mode

### Data Storage Solutions
- **Primary Database**: PostgreSQL with Drizzle ORM for type-safe database operations
- **Connection**: Neon Database serverless PostgreSQL
- **Schema Management**: Drizzle Kit for migrations and schema management
- **Session Storage**: PostgreSQL-backed session store using connect-pg-simple

### Authentication and Authorization
- **Session Management**: Express sessions with PostgreSQL storage
- **User System**: Username/password authentication with encrypted private key storage
- **Wallet Security**: Private keys are stored encrypted in the database

### Trading System Architecture
- **Grid Strategy Engine**: Custom grid bot service that calculates optimal buy/sell levels
- **Price Monitoring**: Real-time price feeds integration
- **Order Management**: Automated order placement and execution tracking
- **Risk Management**: Built-in stop-loss and take-profit mechanisms

### Database Schema Design
Core entities include:
- **Users**: Authentication and profile management
- **Wallets**: Solana wallet integration with encrypted private key storage
- **Strategies**: Grid trading strategy configurations and parameters
- **Trades**: Complete trade execution history and performance tracking
- **Telegram Config**: Bot notification settings and chat management

## External Dependencies

### Blockchain Infrastructure
- **Solana Web3.js**: Primary Solana blockchain interaction library
- **SPL Token**: Solana Program Library for token operations
- **RPC Provider**: QuickNode or custom Solana RPC endpoint for blockchain queries

### Trading and Market Data
- **Jupiter API**: Solana's premier DEX aggregator for price quotes and swap execution
- **Price Feeds**: Real-time market data for strategy execution
- **Token Metadata**: Token information and validation services

### Communication Services
- **Telegram Bot API**: Real-time notifications and command interface
- **Node Telegram Bot API**: TypeScript wrapper for Telegram bot functionality

### Development and Deployment
- **Vite**: Modern build tool with React plugin and hot module replacement
- **Replit Integration**: Development environment with cartographer plugin
- **PostCSS**: CSS processing with Tailwind CSS and Autoprefixer

### Database and Storage
- **Neon Database**: Serverless PostgreSQL hosting
- **Drizzle ORM**: Type-safe database operations and query building
- **Migration System**: Automated database schema versioning

### UI and Styling
- **Tailwind CSS**: Utility-first CSS framework
- **Radix UI**: Headless UI primitives for accessibility
- **Lucide React**: Icon library for consistent iconography
- **Class Variance Authority**: Dynamic styling with variant support