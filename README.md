# Axipays Payment Dashboard

A modern, secure, and user-friendly payment processing dashboard built with React and TypeScript. This application provides a seamless interface for managing payments and transactions through the Axipays platform.

## 🚀 Features

- **Secure Payment Processing**
  - Integrated iframe-based payment system
  - Real-time payment status updates
  - Comprehensive transaction management
  - Secure credit card handling

- **Transaction Management**
  - Create and track transactions
  - Real-time status updates (pending, success, failed)
  - Transaction history with local storage persistence
  - WebSocket-based real-time updates

## 🛠️ Technology Stack

- **Frontend Framework**: React with TypeScript
- **State Management**: React Context API
- **Routing**: React Router
- **Data Fetching**: React Query (TanStack Query)
- **UI Components**: Custom UI components with modern design
- **Real-time Updates**: WebSocket integration
- **Storage**: Local Storage for transaction persistence

## 📁 Project Structure

```
src/
├── components/         # Reusable UI components
├── context/           # React Context providers
├── hooks/             # Custom React hooks
├── integrations/      # External service integrations
├── lib/              # Utility functions
├── pages/            # Route components
└── main.tsx          # Application entry point
```

## 🔑 Key Components

### PaymentIframe
- Handles secure payment processing
- Communicates with external payment service
- Manages payment form data and status updates
- Implements security measures for iframe communication

### PaymentContext
- Central state management for transactions
- Provides transaction CRUD operations
- Handles real-time updates via WebSocket
- Manages local storage persistence

## 🗺️ Application Routes

- `/` - Home/Index page
- `/checkout` - Payment checkout page
- `/payment-status/:id/:status` - Payment status page
- `*` - 404 Not Found page

## 🔄 Data Flow

1. User initiates payment
2. Payment data is collected and validated
3. Transaction is created and stored
4. Payment is processed through iframe
5. Status updates are received via WebSocket
6. UI is updated with transaction status
7. User is notified of payment outcome

## 🛡️ Security Features

- Secure iframe integration for payment processing
- Origin verification for iframe communication
- Sandboxed iframe with restricted permissions
- Secure handling of sensitive payment data

## 💅 UI/UX Features

- Modern, responsive design
- Toast notifications for status updates
- Tooltip provider for enhanced user experience
- Card-based layout for payment information
- Real-time status updates
- User-friendly error handling

## ⚠️ Error Handling

- Graceful error handling for failed payments
- Error notifications via toast messages
- Fallback UI for failed states
- 404 handling for invalid routes

## 🚀 Getting Started

1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```

## 🔧 Environment Setup

Create a `.env` file in the root directory with the following variables:

```env
VITE_API_URL=your_api_url
VITE_IFRAME_URL=your_iframe_url
```

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📧 Support

For support, email support@axipays.com or join our Slack channel.

---

Built with ❤️ by the Axipays Team
