# Evergreen Consistency Website

A modern, responsive website built with Next.js and Tailwind CSS for Evergreen Consistency, showcasing sustainable solutions and environmental stewardship.

## 🚀 Features

- **Modern Design**: Clean, professional design with a focus on sustainability
- **Responsive**: Fully responsive design that works on all devices
- **Fast Performance**: Built with Next.js for optimal performance
- **SEO Optimized**: Proper meta tags and semantic HTML
- **Accessible**: WCAG compliant design patterns

## 🛠️ Tech Stack

- **Framework**: Next.js 15.3.4
- **Language**: TypeScript
- **Styling**: Tailwind CSS 4
- **React**: React 19
- **Build Tool**: Turbopack

## 📦 Installation

1. Clone the repository:
```bash
git clone https://github.com/Evergreen-Consistency/Evergreen-Consistency-Web.git
cd Evergreen-Consistency-Web
```

2. Install dependencies:
```bash
npm install
```

3. Run the development server:
```bash
npm run dev
```

4. Open [http://localhost:3000](http://localhost:3000) in your browser.

## 🏗️ Build for Production

To create a production build:

```bash
npm run build
```

The build output will be in the `out/` directory, ready for deployment to static hosting services like Cloudflare Pages.

## 🚀 Deployment

### Cloudflare Pages

1. Connect your GitHub repository to Cloudflare Pages
2. Set the build command to: `npm run build`
3. Set the build output directory to: `out`
4. Deploy!

### Other Static Hosting

The `out/` directory contains static files that can be deployed to any static hosting service:
- Vercel
- Netlify
- AWS S3
- GitHub Pages

## 📁 Project Structure

```
├── src/
│   └── app/
│       ├── layout.tsx      # Root layout component
│       ├── page.tsx        # Home page component
│       └── globals.css     # Global styles
├── public/                 # Static assets
├── package.json           # Dependencies and scripts
├── tailwind.config.ts     # Tailwind CSS configuration
├── next.config.ts         # Next.js configuration
├── tsconfig.json          # TypeScript configuration
└── README.md              # This file
```

## 🎨 Customization

### Colors
The website uses a green/emerald color scheme. You can customize colors in `tailwind.config.ts` and the component files.

### Content
Update the content in `src/app/page.tsx` to match your organization's information.

### Styling
Modify `src/app/globals.css` for custom styles and `tailwind.config.ts` for theme customization.

## 📝 Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run lint` - Run ESLint

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📄 License

This project is private and proprietary to Evergreen Consistency.

## 📞 Contact

For questions or support, contact:
- Email: info@evergreenconsistency.com
- Website: https://evergreenconsistency.com

---

Built with ❤️ for a sustainable future. 