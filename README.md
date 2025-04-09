# 📚 MERN Book Search Engine (GraphQL Refactor)

Refactored a fully functional Google Books search engine from a RESTful API to a GraphQL API using Apollo Server. This MERN (MongoDB, Express, React, Node.js) stack application allows users to search, save, and manage books via the Google Books API, and integrates secure user authentication.

---

## 📄 Table of Contents
- [Live Demo](#🔗-live-demo)
- [Technologies](#⚖%ef%b8%8f-technologies)
- [Features](#✨-features)
- [Installation](#⚙%ef%b8%8f-installation)
- [Usage](#🔍-usage)
- [GraphQL API](#🖐%ef%b8%8f-graphql-api)
- [Deployment](#🚀-deployment)
- [Screenshots](#📸-screenshots)
- [License](#📃-license)

---

## 🔗 Live Demo
[Deployed Application](https://your-deployment-url.render.com)

---

## ⚖️ Technologies
- MongoDB & Mongoose
- Express.js
- React.js
- Node.js
- Apollo Client & Apollo Server
- GraphQL
- JWT Authentication
- Render Deployment

---

## ✨ Features
- Google Books search engine
- Secure login and signup with JWT
- Save books to user account
- View and remove saved books
- GraphQL used for all API interactions

---

## ⚙️ Installation

1. **Clone the Repository**
```bash
git clone https://github.com/your-username/book-search-graphql.git
cd book-search-graphql
```

2. **Install Dependencies**
```bash
npm install
cd client
npm install
cd ..
```

3. **Environment Variables**
Create a `.env` file in the root:
```
PORT=3001
MONGODB_URI=<your_mongoDB_atlas_uri>
JWT_SECRET=<your_jwt_secret>
```

4. **Start the App**
```bash
npm run develop
```

---

## 🔍 Usage
- Search for books by title or keyword
- Signup/Login to access saving features
- Click "Save This Book" to save to your profile
- View saved books on the "Saved Books" page

---

## 🖐️ GraphQL API

### Queries
```graphql
query Me {
  me {
    _id
    username
    email
    savedBooks {
      bookId
      title
      authors
      description
      image
      link
    }
  }
}
```

### Mutations
```graphql
mutation Login($email: String!, $password: String!)
mutation AddUser($username: String!, $email: String!, $password: String!)
mutation SaveBook($input: BookInput!)
mutation RemoveBook($bookId: String!)
```

---

## 🚀 Deployment
- App deployed on **Render**
- Database hosted on **MongoDB Atlas**

---

## 📸 Screenshots
![Search Page](./Assets/18-mern-homework-demo-01.gif)
![Save Book](./Assets/18-mern-homework-demo-02.gif)
![Saved Books](./Assets/18-mern-homework-demo-03.gif)

---

## 📃 License
This project is licensed under the MIT License.

---

## 👨‍💻 Author
**Your Name**  
GitHub: [@your-username](https://github.com/your-username)

