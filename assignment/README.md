# NiuHome

## Project Overview
NiuHome is a web platform that showcases premium properties, providing users with a curated selection of homes tailored to various needs and lifestyles. This project is deployed on Netlify with automatic deployment configured via GitHub Actions, allowing seamless updates directly from the main GitHub branch.

## Deployment Instructions

### 1. Netlify Setup and GitHub Integration

#### Step 1: Create a Netlify Account
1. Go to [Netlify](https://www.netlify.com/) and sign up for a free account.
![foto-1](../Assets/1.%20homepage-signup.png)
![foto-2](../Assets/2.%20signup-page.png)

2. Once registered, go to your Netlify dashboard.

#### Step 2: Connect GitHub Repository to Netlify
1. In the Netlify dashboard, click on **"Import from Git"**.
![foto-3](../Assets/3.%20netlify-dashboard.png)

2. Choose **GitHub** as the deployment provider and authorize Netlify to access your GitHub account.
![foto-3](../Assets/4.%20choose-github.png)

3. Select the repository containing your NiuHome project.
4. Configure the **Build and Deploy settings**:
   - **Branch to Deploy**: Choose the main branch (or your preferred branch for deployment).
   - **Publish Directory**: Specify the directory where your main files are located (e.g., `assignment` for this project).

5. Click **Deploy Site**. Netlify will automatically deploy your site from the GitHub repository.

#### Step 3: Auto Deployment Setup on GitHub
- Any push or pull request merged into the main branch will automatically trigger a deployment on Netlify. This is managed through GitHub Actions and Netlify’s integration with the repository, ensuring your site stays up-to-date.

### 2. Custom Domain and DNS Setup

#### Step 1: Purchase a Custom Domain
1. Buy a custom domain from a registrar like [Niagahoster](https://www.niagahoster.co.id/), [Namecheap](https://www.namecheap.com/), or other providers. RevoU suggests purchasing a `.site` domain to stay within budget constraints.

#### Step 2: Configure DNS on Netlify
1. In your Netlify dashboard, navigate to **Domain Settings** and select **Add Custom Domain**.
2. Enter the purchased domain name and follow the instructions to verify domain ownership.

#### Step 3: Update DNS Settings with Registrar
1. Go to your domain registrar's dashboard and access the **DNS settings**.
2. Update the DNS records with the values provided by Netlify:
   - **CNAME Record**: Point your domain (e.g., `www.yourdomain.com`) to Netlify’s default domain for your site.
   - **A Record**: (If required) Set up an A record pointing your domain to Netlify’s IP addresses.

3. Save the changes. DNS propagation can take a few minutes to a few hours. Once completed, your site will be accessible via your custom domain.

## Project Structure
