# Just Tech News

A full-stack news aggregation web application where users can post tech articles, upvote submissions, and leave comments. Built with Node.js, Express, Sequelize ORM, and Handlebars templating.

## Features

- User authentication with secure password hashing (bcrypt) and session management
- Create, read, update, and delete news post submissions
- Upvote posts and comment on submissions
- Server-side rendering with Handlebars templating engine
- Persistent data storage with MySQL via Sequelize ORM
- MVC architecture with organized controllers, models, and views
- Database seeding for development and testing

## Tech Stack

**Backend:** Node.js, Express.js, Sequelize ORM, MySQL2  
**Templating:** Express-Handlebars  
**Authentication:** bcrypt, express-session, connect-session-sequelize  
**Testing:** Jest  
**Tools:** dotenv, nodemon

## Installation

1. Clone the repository
   ```bash
   git clone https://github.com/woodb58/just-tech-news.git
   cd just-tech-news
   ```

2. Install dependencies
   ```bash
   npm install
   ```

3. Create a `.env` file in the root directory and add your database credentials
   ```
   DB_NAME=just_tech_news_db
   DB_USER=your_mysql_username
   DB_PASSWORD=your_mysql_password
   SECRET=your_session_secret
   ```

4. Create the database
   ```bash
   mysql -u root -p
   source db/schema.sql
   exit
   ```

5. Seed the database
   ```bash
   npm run seeds
   ```

6. Start the server
   ```bash
   npm start
   ```

   The app will be running at `http://localhost:3001`

## Usage

- Visit the homepage to browse submitted tech articles
- Sign up or log in to submit posts, upvote, and comment
- Manage your own posts from your dashboard

## Testing

```bash
npm test
```

## License

ISC
