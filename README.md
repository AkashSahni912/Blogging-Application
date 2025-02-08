Blogify
Blogify is a simple blogging platform built using Node.js, Express, MongoDB, and EJS. It allows users to create, read, and comment on blogs. It also supports user authentication, where users can sign up, sign in, and log out.

Features
User Authentication: Allows users to sign up, sign in, and log out.
Blog Management: Users can create and view blogs. Admins can manage blog content.
Commenting System: Authenticated users can comment on blogs.
Responsive Design: The platform is designed to be responsive and works well on all devices.
Tech Stack
Backend: Node.js, Express.js
Database: MongoDB
Authentication: JSON Web Tokens (JWT)
Templating Engine: EJS
File Upload: Multer (for blog cover image uploads)
Requirements
Node.js: v14 or above
MongoDB: Make sure you have MongoDB running locally or use MongoDB Atlas.


Folder Structure
/blogify
│
├── /controllers            # Controller files handling routes logic
├── /models                 # Mongoose models for database collections
├── /public                 # Static files (CSS, JavaScript, images)
│   └── /uploads            # Uploads folder for blog images
├── /routes                 # Route files for different parts of the application
├── /views                  # EJS templates for frontend
├── /middlewares            # Middleware functions (authentication checks)
├── /services               # Utility functions (token creation/validation)
├── .env                    # Environment configuration file
├── package.json            # Project dependencies and scripts
└── server.js               # Main server file

Routes
GET /: Homepage displaying all blogs.
GET /user/signin: Sign in page.
POST /user/signin: Handles user login and sets a JWT cookie.
GET /user/signup: Sign up page.
POST /user/signup: Handles user registration.
GET /blog/add-new: Page to add a new blog (authenticated users only).
POST /blog: Submit a new blog post.
GET /blog/:id: View a single blog post and its comments.
POST /blog/comment/:blogId: Submit a comment on a blog post.
GET /user/logout: Log out the current user.
Authentication
JWT (JSON Web Tokens) is used for user authentication. Upon signing in, a JWT token is created and stored in a cookie, which is used for protected routes.

Running Tests
You can run tests using Mocha or any other testing framework of your choice. Currently, no tests have been implemented, but you can add them for further improvements.

Contributing
Feel free to fork the repository, make changes, and create a pull request. Any improvements or bug fixes are welcome!

License
This project is licensed under the MIT License - see the LICENSE file for details,
