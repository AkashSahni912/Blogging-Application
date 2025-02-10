<h1> Blogify </h1>
Blogify is a simple blogging platform built using Node.js, Express, MongoDB, and EJS. It allows users to create, read, and comment on blogs. It also supports user authentication, where users can sign up, sign in, and log out. <br>
<br>
Features <br>
User Authentication: Allows users to sign up, sign in, and log out. <br>
Blog Management: Users can create and view blogs. Admins can manage blog content. <br>
Commenting System: Authenticated users can comment on blogs. <br>
Responsive Design: The platform is designed to be responsive and works well on all devices. <br>
Tech Stack <br>
Backend: Node.js, Express.js <br>
Database: MongoDB <br>
Authentication: JSON Web Tokens (JWT) <br>
Templating Engine: EJS <br>
File Upload: Multer (for blog cover image uploads) <br>
Requirements <br>
Node.js: v14 or above <br>
MongoDB: Make sure you have MongoDB running locally or use MongoDB Atlas. <br>
<br>
<br>
Folder Structure <br>
/blogify <br>
│ <br>
├── /controllers            # Controller files handling routes logic <br>
├── /controllers            # Controller files handling routes logic <br>
├── /models                 # Mongoose models for database collections <br>
├── /public                 # Static files (CSS, JavaScript, images) <br>
│   └── /uploads            # Uploads folder for blog images <br>
├── /routes                 # Route files for different parts of the application <br>
├── /views                  # EJS templates for frontend <br>
├── /middlewares            # Middleware functions (authentication checks) <br>
├── /services               # Utility functions (token creation/validation) <br>
├── .env                    # Environment configuration file <br>
├── package.json            # Project dependencies and scripts <br>
└── server.js               # Main server file <br>
<br>
Routes <br>
GET /: Homepage displaying all blogs. <br>
GET /user/signin: Sign in page. <br>
POST /user/signin: Handles user login and sets a JWT cookie. <br>
GET /user/signup: Sign up page. <br>
POST /user/signup: Handles user registration. <br>
GET /blog/add-new: Page to add a new blog (authenticated users only). <br>
POST /blog: Submit a new blog post. <br>
GET /blog/:id: View a single blog post and its comments. <br>
POST /blog/comment/:blogId: Submit a comment on a blog post. <br>
GET /user/logout: Log out the current user. <br>
Authentication <br>
JWT (JSON Web Tokens) is used for user authentication. Upon signing in, a JWT token is created and stored in a cookie, which is used for protected routes. <br>
<br>
Running Tests <br>
You can run tests using Mocha or any other testing framework of your choice. Currently, no tests have been implemented, but you can add them for further improvements. <br>
<br>
Contributing <br>
Feel free to fork the repository, make changes, and create a pull request. Any improvements or bug fixes are welcome! <br>
 <br>
License <br>
This project is licensed under the MIT License - see the LICENSE file for details, <br>
