# Next.js News App

A **server-side rendered (SSR) news application** built with **Next.js (App Router)** and Tailwind CSS, fetching news dynamically based on categories.

## 🚀 Features
- **Server-Side Rendering (SSR)** for dynamic category-based news fetching.
- **API Routes** for fetching news from an external source.
- **Dynamic Routing** with `/news/[category]` pages.
- **Styled with Tailwind CSS** for responsive and modern UI.
- **Hover Flip Effect** on news cards (without Framer Motion).

## 📂 Folder Structure
```
/nextjs-news-app
│── app/
│   ├── api/news/[category]/route.js  # API route to fetch news
│   ├── news/[category]/page.jsx      # Dynamic news category page
│   ├── layout.jsx                    # Main layout component
│   ├── globals.css                   # Global styles
|   ├── page.jsx                      # Home page
│── components/
│   ├── Card.jsx                       # News card component
|   ├── News.jsx                       # News component for Home page
│── .env.local                         # Environment variables
│── next.config.js                     # Next.js configuration
│── package.json                       # Dependencies
│── README.md                          # Project documentation
```

## 🛠 Installation

1. **Clone the repository**
```sh
git clone https://github.com/your-username/nextjs-news-app.git
cd nextjs-news-app
```

2. **Install dependencies**
```sh
npm install
# OR
yarn install
```

3. **Set up environment variables**
Create a `.env.local` file and add:
```env
NEXT_PUBLIC_BASE_URL=http://localhost:3000
NEWS_API_KEY=your_news_api_key_here
```

4. **Run the development server**
```sh
npm run dev
# OR
yarn dev
```
Visit `http://localhost:3000` in your browser.

## 🔧 API Usage
### **Fetch News by Category**
```
GET /api/news/{category}
```
**Example:**
```
GET /api/news/technology
```
Returns:
```json
{
  "articles": [
    {
      "title": "Tech News",
      "description": "Latest updates in technology...",
      "author": "John Doe",
      "source": { "name": "TechCrunch" }
    }
  ]
}
```



Made with ❤️ using Next.js & Tailwind CSS 🚀

