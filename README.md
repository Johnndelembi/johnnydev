# JohnnyDev Portfolio Website

A responsive personal portfolio website built with Tailwind CSS, showcasing skills, projects, and contact information.

![JohnnyDev Portfolio](build/img/hero-image.png)

## Description

This is a personal portfolio website for John, a FullStack Developer, Data Scientist, and DevOps Engineer. The website showcases John's skills, projects, and provides contact information for potential clients or employers.

## Technologies Used

- HTML5
- [Tailwind CSS](https://tailwindcss.com/) (v3.4.9)
- Node.js (for build process)
- npm (for package management)
- [EmailJS](https://www.emailjs.com/) (for contact form functionality)

## Project Structure

```
johnnydev/
├── build/                  # Production-ready files
│   ├── css/                # Compiled CSS
│   │   └── style.css       # Main stylesheet (compiled from input.css)
│   ├── img/                # Image assets
│   └── index.html          # Main HTML file
├── src/                    # Source files
│   └── input.css           # Tailwind CSS source file
├── package.json            # Project dependencies and scripts
├── package-lock.json       # Locked versions of dependencies
├── tailwind.config.js      # Tailwind CSS configuration
└── README.md               # Project documentation
```

## Features

- **Responsive Design**: Adapts to different screen sizes (mobile, tablet, desktop)
- **Modern UI**: Clean and professional design using Tailwind CSS
- **Functional Contact Form**: Powered by EmailJS to send messages without a backend server
- **Sections**:
  - Hero section with introduction
  - Skills showcase
  - Project portfolio with descriptions and demo links
  - Contact section with working form

## Skills Showcased

- Bootstrap & Tailwind CSS
- Git
- DevOps
- Django Framework
- Data Analytics
- Machine Learning
- Neural Network Architectures
- Generative AI & Conversational AI

## Projects Featured

1. **AI Chatbot**: Conversational AI capable of human-like interactions
2. **YouTube Downloader ("Freebie")**: Tool for downloading videos and audio in high quality
3. **University Social Network**: Platform for student community interactions
4. **Salary Predictor Model**: Machine learning model for salary prediction
5. **African AI Insights Platform**: AI-powered platform for business intelligence and real-time interactive analytics
6. **ML Pipeline**: System for predicting oil, gas, and water prices

## Setup and Installation

1. Clone the repository:
   ```
   git clone <repository-url>
   cd johnnydev
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Build the CSS:
   ```
   npm run build
   ```

4. For development with auto-refresh:
   ```
   npm run watch
   ```

5. To format HTML files:
   ```
   npm run prettier
   ```

## Development

The project uses Tailwind CSS for styling. The main source file is `src/input.css`, which is compiled to `build/css/style.css` using the Tailwind CLI.

### Available Scripts

- `npm run build`: Builds the CSS file
- `npm run watch`: Watches for changes and rebuilds CSS
- `npm run prettier`: Formats HTML files using Prettier

## Customization

To customize the website:

1. Edit the HTML in `build/index.html`
2. Modify Tailwind configuration in `tailwind.config.js`
3. Add custom styles to `src/input.css` if needed
4. Run `npm run build` to compile the CSS

## Contact Form Configuration

The website uses EmailJS to handle the contact form submissions without a backend server. To configure EmailJS:

1. Sign up for a free account at [EmailJS](https://www.emailjs.com/)
2. Create an email service (e.g., Gmail, Outlook, etc.)
3. Create an email template with the following variables:
   - `user_name`: Sender's name
   - `user_email`: Sender's email
   - `message`: Message content
4. Update the EmailJS configuration in `build/index.html`:
   - Locate the `emailjsConfig` object at the top of the file (around line 14)
   - Replace the placeholder values with your actual credentials:
     ```javascript
     const emailjsConfig = {
         publicKey: 'YOUR_PUBLIC_KEY',      // Your EmailJS Public Key
         serviceId: 'YOUR_SERVICE_ID',      // Your EmailJS Service ID
         templateId: 'YOUR_TEMPLATE_ID'     // Your EmailJS Template ID
     };
     ```

The contact form includes validation and displays success/error messages after submission.

## Contact

For inquiries, contact John at:
- Email: [williamjohnie61@gmail.com](mailto:williamjohnie61@gmail.com)
- Whatsapp: Available through the website

## License

[Add license information here]
