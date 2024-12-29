# I-Hate-Sea-Shop

This repository contains the source code for the "I-Hate-Sea-Shop" website template store. The project is designed to showcase various website templates for e-commerce and other business purposes. Built with Next.js, it integrates with Sanity for content management and utilizes Tailwind CSS for a responsive and modern design.

## Project Overview

"I-Hate-Sea-Shop" is a simple, customizable e-commerce store template that leverages modern web technologies. It offers a clean, user-friendly interface for showcasing products, managing content via Sanity Studio, and deploying via Vercel for fast performance.

### Features:
- A responsive, customizable store template
- E-commerce functionality with product display and management
- Integrated with Sanity for content management
- Tailwind CSS for quick styling and layout management
- Simple setup and deployment with Vercel
- Easy-to-navigate interface for administrators and users
- Modern front-end stack with Next.js and TypeScript

---

## Table of Contents

- [Project Overview](#project-overview)
- [Important files and folders](#important-files-and-folders)
- [Configuration](#configuration)
  - [Step 1: Set up the environment](#step-1-set-up-the-environment)
  - [Step 2: Set up the project locally](#step-2-set-up-the-project-locally)
  - [Step 3: Run Next.js locally in development mode](#step-3-run-nextjs-locally-in-development-mode)
  - [Step 4: Deploy to production](#step-4-deploy-to-production)
- [Questions and Answers](#questions-and-answers)
- [Next Steps](#next-steps)

---

## Important Files and Folders

| File(s)                             | Description                                                       |
|-------------------------------------|-------------------------------------------------------------------|
| `sanity.config.ts`                  | Config file for Sanity Studio                                     |
| `sanity.cli.ts`                     | Config file for Sanity CLI                                        |
| `/pages/api/revalidate.ts`          | Serverless route for triggering Incremental Static Revalidation   |
| `/pages/api/draft.ts`              | Serverless route for triggering Draft mode                       |
| `/schemas`                          | Defines content types for Sanity Studio                           |
| `/lib/sanity`                       | Contains client-side configuration for interacting with Sanity   |
| `/components`                       | Reusable components for the store (e.g., product listings, cart)  |
| `/styles`                           | Tailwind CSS configuration and custom styles                      |
| `/public`                           | Public assets such as images and fonts                            |

---

## Configuration

### Step 1: Set up the environment
1. Deploy the project using the "Deploy with Vercel" button to set up both the store frontend and the Sanity backend.

### Step 2: Set up the project locally
1. Clone the repository from your GitHub account.
2. Run the following command to link the project with Vercel:
   ```bash
   npx vercel link
   ```
3. Pull the necessary environment variables:
   ```bash
   npx vercel env pull
   ```

### Step 3: Run Next.js locally in development mode
1. Install dependencies and run the development server:
   ```bash
   npm install && npm run dev
   ```
2. Your e-commerce store will be accessible at [http://localhost:3000](http://localhost:3000).

### Step 4: Deploy to production
1. To deploy changes to production, push your changes via Git:
   ```bash
   git add .
   git commit -m "Your commit message"
   git push
   ```
2. Alternatively, deploy via Vercel CLI:
   ```bash
   npx vercel --prod
   ```

---

## Questions and Answers

**It doesn't work! Where can I get help?**

- You can post your questions in the following communities:
  - GitHub Discussions for [Next.js](https://github.com/vercel/next.js/discussions)
  - [Sanity's GitHub Discussions](https://github.com/sanity-io/sanity/discussions)
  - [Sanity's Community Slack](https://slack.sanity.io/)

**How can I customize the store's appearance?**

- You can customize the store's layout and design by editing the Tailwind CSS configuration and modifying the components under `/components`.

**How can I manage content for the store?**

- Content can be managed directly via the Sanity Studio, which is integrated into the project. Access the studio via [http://localhost:3000/studio](http://localhost:3000/studio).

---

## Next Steps

- Join the [Slack community](https://slack.sanity.io/) to ask questions and get help.
- Learn how to customize the content structure and query your content.
- Explore [content modeling](https://www.sanity.io/docs/content-modeling) in Sanity.
