# Portfolio Website with React, Tailwind CSS, and Sanity

This is a modern, responsive portfolio website built with React and styled using Tailwind CSS. It features a content management system powered by Sanity.io for easy content updates.

## Features

- **Modern UI Design** - Clean and professional interface with smooth animations
- **Responsive** - Mobile-first design ensures compatibility with all devices
- **Dynamic Content** - All content managed through Sanity CMS
- **Portfolio Showcase** - Filterable projects section to display your work
- **Skills & Experience** - Visual representation of your abilities and work history
- **Testimonials** - Client feedback carousel with admin and user submission options
- **Contact Form** - Interactive form with email integration
- **SEO Optimized** - Best practices implemented for search engine visibility

## Pages/Sections

1. **Hero Section** - Engaging introduction
2. **About** - Information about you and your services
3. **Work** - Portfolio projects with filtering capability
4. **Skills** - Technical abilities with visual indicators
5. **Experience** - Work history timeline
6. **Testimonials** - Client reviews slider
7. **Footer/Contact** - Contact form with social links

## Technical Stack

- **Frontend**: React.js
- **Styling**: Tailwind CSS
- **CMS**: Sanity.io
- **Animations**: Framer Motion
- **Icons**: React Icons
- **Form Handling**: Integrated with Sanity

## Sanity Integration

The website uses Sanity.io as a headless CMS to manage all content including:

- Portfolio projects
- Skills and experience
- Testimonials
- About information
- Contact details

### Sanity Schemas

The project includes the following schemas:

- **works** - Portfolio projects
- **testimonials** - Client feedback
- **brands** - Company logos
- **abouts** - About section content
- **skills** - Technical abilities
- **experiences** - Work history
- **contact** - Contact form submissions

## Testimonial Submission Feature

A special feature of this site is the ability for users to submit testimonials directly through the contact form:

1. Users can toggle between regular contact messages and testimonial submissions
2. When submitting a testimonial, additional fields appear (company, photo upload)
3. Upon submission, testimonials are stored in Sanity and can be reviewed before publishing
4. Published testimonials appear in the testimonials carousel

## Getting Started

### Prerequisites

- Node.js (v14 or later)
- npm or yarn
- Sanity account

### Installation

1. Clone the repository
   ```
   git clone https://github.com/yourusername/your-portfolio.git
   cd your-portfolio
   ```

2. Install frontend dependencies
   ```
   npm install
   # or
   yarn install
   ```

3. Install Sanity CLI (if not already installed)
   ```
   npm install -g @sanity/cli
   # or
   yarn global add @sanity/cli
   ```

4. Initialize Sanity studio (in a backend folder)
   ```
   cd backend
   sanity init
   ```

5. Import the provided schemas into your Sanity studio

### Environment Setup

Create a `.env` file in the frontend root with the following variables:
```
REACT_APP_SANITY_PROJECT_ID=your_sanity_project_id
REACT_APP_SANITY_TOKEN=your_sanity_token
```

### Running the Development Server

1. Start the frontend
   ```
   npm start
   # or
   yarn start
   ```

2. Start the Sanity studio (in the backend directory)
   ```
   sanity start
   ```

## Deployment

### Frontend Deployment

The frontend can be deployed to platforms like Vercel, Netlify, or GitHub Pages:

```
npm run build
# or
yarn build
```

Then follow the platform-specific deployment instructions.

### Sanity Studio Deployment

Deploy the Sanity studio:

```
cd backend
sanity deploy
```

## Customization

### Tailwind Configuration

- Modify `tailwind.config.js` to customize colors, fonts, and other design tokens
- Update the global styles in `src/index.css`

### Component Styling

- All components use Tailwind utility classes for styling
- Layout components in the `src/wrapper` directory handle common layout patterns

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Design inspiration from modern portfolio trends
- Sanity.io for the flexible content management system
- Tailwind CSS for the utility-first styling approach
