# Evan Rosado - Professional Portfolio

This repository contains my professional portfolio showcasing expertise in network security engineering, platform engineering, and full-stack development.

## 🌐 Live Portfolio

Visit the live portfolio at: **[evanusmodestus.github.io](https://evanusmodestus.github.io)**

## 📁 Repository Structure

```
├── index.adoc                    # Main portfolio page
├── 01_PROJECTS/                  # Featured projects
│   ├── 2025-PROJ-WEB-001-domus-digitalis.adoc
│   ├── 2025-PROJ-NET-001-ise-automation-suite.adoc
│   └── ...
├── 02_WRITING/                   # Technical articles
│   ├── 2025-WRITE-ISE-001-nine-years-experience.adoc
│   └── ...
├── 03_EXPERIENCE/                # Professional experience details
├── assets/                       # CSS, images, and other assets
│   ├── css/portfolio.css
│   └── images/
└── .github/workflows/            # GitHub Actions for automated publishing
    └── publish-portfolio.yml
```

## 🛠 Technology Stack

- **Content Format**: AsciiDoc for rich technical documentation
- **Styling**: Custom CSS with dark mode support
- **Build System**: GitHub Actions with AsciiDoctor
- **Hosting**: GitHub Pages
- **Features**: Code copy functionality, responsive design, professional styling

## 🚀 Key Features

### Professional Content
- **9+ years of Cisco ISE experience** with production insights
- **Full-stack development projects** with real-world implementation details
- **Network automation expertise** with Python and infrastructure as code
- **Technical writing** covering enterprise security and platform engineering

### Technical Implementation
- **AsciiDoc-powered**: Rich documentation with code syntax highlighting
- **Responsive Design**: Professional appearance across all devices
- **Code Copy Functionality**: Interactive code blocks with copy-to-clipboard
- **Dark Mode Support**: Automatic theme detection and switching
- **Performance Optimized**: Fast loading with efficient CSS and minimal JavaScript

## 📖 Content Highlights

### Featured Projects

1. **[Domus Digitalis](01_PROJECTS/2025-PROJ-WEB-001-domus-digitalis.adoc)** - Full-stack portfolio platform
2. **[ISE Automation Suite](01_PROJECTS/2025-PROJ-NET-001-ise-automation-suite.adoc)** - Enterprise network access control automation
3. **Knowledge Management System** - Sophisticated personal knowledge management
4. **Development Environment** - Cross-platform dotfiles and automation

### Technical Writing

- **Nine Years of Cisco ISE**: Production insights and automation strategies
- **Network to Full-Stack Journey**: Transitioning from network engineering to development
- **Enterprise Automation**: Python-based network infrastructure automation
- **Platform Engineering**: Modern DevOps and infrastructure practices

## 🔧 Local Development

### Prerequisites

- Ruby with AsciiDoctor gem
- Modern web browser for testing

### Setup

```bash
# Clone the repository
git clone https://github.com/EvanusModestus/EvanusModestus.git
cd EvanusModestus

# Install AsciiDoctor
gem install asciidoctor rouge

# Build the site locally
mkdir -p _site

# Convert main page
asciidoctor \
  -a toc=left \
  -a toclevels=3 \
  -a numbered \
  -a icons=font \
  -a source-highlighter=rouge \
  -a stylesheet=assets/css/portfolio.css \
  -a linkcss \
  -D _site \
  index.adoc

# Copy assets
cp -r assets _site/

# Serve locally (Python 3)
cd _site && python -m http.server 8000
```

Visit `http://localhost:8000` to view the portfolio locally.

## 📝 Content Guidelines

### File Naming Convention

All content follows an ID-based naming structure:

```
YYYY-CATEGORY-TYPE-###-description.adoc

Where:
- YYYY = Year
- CATEGORY = PROJ (Projects), WRITE (Writing), EXP (Experience)
- TYPE = Technology/focus area (WEB, NET, DEV, SYS, etc.)
- ### = Sequential number
- description = Brief descriptive name
```

### AsciiDoc Standards

- Use semantic markup for better accessibility
- Include table of contents for articles longer than 500 words
- Add source highlighting for all code blocks
- Maintain consistent heading hierarchy
- Include author metadata and revision dates

## 🚀 Deployment

The portfolio automatically builds and deploys via GitHub Actions when:

1. **Manual trigger**: Using the workflow dispatch button
2. **Automatic**: On push to main/master branch when AsciiDoc files change

### Deployment Process

1. Checkout repository
2. Install Ruby and AsciiDoctor
3. Convert all AsciiDoc files to HTML
4. Apply custom CSS styling
5. Add interactive JavaScript features
6. Deploy to GitHub Pages

## 🎯 Performance Features

- **Minimal Dependencies**: Only AsciiDoctor for building
- **Optimized CSS**: Single stylesheet with efficient selectors
- **Progressive Enhancement**: Core content works without JavaScript
- **Responsive Design**: Mobile-first approach with desktop enhancements
- **Fast Loading**: Optimized images and minimal resource usage

## 🔗 Professional Links

- **LinkedIn**: [/in/evanjrosado](https://www.linkedin.com/in/evanjrosado/)
- **Email**: evan.rosado@outlook.com
- **Blog**: [blog.evanusmodestus.dev](https://blog.evanusmodestus.dev)
- **Portfolio**: [domusdigitalis.dev](https://domusdigitalis.dev) *(Coming Soon)*

## 📄 License

This portfolio content is © 2025 Evan Rosado. All rights reserved.

The CSS framework and build system are available under MIT license for educational purposes.

---

**Connect • Automate • Secure • Innovate**

*Professional Portfolio | Network Security Engineer | Aspiring Platform Engineer*