## 1. Create your portfolio page using HTML tags
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
</head>
<body>

    <header>
        <h1>My Portfolio</h1>
    </header>

    <section class="container">
        <div class="project">
            <h2>Project 1: Title</h2>
            <p>Description of Project 1...</p>
            <img src="pic1.webp" alt="Project 1" style="width: 250px; height: 200px;">

        </div>
        <div class="project">
            <h2>Project 2: Title</h2>
            <p>Description of Project 2...</p>
            <img src="pic2.webp" alt="Project 2" style="width: 250px; height: 200px;">
        </div>
        <!-- Add more projects as needed -->

    </section>

</body>

</html>


2. Update the portfolio page by adding styles to it. Add a contact Us form as well.
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        header {
            background-color: #333;
            color: #fff;
            padding: 20px;
            text-align: center;
        }

        section {
            padding: 20px;
            margin: 20px;
            background-color: #fff;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }

        h1 {
            margin-top: 0;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
        }

        .project {
            margin-bottom: 20px;
        }

        .project img {
            max-width: 100%;
            height: auto;
        }

        .contact-form {
            margin-top: 30px;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            margin-bottom: 5px;
        }

        .form-group input[type="text"],
        .form-group textarea {
            width: 100%;
            padding: 8px;
            border: 1px solid #ccc;
            border-radius: 4px;
            box-sizing: border-box;
        }

        .form-group textarea {
            height: 100px;
        }

        .form-group input[type="submit"] {
            background-color: #333;
            color: #fff;
            border: none;
            padding: 10px 20px;
            border-radius: 4px;
            cursor: pointer;
        }

        .form-group input[type="submit"]:hover {
            background-color: #555;
        }
    </style>
</head>

<body>

    <header>
        <h1>My Portfolio</h1>
    </header>

    <section class="container">
        <div class="project">
            <h2>Project 1: Title</h2>
            <p>Description of Project 1...</p>
            <img src="pic1.jpg" alt="Project 1" style="width: 300px; height: 200px;" >
        </div>
        <div class="project">
            <h2>Project 2: Title</h2>
            <p>Description of Project 2...</p>
            <img src="pic2.webp" alt="Project 2" style="width: 300px; height: 200px;">
        </div>
        <!-- Add more projects as needed -->

        <div class="contact-form">
            <h2>Contact Us</h2>
            <form action="#" method="post">
                <div class="form-group">
                    <label for="name">Name:</label>
                    <input type="text" id="name" name="name" required>
                </div>
                <div class="form-group">
                    <label for="email">Email:</label>
                    <input type="text" id="email" name="email" required>
                </div>
                <div class="form-group">
                    <label for="message">Message:</label>
                    <textarea id="message" name="message" required></textarea>
                </div>
                <div class="form-group">
                    <input type="submit" value="Send Message">
                </div>
            </form>
        </div>
    </section>

</body>

</html>



3. Update the same page using external style sheets or move the added styles to a CSS file and add it to the HTML page
A.	Just separate CSS in experiment 2 into an external file and we have experiment 3


4. Update the portfolio page to use Bootstrap.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

    <header class="bg-dark text-white py-4">
        <div class="container">
            <h1 class="mb-0">My Portfolio</h1>
        </div>
    </header>

    <section class="container mt-4">
        <div class="project">
            <h2>Project 1: Title</h2>
            <p>Description of Project 1...</p>
            <img src="pic1.jpg" alt="Project 1" width="250px" height="150px" class="img-fluid">
        </div>
        <div class="project">
            <h2>Project 2: Title</h2>
            <p>Description of Project 2...</p>
            <img src="pic2.webp" alt="Project 2" width="250px" height="150px" class="img-fluid">
        </div>
        <!-- Add more projects as needed -->

        <div class="contact-form mt-4">
            <h2>Contact Us</h2>
            <form>
                <div class="form-group">
                    <label for="name">Name:</label>
                    <input type="text" id="name" name="name" class="form-control" required>
                </div>
                <div class="form-group">
                    <label for="email">Email:</label>
                    <input type="text" id="email" name="email" class="form-control" required>
                </div>
                <div class="form-group">
                    <label for="message">Message:</label>
                    <textarea id="message" name="message" class="form-control" rows="4" required></textarea>
                </div>
                <div class="form-group">
                    <button type="submit" class="btn btn-dark">Send Message</button>
                </div>
            </form>
        </div>
    </section>

    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.4/dist/umd/popper.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
</body>
</html>



5. Create Home, About Us, Products, Partners, Contact Us pages for a static e-commerce website using Bootstrap. Add a gallery page using Bootstrap grid model. Add Navbar, header and footer to all pages. Add a Login link (Modal).
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>E-commerce Website</title>
    <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">
</head>

<body>

    <!-- Navbar -->
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
        <div class="container">
            <a class="navbar-brand" href="#">E-commerce</a>
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav"
                aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ml-auto">
                    <li class="nav-item active">
                        <a class="nav-link" href="index.html">Home</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="about.html">About Us</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="products.html">Products</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="partners.html">Partners</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="contact.html">Contact Us</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#" data-toggle="modal" data-target="#loginModal">Login</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- Header -->
    <header class="jumbotron jumbotron-fluid text-center bg-secondary text-white">
        <div class="container">
            <h1 class="display-4">Welcome to our E-commerce Website</h1>
            <p class="lead">Discover amazing products and services.</p>
        </div>
    </header>

    <!-- Login Modal -->
    <div class="modal fade" id="loginModal" tabindex="-1" role="dialog" aria-labelledby="loginModalLabel"
        aria-hidden="true">
        <div class="modal-dialog" role="document">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="loginModalLabel">Login</h5>
                    <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                        <span aria-hidden="true">&times;</span>
                    </button>
                </div>
                <div class="modal-body">
                    <!-- Your login form goes here -->
                    <form>
                        <div class="form-group">
                            <label for="username">Username</label>
                            <input type="text" class="form-control" id="username" placeholder="Enter your username">
                        </div>
                        <div class="form-group">
                            <label for="password">Password</label>
                            <input type="password" class="form-control" id="password" placeholder="Enter your password">
                        </div>
                        <button type="submit" class="btn btn-primary">Login</button>
                    </form>
                </div>
            </div>
        </div>
    </div>

    <!-- Main Content -->
    <div class="container mt-5">
        <h2>Home Page</h2>
        <p>This is the home page content.</p>
    </div>

    <!-- Footer -->
    <footer class="bg-dark text-white text-center py-4">
        <div class="container">
            <p>&copy; 2024 E-commerce. All rights reserved.</p>
        </div>
    </footer>

    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.4/dist/umd/popper.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
</body>

</html>



6. . Add a weather component to the home page of the above website, using ReactJS.
Weather component.js
import React, { useState, useEffect } from 'react';
import axios from 'axios';

const WeatherComponent = () => {
  const [weather, setWeather] = useState(null);

  useEffect(() => {
    const fetchWeather = async () => {
      try {
        const response = await axios.get('https://api.openweathermap.org/data/2.5/weather?q=Delhi&appid=142933f6ce24ebbe60293131d8a226eb&units=metric');
        setWeather(response.data);
      } catch (error) {
        console.error('Error fetching weather data:', error);
      }
    };

    fetchWeather();
  }, []);

  return (
    <div className="container mt-5">
      <h2>Weather</h2>
      {weather && (
        <div>
          <p>Temperature: {weather.main.temp}°C</p>
          <p>Description: {weather.weather[0].description}</p>
        </div>
      )}
    </div>
  );
};

export default WeatherComponent;


App.js
import React from 'react';
import 'bootstrap/dist/css/bootstrap.min.css'; // Import Bootstrap CSS
import WebsiteContent from './components/WebsiteContent';
import WeatherComponent from './components/WeatherComponent';

function App() {
  return (
    <div className="App">
      <WebsiteContent />
      <WeatherComponent />
    </div>
  );
}

export default App;


 
7. Update the ‘contact us’ page to a ReactJS component. An email should be sent each time contact us form is submitted
ContactUs.js
import React, { useRef, useEffect } from 'react';
import emailjs from 'emailjs-com';

const ContactUs = () => {
  const form = useRef();

  useEffect(() => {
    emailjs.init('CzjD5B_NCWY5n1cJm'); // Initialize EmailJS with your public key
  }, []);

  const sendEmail = (e) => {
    e.preventDefault();

    emailjs
      .sendForm('service_i88harq', 'template_9kwpa9i', form.current)
      .then(
        () => {
          alert('SUCCESS!');
        },
        (error) => {
          alert(`FAILED... ${error.text}`);
          console.error('EmailJS Error:', error);
        },
      );
  };

  return (
    <form ref={form} onSubmit={sendEmail}>
      <label>Name</label>
      <input type="text" name="user_name" />
      <label>Email</label>
      <input type="email" name="user_email" />
      <label>Message</label>
      <textarea name="message" />
      <input type="submit" value="Send" />
    </form>
  );
};

export default ContactUs;



8. Add a Login component using ReactJS. User should be able to login, using pre-defined logins. Session should be maintained using react hooks
AuthContext.js
import React, { createContext, useState, useEffect } from 'react';

// Create a context for authentication
export const AuthContext = createContext();

const AuthProvider = ({ children }) => {
  const [user, setUser] = useState(null);

  // Load user from localStorage if available
  useEffect(() => {
    const storedUser = localStorage.getItem('user');
    if (storedUser) {
      setUser(JSON.parse(storedUser));
    }
  }, []);

  const login = (username, password) => {
    // Define pre-defined users
    const predefinedUsers = [
      { username: 'user1', password: 'pass1' },
      { username: 'user2', password: 'pass2' },
    ];

    const user = predefinedUsers.find(
      (u) => u.username === username && u.password === password
    );

    if (user) {
      setUser(user);
      localStorage.setItem('user', JSON.stringify(user));
      return true;
    }
    return false;
  };

  const logout = () => {
    setUser(null);
    localStorage.removeItem('user');
  };

  return (
    <AuthContext.Provider value={{ user, login, logout }}>
      {children}
    </AuthContext.Provider>
  );
};

export default AuthProvider;


Login.js
import React, { useState, useContext } from 'react';
import { AuthContext } from './AuthContext';

const LoginPage = () => {
  const [username, setUsername] = useState('');
  const [password, setPassword] = useState('');
  const [error, setError] = useState('');
  const { user, login, logout } = useContext(AuthContext);

  const handleSubmit = (e) => {
    e.preventDefault();
    if (login(username, password)) {
      setError('');
    } else {
      setError('Invalid username or password');
    }
  };

  if (user) {
    return (
      <div className="container">
        <h2>Welcome, {user.username}!</h2>
        <button onClick={logout} className="btn btn-primary">Logout</button>
      </div>
    );
  }

  return (
    <div className="container">
      <h2>Login</h2>
      <form onSubmit={handleSubmit}>
        <div className="form-group">
          <label>Username:</label>
          <input
            type="text"
            className="form-control"
            value={username}
            onChange={(e) => setUsername(e.target.value)}
          />
        </div>
        <div className="form-group">
          <label>Password:</label>
          <input
            type="password"
            className="form-control"
            value={password}
            onChange={(e) => setPassword(e.target.value)}
          />
        </div>
        <button type="submit" className="btn btn-primary">Login</button>
      </form>
      {error && <p style={{ color: 'red' }}>{error}</p>}
    </div>
  );
};

export default LoginPage;


App.js
import React from 'react';
import 'bootstrap/dist/css/bootstrap.min.css'; // Import Bootstrap CSS
import LoginPage from './components/Login';
import AuthProvider from './components/AuthContext';

function App() {
  return (
    <AuthProvider>
      <div className="App">
        <LoginPage />
      </div>
    </AuthProvider>
  );
}
export default App;
9. Each page in the site should be a React JS component and the elements in each page should be child components.
HomeChild.js
import React from 'react';

const HomeChild = () => <div>Home Child Content</div>;

export default HomeChild;


Home.js
import React from 'react';
import HomeChild from './HomeChild';

const Home = () => (
  <div>
    <h2>Home Page</h2>
    <HomeChild />
  </div>
);

export default Home;


AboutChild.js
import React from 'react';

const AboutChild = () => <div>About Child Content</div>;

export default AboutChild;


About.js
import React from 'react';
import AboutChild from './AboutChild';

const About = () => (
  <div>
    <h2>About Page</h2>
    <AboutChild />
  </div>
);

export default About;


App.js
import React from 'react';
import 'bootstrap/dist/css/bootstrap.min.css'; // Import Bootstrap CSS
import WebsiteContent from './components/WebsiteContent';
import Home from './components/Home';
import About from './components/About';

function App() {
  return (
      <div className="App">
        <WebsiteContent />
        <Home />
      </div>
  );
}

export default App;



10. React Routing should be used to take care of routing from browser location bar and also from Navbar
App.js
import React from 'react';
import 'bootstrap/dist/css/bootstrap.min.css'; // Import Bootstrap CSS
import { BrowserRouter as Router, Route, Routes } from 'react-router-dom'; 
import About1 from './components/About1'; 
import Home1 from './components/Home1'; 
import Contact1 from './components/Contact1'; 
import Navbar from './components/Navbar'; 

function App() {
  return (
      <Router>
        <div className="App">
          <Navbar />
          <Routes>
            <Route path="/home1" element={<Home1 />} />
            <Route path="/about1" element={<About1 />} />
            <Route path="/contact1" element={<Contact1 />} />
          </Routes>
          <FooterComponent />
        </div>
      </Router>
  );
}

export default App;


Navbar.js
import React from 'react';
import { Link } from 'react-router-dom';

const Navbar = () => (
    <nav style={{ backgroundColor: '#333', color: '#fff', padding: '10px 0' }}>
        <div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'center', maxWidth: '1200px', margin: '0 auto' }}>
            <Link to="/" style={{ fontSize: '1.5rem', textDecoration: 'none', color: '#fff' }}>
                My Website
            </Link>
            <div style={{ display: 'flex', gap: '20px' }}>
                <Link to="/home1" style={{ textDecoration: 'none', color: '#fff', fontSize: '1.2rem', padding: '10px' }}>
                    Home1
                </Link>
                <Link to="/about1" style={{ textDecoration: 'none', color: '#fff', fontSize: '1.2rem', padding: '10px' }}>
                    About1
                </Link>
                <Link to="/contact1" style={{ textDecoration: 'none', color: '#fff', fontSize: '1.2rem', padding: '10px' }}>
                    Contact1
                </Link>
            </div>
        </div>
    </nav>
);

export default Navbar;


Home1.js
import React from 'react';

const Home1 = () => (
  <div>
    <h1>Home1 Page</h1>
    <p>Welcome to the Home1 page!</p>
  </div>
);

export default Home1;


Contact1.js
import React from 'react';

const About1 = () => (
  <div>
    <h1>About1 Page</h1>
    <p>Welcome to the About1 page!</p>
  </div>
);

export default About1;
About1.js
import React from 'react';

const Contact1 = () => (
  <div>
    <h1>Contact1 Page</h1>
    <p>Welcome to the Contact1 page!</p>
  </div>
);

export default Contact1;


