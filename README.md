<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dev Portfolio | GitHub</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #24292e;
            --secondary: #0366d6;
            --light: #f6f8fa;
            --dark: #1f2328;
            --text: #24292e;
            --text-light: #57606a;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif;
        }
        
        body {
            background-color: var(--light);
            color: var(--text);
            line-height: 1.6;
        }
        
        header {
            background-color: var(--primary);
            color: white;
            padding: 2rem 0;
            text-align: center;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
        }
        
        .profile {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin-bottom: 2rem;
        }
        
        .avatar {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            border: 5px solid white;
            margin-bottom: 1rem;
            object-fit: cover;
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 0.5rem;
        }
        
        .username {
            font-size: 1.5rem;
            color: #c9d1d9;
            margin-bottom: 1rem;
        }
        
        .bio {
            max-width: 600px;
            margin: 0 auto 1.5rem;
        }
        
        .social-links {
            display: flex;
            gap: 1rem;
            margin-bottom: 1.5rem;
        }
        
        .social-links a {
            color: white;
            font-size: 1.5rem;
            transition: transform 0.3s;
        }
        
        .social-links a:hover {
            transform: translateY(-3px);
        }
        
        .btn {
            display: inline-block;
            background-color: var(--secondary);
            color: white;
            padding: 0.75rem 1.5rem;
            border-radius: 6px;
            text-decoration: none;
            font-weight: 600;
            transition: background-color 0.3s;
            margin: 0.5rem;
        }
        
        .btn:hover {
            background-color: #035fc7;
        }
        
        section {
            padding: 3rem 0;
        }
        
        h2 {
            font-size: 2rem;
            margin-bottom: 2rem;
            text-align: center;
            position: relative;
        }
        
        h2::after {
            content: '';
            display: block;
            width: 80px;
            height: 4px;
            background-color: var(--secondary);
            margin: 0.5rem auto 0;
        }
        
        .projects {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .project-card {
            background-color: white;
            border-radius: 6px;
            overflow: hidden;
            box-shadow: 0 3px 6px rgba(0,0,0,0.1);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }
        
        .project-image {
            width: 100%;
            height: 180px;
            object-fit: cover;
        }
        
        .project-content {
            padding: 1.5rem;
        }
        
        .project-title {
            font-size: 1.25rem;
            margin-bottom: 0.5rem;
        }
        
        .project-description {
            color: var(--text-light);
            margin-bottom: 1rem;
        }
        
        .project-languages {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin-bottom: 1rem;
        }
        
        .language {
            display: inline-block;
            padding: 0.25rem 0.5rem;
            background-color: var(--light);
            border-radius: 20px;
            font-size: 0.8rem;
            color: var(--text-light);
        }
        
        .project-links {
            display: flex;
            justify-content: space-between;
        }
        
        .stats {
            display: flex;
            justify-content: center;
            gap: 2rem;
            flex-wrap: wrap;
            margin-bottom: 3rem;
        }
        
        .stat-item {
            text-align: center;
            background-color: white;
            padding: 1.5rem 2rem;
            border-radius: 6px;
            box-shadow: 0 3px 6px rgba(0,0,0,0.1);
            min-width: 150px;
        }
        
        .stat-number {
            font-size: 2.5rem;
            font-weight: 700;
            color: var(--secondary);
        }
        
        .stat-label {
            color: var(--text-light);
            font-size: 0.9rem;
        }
        
        footer {
            background-color: var(--dark);
            color: white;
            text-align: center;
            padding: 2rem 0;
            margin-top: 2rem;
        }
        
        @media (max-width: 768px) {
            .projects {
                grid-template-columns: 1fr;
            }
            
            .stats {
                flex-direction: column;
                align-items: center;
                gap: 1rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="profile">
                <img src="https://avatars.githubusercontent.com/u/yourusername" alt="Profile" class="avatar">
                <h1>Your Name</h1>
                <div class="username">@yourusername</div>
                <p class="bio">Full-stack developer passionate about building open source projects and contributing to the developer community.</p>
                <div class="social-links">
                    <a href="https://github.com/yourusername" target="_blank"><i class="fab fa-github"></i></a>
                    <a href="https://twitter.com/yourusername" target="_blank"><i class="fab fa-twitter"></i></a>
                    <a href="https://linkedin.com/in/yourusername" target="_blank"><i class="fab fa-linkedin"></i></a>
                </div>
                <a href="https://github.com/yourusername" class="btn" target="_blank">View GitHub Profile</a>
            </div>
        </div>
    </header>
    
    <section id="stats">
        <div class="container">
            <h2>GitHub Stats</h2>
            <div class="stats">
                <div class="stat-item">
                    <div class="stat-number">42</div>
                    <div class="stat-label">Repositories</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">128</div>
                    <div class="stat-label">Contributions</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">24</div>
                    <div class="stat-label">Followers</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">12</div>
                    <div class="stat-label">Following</div>
                </div>
            </div>
        </div>
    </section>
    
    <section id="projects">
        <div class="container">
            <h2>Featured Projects</h2>
            <div class="projects">
                <div class="project-card">
                    <img src="https://via.placeholder.com/600x400?text=Project+1" alt="Project 1" class="project-image">
                    <div class="project-content">
                        <h3 class="project-title">Project One</h3>
                        <p class="project-description">A web application built with React and Node.js that solves problem X.</p>
                        <div class="project-languages">
                            <span class="language">JavaScript</span>
                            <span class="language">React</span>
                            <span class="language">Node.js</span>
                        </div>
                        <div class="project-links">
                            <a href="#" class="btn">View Project</a>
                            <a href="#" class="btn">View Code</a>
                        </div>
                    </div>
                </div>
                
                <div class="project-card">
                    <img src="https://via.placeholder.com/600x400?text=Project+2" alt="Project 2" class="project-image">
                    <div class="project-content">
                        <h3 class="project-title">Project Two</h3>
                        <p class="project-description">Mobile app developed with Flutter for tracking fitness activities.</p>
                        <div class="project-languages">
                            <span class="language">Dart</span>
                            <span class="language">Flutter</span>
                            <span class="language">Firebase</span>
                        </div>
                        <div class="project-links">
                            <a href="#" class="btn">View Project</a>
                            <a href="#" class="btn">View Code</a>
                        </div>
                    </div>
                </div>
                
                <div class="project-card">
                    <img src="https://via.placeholder.com/600x400?text=Project+3" alt="Project 3" class="project-image">
                    <div class="project-content">
                        <h3 class="project-title">Project Three</h3>
                        <p class="project-description">Machine learning model for predicting stock prices with Python.</p>
                        <div class="project-languages">
                            <span class="language">Python</span>
                            <span class="language">TensorFlow</span>
                            <span class="language">Pandas</span>
                        </div>
                        <div class="project-links">
                            <a href="#" class="btn">View Project</a>
                            <a href="#" class="btn">View Code</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <footer>
        <div class="container">
            <p>© 2023 Your Name. All rights reserved.</p>
            <p>Built with ❤️ and GitHub</p>
        </div>
    </footer>
</body>
</html>
