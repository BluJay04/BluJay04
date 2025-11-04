<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Arun Mathew - Developer Portfolio</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&family=JetBrains+Mono:wght@400&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Inter', sans-serif;
            background: #000000;
            color: #ffffff;
            min-height: 100vh;
            padding: 60px 24px;
            line-height: 1.6;
        }
        
        .container {
            max-width: 900px;
            margin: 0 auto;
        }
        
        /* Header */
        .header {
            margin-bottom: 80px;
        }
        
        h1 {
            font-size: 2.5rem;
            font-weight: 600;
            color: #ffffff;
            margin-bottom: 24px;
            letter-spacing: -1px;
        }
        
        .wave {
            display: inline-block;
            animation: wave 2s infinite;
            transform-origin: 70% 70%;
        }
        
        @keyframes wave {
            0%, 100% { transform: rotate(0deg); }
            10%, 30% { transform: rotate(14deg); }
            20% { transform: rotate(-8deg); }
            40% { transform: rotate(14deg); }
            50% { transform: rotate(0deg); }
        }
        
        .tagline {
            font-size: 1.125rem;
            color: #999999;
            font-weight: 400;
            line-height: 1.7;
        }
        
        /* Sections */
        .section {
            margin-bottom: 80px;
        }
        
        .section-title {
            font-size: 0.875rem;
            font-weight: 500;
            margin-bottom: 24px;
            color: #666666;
            text-transform: uppercase;
            letter-spacing: 1px;
        }
        
        /* Philosophy code block */
        .code-block {
            background: #0a0a0a;
            border: 1px solid #1a1a1a;
            border-radius: 8px;
            padding: 24px;
            font-family: 'JetBrains Mono', monospace;
            font-size: 0.9rem;
            line-height: 1.8;
        }
        
        .code-line {
            display: block;
            color: #808080;
        }
        
        .code-keyword {
            color: #ffffff;
        }
        
        .code-string {
            color: #cccccc;
        }
        
        /* Tech stack grid */
        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(80px, 1fr));
            gap: 12px;
        }
        
        .tech-item {
            aspect-ratio: 1;
            background: #0a0a0a;
            border: 1px solid #1a1a1a;
            border-radius: 8px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            transition: all 0.2s ease;
            cursor: pointer;
        }
        
        .tech-item:hover {
            background: #1a1a1a;
            border-color: #333333;
        }
        
        .tech-item img {
            width: 32px;
            height: 32px;
            opacity: 0.7;
            transition: opacity 0.2s ease;
        }
        
        .tech-item:hover img {
            opacity: 1;
        }
        
        .tech-name {
            font-size: 0.7rem;
            margin-top: 8px;
            color: #666666;
            font-weight: 500;
        }
        
        /* Connect section */
        .connect-section {
            margin-top: 100px;
            padding-top: 40px;
            border-top: 1px solid #1a1a1a;
        }
        
        .connect-link {
            display: inline-block;
            color: #ffffff;
            text-decoration: none;
            font-size: 1rem;
            font-weight: 500;
            padding-bottom: 2px;
            border-bottom: 1px solid #333333;
            transition: border-color 0.2s ease;
        }
        
        .connect-link:hover {
            border-bottom-color: #ffffff;
        }
        
        @media (max-width: 768px) {
            body {
                padding: 40px 20px;
            }
            
            h1 {
                font-size: 2rem;
            }
            
            .tagline {
                font-size: 1rem;
            }
            
            .section {
                margin-bottom: 60px;
            }
            
            .tech-grid {
                grid-template-columns: repeat(auto-fill, minmax(70px, 1fr));
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>Hi <span class="wave">👋</span>, I'm Arun Mathew</h1>
            <p class="tagline">
                I'm a web developer who turns random ideas into code that occasionally behaves itself. 
                I love experimenting with new tools, fine-tuning interfaces, and figuring out why something 
                works only when it shouldn't. When I'm not deep in code, I'm probably plotting my next side 
                project or pretending to debug life.
            </p>
        </div>
        
        <div class="section">
            <h2 class="section-title">Philosophy</h2>
            <div class="code-block">
                <span class="code-line"><span class="code-keyword">const</span> developer = {</span>
                <span class="code-line">  approach: <span class="code-string">"experiment_first"</span>,</span>
                <span class="code-line">  debugging: <span class="code-string">"life_and_code"</span>,</span>
                <span class="code-line">  expertise: [<span class="code-string">"making_things_work"</span>, <span class="code-string">"when_they_shouldnt"</span>],</span>
                <span class="code-line">  hobby: <span class="code-string">"collecting_side_projects"</span></span>
                <span class="code-line">};</span>
            </div>
        </div>
        
        <div class="section">
            <h2 class="section-title">Tech Stack</h2>
            <div class="tech-grid">
                <div class="tech-item" title="HTML5">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="HTML5">
                    <span class="tech-name">HTML</span>
                </div>
                <div class="tech-item" title="CSS3">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="CSS3">
                    <span class="tech-name">CSS</span>
                </div>
                <div class="tech-item" title="JavaScript">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="JavaScript">
                    <span class="tech-name">JS</span>
                </div>
                <div class="tech-item" title="React">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="React">
                    <span class="tech-name">React</span>
                </div>
                <div class="tech-item" title="Node.js">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original-wordmark.svg" alt="Node.js">
                    <span class="tech-name">Node</span>
                </div>
                <div class="tech-item" title="Express">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/express/express-original-wordmark.svg" alt="Express" style="filter: invert(1) opacity(0.7);">
                    <span class="tech-name">Express</span>
                </div>
                <div class="tech-item" title="MongoDB">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original-wordmark.svg" alt="MongoDB">
                    <span class="tech-name">Mongo</span>
                </div>
                <div class="tech-item" title="Python">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="Python">
                    <span class="tech-name">Python</span>
                </div>
                <div class="tech-item" title="C">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/c/c-original.svg" alt="C">
                    <span class="tech-name">C</span>
                </div>
                <div class="tech-item" title="C++">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg" alt="C++">
                    <span class="tech-name">C++</span>
                </div>
                <div class="tech-item" title="Docker">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original-wordmark.svg" alt="Docker">
                    <span class="tech-name">Docker</span>
                </div>
                <div class="tech-item" title="Git">
                    <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="Git">
                    <span class="tech-name">Git</span>
                </div>
                <div class="tech-item" title="Bootstrap">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg" alt="Bootstrap">
                    <span class="tech-name">Bootstrap</span>
                </div>
                <div class="tech-item" title="Postman">
                    <img src="https://www.vectorlogo.zone/logos/getpostman/getpostman-icon.svg" alt="Postman">
                    <span class="tech-name">Postman</span>
                </div>
            </div>
        </div>
        
        <div class="connect-section">
            <a href="https://www.linkedin.com/in/arunmathewajay/" target="_blank" class="connect-link">
                Let's connect →
            </a>
        </div>
    </div>
</body>
</html>
