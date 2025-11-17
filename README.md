✨ Personal Portfolio – Yoga Rizky Alkautsar

This is my personal portfolio website built using Astro and Tailwind CSS.
The goal of this project is to showcase my experience, skills, and projects as an IT Support Supervisor and Web Developer.

The portfolio is fully responsive, clean, and minimalistic — featuring light/dark mode support, modern UI, project cards, and content sections.

Live Demo:
👉 https://personal-portofolio-yoga.vercel.app/

🚀 Tech Stack

Astro – Static-first site builder

Tailwind CSS – Utility-first CSS for styling

Vercel – Hosting & automatic builds

JavaScript – Basic interactivity

LocalStorage – Saving theme preferences

🌙 Features
✔ Clean & Minimal UI

Professionally designed layout with balanced spacing, typography, and structure.

✔ Dark Mode Toggle

Users can switch between light and dark mode.
Preference is saved using localStorage.

✔ Fully Responsive

Optimized for mobile, tablet, and desktop.

✔ Sectioned Layout

Includes:

Hero

About

Skills

Projects

Contact

✔ Reusable Components

ProjectCard.astro

SkillBadge.astro

Header.astro

BaseLayout.astro

✔ Custom Styling

Global styles using Tailwind + custom .section class for boxed sections.

📁 Project Structure
/
├── public/
│   └── images/
│       └── profile.jpg
│
├── src/
│   ├── components/
│   │   ├── Header.astro
│   │   ├── ProjectCard.astro
│   │   └── SkillBadge.astro
│   │
│   ├── layouts/
│   │   └── BaseLayout.astro
│   │
│   ├── pages/
│   │   └── index.astro
│   │
│   └── styles/
│       └── global.css
│
└── README.md

🛠 Installation & Development

Clone repository:

git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME


Install dependencies:

npm install


Start local dev server:

npm run dev


Build for production:

npm run build


Preview build:

npm run preview

🔧 Deployment

This project is deployed on Vercel.

Every push to the main branch triggers an automatic rebuild and deployment.

To deploy manually:

vercel deploy

🎨 How to Customize

You can easily customize this portfolio based on your needs.
Here are the main areas you may want to modify:

1. Update Your Name and Branding

Edit in:

src/components/Header.astro

src/pages/index.astro (Hero section)

Change the text:

Yoga Rizky Alkautsar


to your preferred name or branding.

2. Change Profile Image

Replace the file:

public/images/profile.jpg


with your own photo.
Keep the same filename, or update the image path inside index.astro.

3. Edit Hero Section Content

Modify:

src/pages/index.astro


Look for:

<h1 class="text-4xl md:text-5xl font-extrabold leading-tight mb-4">


Customize your headline, title, and description.

4. Edit About Section

Update text inside:

<section id="about" class="section">


Write your own story, professional summary, experience, etc.

5. Add or Update Skills

Skills are located in:

src/components/SkillBadge.astro


and rendered inside:

<section id="skills" class="section">


Add more badges:

<SkillBadge label="Docker" />
<SkillBadge label="Firebase" />

6. Customize Projects

Edit or add project cards in:

src/pages/index.astro


Each project uses the reusable component:

<ProjectCard
  title="Project Title"
  description="Short project summary."
  tags={['Astro', 'Tailwind']}
/>


You can add as many as you like.

7. Change Colors or Styling

Global styles:

src/styles/global.css


Section styles:

.section {
  @apply border border-gray-300 dark:border-gray-700 
         rounded-xl p-8 mb-10 shadow-sm bg-white 
         dark:bg-gray-900;
}


Modify Tailwind classes for custom look and feel.

8. Dark Mode Customization

Dark mode is controlled by:

<html class="dark"> toggle

localStorage.theme

Tailwind utilities (dark:bg-gray-900, etc.)

You can tweak color palettes directly in:

tailwind.config.mjs

📬 Contact

If you'd like to work together or get in touch:

📧 yogaralkautsar@gmail.com

🔗 LinkedIn (optional — add your link here)

📄 License

This project is open-source and can be used for learning purposes.