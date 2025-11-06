# Book Exchange App

Welcome to the Book Exchange App! This application allows users to buy, sell, and exchange books seamlessly. Below is an overview of the features and structure of the application.

## Features

- **Book Listing**: Users can browse a list of available books for sale.
- **Search and Filter**: Users can search for specific books and filter results based on categories and price range.
- **User Messaging**: Buyers and sellers can communicate through a messaging interface.
- **User Authentication**: Users can register and log in to their accounts securely.
- **Seller Account Management**: Sellers can manage their listings and view inquiries.
- **Admin Dashboard**: Admins can oversee users and manage the platform effectively.
- **Automatic Delisting of Sold Books**: Sold books are automatically removed from the listings.

## Project Structure

```
book-exchange-app
├── src
│   ├── app
│   │   ├── layout.tsx
│   │   ├── page.tsx
│   │   ├── books
│   │   │   ├── page.tsx
│   │   │   └── [id]
│   │   │       ├── page.tsx
│   │   │       └── edit.tsx
│   │   ├── search
│   │   │   └── page.tsx
│   │   ├── auth
│   │   │   ├── login
│   │   │   │   └── page.tsx
│   │   │   └── register
│   │   │       └── page.tsx
│   │   ├── seller
│   │   │   └── dashboard
│   │   │       ├── page.tsx
│   │   │       └── listings.tsx
│   │   ├── messages
│   │   │   ├── page.tsx
│   │   │   └── [conversationId].tsx
│   │   └── admin
│   │       ├── page.tsx
│   │       └── users.tsx
│   ├── components
│   │   ├── BookCard.tsx
│   │   ├── BookList.tsx
│   │   ├── SearchBar.tsx
│   │   ├── Filters.tsx
│   │   ├── Navbar.tsx
│   │   └── Pagination.tsx
│   ├── hooks
│   │   ├── useAuth.ts
│   │   ├── useBooks.ts
│   │   └── useDebounce.ts
│   ├── lib
│   │   ├── db.ts
│   │   ├── auth.ts
│   │   ├── mailer.ts
│   │   └── jobs
│   │       └── delistSoldBooks.ts
│   ├── pages
│   │   └── api
│   │       ├── auth
│   │       │   ├── login.ts
│   │       │   ├── register.ts
│   │       │   └── session.ts
│   │       ├── books
│   │       │   ├── index.ts
│   │       │   ├── [id].ts
│   │       │   └── search.ts
│   │       ├── messages
│   │       │   ├── index.ts
│   │       │   └── [conversationId].ts
│   │       ├── sellers
│   │       │   └── listings.ts
│   │       └── admin
│   │           └── stats.ts
│   ├── styles
│   │   └── globals.css
│   └── types
│       └── index.ts
├── prisma
│   └── schema.prisma
├── scripts
│   └── run-delist-job.ts
├── .env.example
├── next.config.js
├── next-env.d.ts
├── tailwind.config.js
├── postcss.config.js
├── package.json
├── tsconfig.json
├── .eslintrc.json
└── README.md
```

## Getting Started

To get started with the Book Exchange App, follow these steps:

1. Clone the repository:
   ```
   git clone <repository-url>
   ```

2. Navigate to the project directory:
   ```
   cd book-exchange-app
   ```

3. Install the dependencies:
   ```
   npm install
   ```

4. Set up your environment variables by copying `.env.example` to `.env` and filling in the required values.

5. Run the development server:
   ```
   npm run dev
   ```

6. Open your browser and navigate to `http://localhost:3000` to view the application.

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue for any suggestions or improvements.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.