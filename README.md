# 🚀 Portfolio Website with CRUD Management System

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Visit%20Site-blue)](https://rahmatez.github.io)
[![GitHub](https://img.shields.io/badge/GitHub-Repository-green)](https://github.com/rahmatez/rahmatez.github.io)
[![License](https://img.shields.io/badge/License-MIT-yellow)](LICENSE)

> Modern, responsive portfolio website dengan sistem admin dashboard untuk mengelola konten secara real-time menggunakan localStorage dan IndexedDB.

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Admin Dashboard](#admin-dashboard)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Security](#security)
- [Contributing](#contributing)
- [License](#license)

## 🎯 Overview

Portfolio website modern yang dibangun dengan **vanilla JavaScript** dan dilengkapi dengan sistem **CRUD (Create, Read, Update, Delete)** management yang powerful. Website ini menggunakan **localStorage** dan **IndexedDB** untuk penyimpanan data tanpa memerlukan database backend.

### 🌟 Key Highlights

- **Responsive Design** - Mobile-first approach dengan UI yang elegan
- **Admin Dashboard** - Kelola projects, blogs, dan contact messages
- **Authentication System** - Secure login dengan session management
- **Real-time Updates** - Perubahan langsung terlihat di website
- **No Backend Required** - Data tersimpan di browser storage
- **Modern UI/UX** - Clean dan professional design

## ✨ Features

### 🎨 Frontend Features

- **Responsive Layout** - Optimal di semua device
- **Modern Animation** - Smooth transitions dan hover effects
- **Dark/Light Theme** - (Coming soon)
- **Fast Loading** - Optimized performance
- **SEO Friendly** - Meta tags dan sitemap

### 🔧 Admin Features

- **Project Management** - CRUD operations untuk portfolio projects
- **Blog Management** - Manage blog posts dengan rich content
- **Contact Management** - Handle contact messages dengan status tracking
- **User Authentication** - Secure login system
- **Data Export/Import** - Backup dan restore data
- **Statistics Dashboard** - Overview metrics dan analytics

### 📱 Pages

- **Home** - About me dan overview
- **Resume** - Professional experience dan skills
- **Portfolio** - Projects showcase dengan filtering
- **Blog** - Articles dan posts
- **Contact** - Contact form dengan validation
- **Admin Dashboard** - Content management system

## 🛠️ Tech Stack

### Frontend

- **HTML5** - Semantic markup
- **CSS3** - Modern styling dengan custom properties
- **JavaScript (ES6+)** - Vanilla JS untuk interactivity
- **Ion Icons** - Icon library
- **Google Fonts** - Typography

### Data Storage

- **localStorage** - Projects dan blog data
- **IndexedDB** - Contact messages storage
- **Session Storage** - Authentication sessions

### Development Tools

- **Live Server** - Development server
- **Git** - Version control
- **GitHub Pages** - Hosting platform

## 🚀 Getting Started

### Prerequisites

- Web browser modern (Chrome, Firefox, Safari, Edge)
- Code editor (VS Code recommended)
- Live Server extension (untuk development)

### Installation

1. **Clone repository**

   ```bash
   git clone https://github.com/rahmatez/rahmatez.github.io.git
   cd rahmatez.github.io
   ```

2. **Open dengan Live Server**

   - Buka project di VS Code
   - Right-click pada `index.html`
   - Select "Open with Live Server"

3. **Atau buka langsung di browser**
   ```
   file:///path/to/project/index.html
   ```

### First Time Setup

1. **Akses Admin Dashboard**

   - Kunjungi `/pages/login.html`
   - Username: `admin`
   - Password: `rahmatez2024`

2. **Customize Content**
   - Edit personal information di admin dashboard
   - Upload projects dan blog posts
   - Customize styling di `/assets/css/style.css`

## 🔐 Admin Dashboard

### Login Credentials

```
Username: admin
Password: rahmatez2024
```

⚠️ **Security Notice**: Ganti password default setelah setup pertama!

### Dashboard Features

#### 📊 Dashboard Overview

- Statistics dan metrics
- Recent activities
- Quick actions

#### 🎯 Project Management

- **Create**: Tambah project baru dengan image, description, dan tech stack
- **Read**: View semua projects dengan filtering
- **Update**: Edit project details
- **Delete**: Hapus project (dengan confirmation)

#### 📝 Blog Management

- **Create**: Publish blog posts dengan rich content
- **Read**: Manage semua blog posts
- **Update**: Edit existing posts
- **Delete**: Remove posts

#### 📧 Contact Management

- **View**: Semua contact messages
- **Status**: Mark as read/unread
- **Reply**: Send responses (coming soon)
- **Delete**: Remove messages

#### ⚙️ Settings

- **Profile**: Update admin profile
- **Security**: Change password
- **Export**: Backup data
- **Import**: Restore data

## 📁 Project Structure

```
rahmatez.github.io/
├── index.html              # Main homepage
├── CNAME                   # GitHub Pages domain
├── sitemap.xml            # SEO sitemap
├── README.md              # Documentation
├── assets/
│   ├── css/
│   │   ├── style.css      # Main stylesheet
│   │   └── admin.css      # Admin dashboard styles
│   ├── js/
│   │   ├── script.js      # Main JavaScript
│   │   ├── auth-manager.js    # Authentication system
│   │   ├── crud-projects.js   # Project CRUD operations
│   │   ├── crud-blogs.js      # Blog CRUD operations
│   │   ├── crud-contact.js    # Contact CRUD operations
│   │   ├── admin.js           # Admin dashboard logic
│   │   └── blog-display.js    # Blog display functions
│   ├── images/            # Images dan assets
│   └── cv/               # Resume/CV files
├── pages/
│   ├── admin.html        # Admin dashboard
│   ├── login.html        # Login page
│   ├── blog.html         # Blog listing
│   ├── contact.html      # Contact form
│   ├── project.html      # Project showcase
│   └── resume.html       # Resume/CV page
└── debug/               # Development dan testing files
```

## 🎯 Usage

### For Visitors

1. **Browse Portfolio** - Lihat projects dan experience
2. **Read Blog** - Articles dan insights
3. **Contact** - Send messages melalui contact form
4. **Download CV** - Get resume/CV

### For Admin

1. **Login** - Access admin dashboard
2. **Manage Content** - CRUD operations
3. **Monitor Messages** - Handle contact inquiries
4. **Update Portfolio** - Keep content fresh

### Code Examples

#### Adding New Project

```javascript
const projectManager = new ProjectManager();
const newProject = projectManager.createProject({
  title: "Awesome Project",
  category: "web development",
  image: "assets/images/project-new.jpg",
  description: "Project description here...",
  technologies: ["HTML", "CSS", "JavaScript"],
  link: "https://project-link.com",
});
```

#### Managing Blog Posts

```javascript
const blogManager = new BlogManager();
const newBlog = blogManager.createBlog({
  title: "My New Blog Post",
  category: "technology",
  image: "assets/images/blog-new.jpg",
  content: "Blog content here...",
  externalLink: "https://blog-link.com",
});
```

## 🔒 Security

### Authentication Features

- **Password Hashing** - Passwords di-hash sebelum disimpan
- **Session Management** - Automatic session timeout
- **CSRF Protection** - Token-based validation
- **Input Validation** - Sanitize semua user inputs

### Best Practices

- Ganti password default setelah setup
- Regular backup data
- Monitor admin access
- Keep browser updated

### Security Headers

```html
<meta http-equiv="Content-Security-Policy" content="default-src 'self'" />
<meta http-equiv="X-Content-Type-Options" content="nosniff" />
<meta http-equiv="X-Frame-Options" content="DENY" />
```

## 🤝 Contributing

Kontribusi sangat welcome! Berikut cara contribute:

1. **Fork** repository
2. **Create feature branch** (`git checkout -b feature/amazing-feature`)
3. **Commit changes** (`git commit -m 'Add amazing feature'`)
4. **Push to branch** (`git push origin feature/amazing-feature`)
5. **Open Pull Request**

### Development Guidelines

- Follow existing code style
- Add comments untuk complex logic
- Test semua changes sebelum commit
- Update documentation jika needed

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Rahmat Ashari**

- GitHub: [@rahmatez](https://github.com/rahmatez)
- Email: rahmatezdev@gmail.com
- Website: [rahmatez.github.io](https://rahmatez.github.io)

## 🙏 Acknowledgments

- [Ion Icons](https://ionic.io/ionicons) - Beautiful icons
- [Google Fonts](https://fonts.google.com) - Typography
- [GitHub Pages](https://pages.github.com) - Free hosting
- Community feedback dan support

---

⭐ **Star this repository** jika helpful!

📧 **Questions?** Feel free to reach out via email atau create an issue.

🚀 **Live Demo**: [rahmatez.github.io](https://rahmatez.github.io)
