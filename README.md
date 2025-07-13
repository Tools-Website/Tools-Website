<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tools Website - All Your Daily Tools in One Place</title>
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;500;700&family=Inter:wght@300;400;500&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg-main: #0d0f14;
            --bg-nav: #1c222d;
            --bg-sidebar: #12151a;
            --text-primary: #ffffff;
            --text-secondary: #e0e0e0;
            --accent: #42f8f5;
            --accent-glow: rgba(66, 248, 245, 0.6);
            --card-bg: #12151a;
            --transition: all 0.3s ease;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Inter', sans-serif;
            background-color: var(--bg-main);
            color: var(--text-primary);
            line-height: 1.6;
        }
        
        h1, h2, h3, h4 {
            font-family: 'Orbitron', sans-serif;
            font-weight: 500;
        }
        
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header */
        header {
            background-color: var(--bg-nav);
            padding: 15px 0;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
        }
        
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-family: 'Orbitron', sans-serif;
            font-weight: 700;
            font-size: 1.8rem;
            color: var(--text-primary);
            text-decoration: none;
            transition: var(--transition);
        }
        
        .logo:hover {
            text-shadow: 0 0 10px var(--accent-glow);
        }
        
        .logo span {
            color: var(--accent);
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 25px;
        }
        
        nav ul li a {
            color: var(--text-secondary);
            text-decoration: none;
            font-weight: 500;
            transition: var(--transition);
            font-size: 0.95rem;
        }
        
        nav ul li a:hover {
            color: var(--accent);
            text-shadow: 0 0 8px var(--accent-glow);
        }
        
        .contact-link {
            color: var(--accent);
            text-decoration: none;
            transition: var(--transition);
        }
        
        .contact-link:hover {
            text-shadow: 0 0 8px var(--accent-glow);
        }
        
        /* Hero Section */
        .hero {
            padding: 80px 0;
            text-align: center;
            background: linear-gradient(135deg, rgba(28, 34, 45, 0.7) 0%, rgba(13, 15, 20, 1) 100%);
        }
        
        .hero h1 {
            font-size: 2.8rem;
            margin-bottom: 20px;
            line-height: 1.2;
            background: linear-gradient(to right, #ffffff, var(--accent));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        .hero p {
            font-size: 1.2rem;
            color: var(--text-secondary);
            max-width: 700px;
            margin: 0 auto 30px;
        }
        
        .cta-button {
            display: inline-block;
            background-color: var(--card-bg);
            color: var(--accent);
            padding: 12px 30px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 500;
            border: 1px solid var(--accent);
            transition: var(--transition);
            box-shadow: 0 0 15px rgba(66, 248, 245, 0.2);
            font-family: 'Orbitron', sans-serif;
            letter-spacing: 1px;
        }
        
        .cta-button:hover {
            background-color: var(--accent);
            color: var(--bg-main);
            box-shadow: 0 0 20px var(--accent-glow);
            transform: translateY(-3px);
        }
        
        .tool-icons {
            display: flex;
            justify-content: center;
            margin-top: 50px;
            flex-wrap: wrap;
            gap: 20px;
        }
        
        .tool-icon {
            width: 60px;
            height: 60px;
            background-color: var(--card-bg);
            border-radius: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
            transition: var(--transition);
            border: 1px solid rgba(66, 248, 245, 0.2);
        }
        
        .tool-icon:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px var(--accent-glow);
            border-color: var(--accent);
        }
        
        /* Search */
        .search-section {
            padding: 30px 0;
            background-color: rgba(28, 34, 45, 0.3);
        }
        
        .search-container {
            max-width: 700px;
            margin: 0 auto;
        }
        
        .search-bar {
            position: relative;
        }
        
        .search-bar input {
            width: 100%;
            padding: 15px 25px;
            border-radius: 50px;
            border: none;
            background-color: var(--card-bg);
            color: var(--text-primary);
            font-size: 1rem;
            border: 1px solid rgba(66, 248, 245, 0.2);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: var(--transition);
        }
        
        .search-bar input:focus {
            outline: none;
            border-color: var(--accent);
            box-shadow: 0 0 15px var(--accent-glow);
        }
        
        .search-bar input::placeholder {
            color: var(--text-secondary);
            opacity: 0.7;
        }
        
        /* Tools Sections */
        .tools-section {
            padding: 60px 0;
        }
        
        .section-header {
            text-align: center;
            margin-bottom: 40px;
        }
        
        .section-header h2 {
            font-size: 2rem;
            margin-bottom: 10px;
            color: var(--accent);
        }
        
        .section-header p {
            color: var(--text-secondary);
            max-width: 600px;
            margin: 0 auto;
        }
        
        .tools-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 25px;
            margin-top: 30px;
        }
        
        .tool-card {
            background-color: var(--card-bg);
            border-radius: 10px;
            padding: 25px;
            transition: var(--transition);
            border: 1px solid rgba(66, 248, 245, 0.1);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .tool-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px var(--accent-glow);
            border-color: var(--accent);
        }
        
        .tool-card h3 {
            font-size: 1.3rem;
            margin-bottom: 10px;
            color: var(--accent);
        }
        
        .tool-card p {
            color: var(--text-secondary);
            font-size: 0.95rem;
            margin-bottom: 20px;
        }
        
        .tool-card .tool-icon {
            width: 50px;
            height: 50px;
            margin-bottom: 15px;
            background-color: rgba(66, 248, 245, 0.1);
        }
        
        .tool-button {
            display: inline-block;
            background-color: transparent;
            color: var(--accent);
            padding: 8px 20px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 500;
            border: 1px solid var(--accent);
            transition: var(--transition);
            font-size: 0.9rem;
        }
        
        .tool-button:hover {
            background-color: var(--accent);
            color: var(--bg-main);
            box-shadow: 0 0 15px var(--accent-glow);
        }
        
        /* Footer */
        footer {
            background-color: var(--bg-nav);
            padding: 50px 0 20px;
            margin-top: 50px;
        }
        
        .footer-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
        }
        
        .footer-logo {
            font-family: 'Orbitron', sans-serif;
            font-weight: 700;
            font-size: 1.5rem;
            color: var(--text-primary);
            margin-bottom: 15px;
            display: inline-block;
        }
        
        .footer-logo span {
            color: var(--accent);
        }
        
        .footer-about p {
            color: var(--text-secondary);
            margin-bottom: 20px;
            font-size: 0.95rem;
        }
        
        .footer-contact p {
            color: var(--text-secondary);
            margin-bottom: 15px;
        }
        
        .footer-contact a {
            color: var(--accent);
            text-decoration: none;
            transition: var(--transition);
        }
        
        .footer-contact a:hover {
            text-shadow: 0 0 8px var(--accent-glow);
        }
        
        .footer-links h3 {
            color: var(--accent);
            margin-bottom: 20px;
            font-size: 1.2rem;
        }
        
        .footer-links ul {
            list-style: none;
        }
        
        .footer-links ul li {
            margin-bottom: 10px;
        }
        
        .footer-links ul li a {
            color: var(--text-secondary);
            text-decoration: none;
            transition: var(--transition);
            font-size: 0.95rem;
        }
        
        .footer-links ul li a:hover {
            color: var(--accent);
            padding-left: 5px;
        }
        
        .footer-bottom {
            text-align: center;
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: var(--text-secondary);
            font-size: 0.9rem;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .header-container {
                flex-direction: column;
                text-align: center;
            }
            
            nav ul {
                margin-top: 15px;
                justify-content: center;
            }
            
            nav ul li {
                margin: 0 10px;
            }
            
            .hero h1 {
                font-size: 2.2rem;
            }
            
            .hero p {
                font-size: 1rem;
            }
            
            .section-header h2 {
                font-size: 1.8rem;
            }
            
            .tools-grid {
                grid-template-columns: repeat(auto-fill, minmax(240px, 1fr));
            }
        }
        
        @media (max-width: 480px) {
            .hero h1 {
                font-size: 1.8rem;
            }
            
            .section-header h2 {
                font-size: 1.5rem;
            }
            
            .tools-grid {
                grid-template-columns: 1fr;
            }
            
            nav ul {
                flex-wrap: wrap;
            }
            
            nav ul li {
                margin: 5px 10px;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container header-container">
            <a href="#" class="logo">Tools<span>Website</span></a>
            <nav>
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Tools</a></li>
                    <li><a href="#">Contact</a></li>
                    <li><a href="mailto:mbera6669@gmail.com" class="contact-link">mbera6669@gmail.com</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <h1>Your Daily Tools, All in One Place</h1>
            <p>Convert, calculate, compress, and simplify your everyday tasks — fast and free.</p>
            <a href="#" class="cta-button">Explore Tools</a>
            
            <div class="tool-icons">
                <div class="tool-icon">🖼️</div>
                <div class="tool-icon">📄</div>
                <div class="tool-icon">🧮</div>
                <div class="tool-icon">🔤</div>
                <div class="tool-icon">🌐</div>
                <div class="tool-icon">🎨</div>
            </div>
        </div>
    </section>

    <!-- Search -->
    <section class="search-section">
        <div class="container search-container">
            <div class="search-bar">
                <input type="text" placeholder="Search a tool...">
            </div>
        </div>
    </section>

    <!-- Image Tools -->
    <section class="tools-section">
        <div class="container">
            <div class="section-header">
                <h2>🖼 Image Tools</h2>
                <p>Enhance, convert, and optimize your images with our powerful tools</p>
            </div>
            
            <div class="tools-grid">
                <div class="tool-card">
                    <div class="tool-icon">🔄</div>
                    <h3>Image Converter</h3>
                    <p>Convert between JPG, PNG, GIF, WEBP and more formats</p>
                    <a href="image-converter.html" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">🗜️</div>
                    <h3>Image Compressor</h3>
                    <p>Reduce image file size without losing quality</p>
                    <a href="image-compressor.html" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">📏</div>
                    <h3>Image Resizer</h3>
                    <p>Resize images to any dimension while maintaining aspect ratio</p>
                    <a href="image-resizer.html" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">✂️</div>
                    <h3>Image Cropper</h3>
                    <p>Crop images to remove unwanted areas or focus on specific parts</p>
                    <a href="image-crop.html" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">🔤</div>
                    <h3>Image to Text (OCR)</h3>
                    <p>Extract text from images with optical character recognition</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">🔄</div>
                    <h3>Image Rotator/Flipper</h3>
                    <p>Rotate or flip images horizontally/vertically</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Document Tools -->
    <section class="tools-section">
        <div class="container">
            <div class="section-header">
                <h2>📄 Document Tools</h2>
                <p>Manage, convert, and optimize your documents with ease</p>
            </div>
            
            <div class="tools-grid">
                <div class="tool-card">
                    <div class="tool-icon">🔄</div>
                    <h3>PDF to Word</h3>
                    <p>Convert PDF files to editable Word documents</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">🗜️</div>
                    <h3>PDF Compressor</h3>
                    <p>Reduce PDF file size while maintaining quality</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">✂️</div>
                    <h3>PDF Merger & Splitter</h3>
                    <p>Combine multiple PDFs or split pages from a PDF</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">🔄</div>
                    <h3>Document Converter</h3>
                    <p>Convert between various document formats</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">🔒</div>
                    <h3>PDF Lock/Unlock</h3>
                    <p>Add or remove password protection from PDF files</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">✍️</div>
                    <h3>eSign PDF</h3>
                    <p>Add electronic signatures to your PDF documents</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Calculator Tools -->
    <section class="tools-section">
        <div class="container">
            <div class="section-header">
                <h2>🧮 Calculator Tools</h2>
                <p>Perform various calculations for your personal and professional needs</p>
            </div>
            
            <div class="tools-grid">
                <div class="tool-card">
                    <div class="tool-icon">🔢</div>
                    <h3>Scientific Calculator</h3>
                    <p>Advanced calculator with scientific functions</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">🎂</div>
                    <h3>Age Calculator</h3>
                    <p>Calculate age in years, months, and days</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">⚖️</div>
                    <h3>BMI Calculator</h3>
                    <p>Calculate your Body Mass Index</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">💰</div>
                    <h3>Loan EMI Calculator</h3>
                    <p>Calculate Equated Monthly Installments for loans</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">🧾</div>
                    <h3>GST Calculator</h3>
                    <p>Calculate Goods and Services Tax amounts</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">💱</div>
                    <h3>Currency Converter</h3>
                    <p>Convert between world currencies with live rates</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Text Tools -->
    <section class="tools-section">
        <div class="container">
            <div class="section-header">
                <h2>🔤 Text Tools</h2>
                <p>Manipulate and analyze text with our comprehensive text tools</p>
            </div>
            
            <div class="tools-grid">
                <div class="tool-card">
                    <div class="tool-icon">🔄</div>
                    <h3>Text Case Converter</h3>
                    <p>Convert text between uppercase, lowercase and more</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">📊</div>
                    <h3>Word & Character Counter</h3>
                    <p>Count words, characters, sentences and paragraphs</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">🧹</div>
                    <h3>Remove Duplicate Lines</h3>
                    <p>Clean your text by removing duplicate lines</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">🔠</div>
                    <h3>Text Sorter</h3>
                    <p>Sort lines of text alphabetically or numerically</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">🔙</div>
                    <h3>Text Reverser</h3>
                    <p>Reverse text or the order of lines</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">🔐</div>
                    <h3>Text Encryptor/Decryptor</h3>
                    <p>Encrypt and decrypt text with secure algorithms</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Web/Developer Tools -->
    <section class="tools-section">
        <div class="container">
            <div class="section-header">
                <h2>🌐 Web/Developer Tools</h2>
                <p>Essential tools for web developers and programmers</p>
            </div>
            
            <div class="tools-grid">
                <div class="tool-card">
                    <div class="tool-icon">🗜️</div>
                    <h3>HTML/CSS/JS Minifier</h3>
                    <p>Minify your code to reduce file size</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">{} </div>
                    <h3>JSON Formatter & Validator</h3>
                    <p>Format and validate JSON data</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">🔢</div>
                    <h3>Base64 Encoder/Decoder</h3>
                    <p>Encode and decode Base64 strings</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">🔗</div>
                    <h3>URL Encoder/Decoder</h3>
                    <p>Encode and decode URL strings</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">🎨</div>
                    <h3>Color Picker & Converter</h3>
                    <p>Pick colors and convert between formats</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
                
                <div class="tool-card">
                    <div class="tool-icon">.*</div>
                    <h3>Regex Tester</h3>
                    <p>Test and debug regular expressions</p>
                    <a href="#" class="tool-button">Use Tool</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-container">
                <div class="footer-about">
                    <a href="#" class="footer-logo">Tools<span>Website</span></a>
                    <p>Simplifying your digital life with powerful, easy-to-use tools for all your needs.</p>
                </div>
                
                <div class="footer-contact">
                    <h3>Contact Us</h3>
                    <p><a href="mailto:mbera6669@gmail.com">mbera6669@gmail.com</a></p>
                </div>
                
                <div class="footer-links">
                    <h3>Quick Links</h3>
                    <ul>
                        <li><a href="#">Home</a></li>
                        <li><a href="#">All Tools</a></li>
                        <li><a href="#">Privacy Policy</a></li>
                        <li><a href="#">Terms of Use</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="footer-bottom">
                <p>&copy; 2023 Tools Website. All rights reserved.</p>
            </div>
        </div>
    </footer>
</body>
</html>
