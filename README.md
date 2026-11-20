# JAY MOGAL STUDIO — Admin Panel

Separate static admin dashboard for the JAY MOGAL STUDIO website. Built with HTML, CSS, JavaScript and Supabase Auth/PostgreSQL/Storage. No Vercel.

## GitHub Pages
Open repository Settings → Pages → Build and deployment → Deploy from a branch → select main / root, or configure GitHub Actions. The entry page is index.html.

## Sign in
Use the administrator account created in Supabase Auth. The account must have an active row in public.admin_profiles. This panel checks that authorization after every sign-in/session restore.

## Features
- Dashboard counts for projects, services, inquiries and reviews
- CRUD for services, portfolio projects and pricing
- Upload service images, portfolio cover images and studio logo to the public studio-media bucket
- Inquiry list with WhatsApp contact and contacted status
- Approve or reject customer reviews
- Edit business details, logo URL, hero/about/vision/mission content

## Configuration and security
config.js contains the Supabase project URL and public publishable key only. Never put a service-role key in this repository. Database RLS remains the enforcement layer; hiding the admin UI is not a substitute for RLS.
