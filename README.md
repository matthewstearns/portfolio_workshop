# Welcome to a workshop on building a professional website!!! 💻

This repository is here to help you build your personal academic portfolio website. Ideally, by the end of this, you’ll have a professional webpage to showcase your research, publications, and achievements. Here we’ll use H**TML5 UP templates** to create a static website and deploy it to **GitHub Pages** for free!!! Note that you can also use **Jekyll** or **Hugo**, but I am most familiar with **HTML5 UP**, so we will be using that for the demonstration. A lot of the main content here is derived from a previous workshop done [here](https://github.com/manasvishal/website-building-u2grc). 

> 💡 *Feel free to choose the tools that best suit your skills and style. Each option has its own setup instructions.*

*Example*: My [webpage](https://matthewstearns.com) is built with [Dimension by HTML5 UP](https://html5up.net/uploads/demos/dimension/#); I just heavily edited the CSS, and HTML.  

---

### Table of Contents
1. [Prerequisites](#prerequisites) (Important - please read and make sure you have this set up correctly)
2. [Step 1: Fork and Clone the Repository](#step-1-fork-and-clone-the-repository) 
3. [Step 2: Choose a Website Template](#step-2-choose-a-website-template)
4. [Step 3: Set Up Your Website with HTML5 UP, Jekyll, or Hugo](#step-3-set-up-your-website-with-html5-up-jekyll-or-hugo)
5. [Step 4: Customize Your Website](#step-4-customize-your-website)
6. [Step 5: Deploy to GitHub Pages](#step-5-deploy-to-github-pages)
7. [Resources & Tips](#resources--tips)

---

### Prerequisites

There are a few things you’ll need before we start. 

- **GitHub Account:** Create one [here](https://github.com/) if you haven’t already. I also suggest that students sign up for the GitHub Student Developer Pack [here](https://education.github.com/pack).
- **Git**: [Download Git](https://git-scm.com/) to version control your website.
- **Code Editor**: Use [VS Code](https://code.visualstudio.com/), any code editor works, I'm just biased to VS Code... 
- **Local Server**: After installing VS Code, you will need to add the **Live Server** extension, which lets you launch a local development server with live reload for static & dynamic pages.

> *Optional but helpful*: Familiarity with basic HTML, CSS, Markdown, or command line usage.

---

### Step 1: Create Repository

There are two ways: 

#### Option A:

1. **Fork this repository** to create a copy under your GitHub account.
2. **Clone the repository** to your local machine. Open a terminal and run:

   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
   ```

   Now you’ll be able to work on your website locally!

#### Option B:
- Log in to your GitHub account, and once in your dashboard, click the create repository button. Just give it a name, something like `yourusername/website-portfolio` or whatever you feel is best. It is **VERY VERY VERY** important that we choose **public**.

---

### Step 2: Choose a Website Template

You have three main options for building your portfolio. Choose the one that best fits your needs:

1. **HTML5 UP Templates**: Simple, beautiful HTML templates. Good for custom HTML/CSS.
2. **Jekyll**: A popular static site generator that works well with Markdown and GitHub Pages.
3. **Hugo**: Another static site generator that’s fast and flexible, especially for complex sites.

> **Note**: HTML5 UP templates provide raw HTML/CSS files, while Jekyll and Hugo generate static pages using Markdown and themes.

---

### Step 3: Set Up Your Website with HTML5 UP, Jekyll, or Hugo


#### Option A: HTML5 UP Templates

1. Go to [HTML5 UP](https://html5up.net/) and browse the templates. 
2. Download the template you like, unzip it, and move its contents to your cloned repository.
3. Customize the HTML and CSS to reflect your personal information.

More resources:
- Standalone picocss templates : https://picocss.com/examples
- 100 templates : https://technext.github.io/100-template-bundle/


#### Option B: Jekyll

1. Install Jekyll by following [these instructions](https://jekyllrb.com/docs/installation/).
2. Create a new Jekyll site:

   ```bash
   jekyll new my-portfolio
   ```

3. Move your Jekyll site files into your cloned repository folder.
4. Start a local server to preview:

   ```bash
   bundle exec jekyll serve
   ```

5. Access the site at `http://localhost:4000` to see your progress.

More resources: 
- A comprehensive guide:  https://blog.christianposta.com/theme-setup/
- Another one:  https://www.pwills.com/posts/2017/12/20/website.html
- https://jamstackthemes.dev/theme/jekyll-professional-resume/
- https://jekyll-theme-minimal-resume.netlify.app/ https://github.com/murraco/jekyll-theme-minimal-resume
- https://jamstackthemes.dev/theme/jekyll-online-cv/
- https://ddbullfrog.github.io/resumecard/

#### Option C: Hugo

1. Install Hugo by following [these instructions](https://gohugo.io/getting-started/installing/).
2. Create a new Hugo site:

   ```bash
   hugo new site my-portfolio
   ```

3. Choose a theme from [Hugo Themes](https://themes.gohugo.io/) and install it.
4. Move your Hugo site files into your cloned repository folder.
5. Start a local server to preview:

   ```bash
   hugo server -D
   ```

6. Visit `http://localhost:1313` to view your website locally.
 
> **Note**: If using Jekyll or Hugo, you can probably view it directly in a code editor by right-clicking in VS Code and selecting Launch Server… This assumes you have the **Live Server** extension installed.
---

### Step 4: Customize Your Website

Now it’s time to make the website yours! Here are a few things you’ll want to update:

- **Personal Information**: Update your name, photos, bio, and contact information.
- **Research & Publications**: Add sections for your academic work, projects, and publications.
- **Social Media Links**: Add links to your LinkedIn, GitHub, Twitter, ORCiD, or Google Scholar profiles.

If you're using HTML5 UP, edit the HTML files directly. For Jekyll and Hugo, you’ll generally edit Markdown files in the `content` or `_posts` folders.

---

### Step 5: Deploy to GitHub Pages

Once you’re happy with your website, it’s time to deploy! This can be done a few ways...

#### Option A: Via Terminal 

Commit and push your changes to your GitHub repository:

   ```bash
   git add .
   git commit -m "Initial website setup"
   git push origin main
   ```

#### Option B: Uploading in browser 

1. Drag files into the repository and wait for them to upload. (You can only upload up to 100 files using the browser; otherwise, you would need to use GitHub Desktop for more than 100 files.)
2. After the files are uploaded, scroll down and commit the changes; it may take a few minutes to complete.

#### Now We Will Enable GitHub Pages

1. Go to your repository on GitHub.
   - Go to **Settings** at the top of the page.
   - Then navigate to **Pages** on the left.
   - Under Source, choose **GitHub Actions**.
   - Since we’re creating a static HTML website, click configure under that workflow.
   - We can leave this as the default, since everything we’re publishing is under the main branch. We can just leave it as is, then commit the changes.
2. Click the actions tab, and we can see it is deploying the static content, so we just have to wait a few…
3. After a few minutes, head back to settings and under pages, your site will be live at `https://yourusername.github.io/your-repo-name.`

More resources:
- https://www.arnoudplantinga.nl/post/getting-started/
- https://matteocourthoud.github.io/post/website/
- https://lakemper.eu/blog/getting-started-with-hugo-academic-and-github-pages/

> **Note**: If using Jekyll or Hugo, make sure your `_config.yml` or `config.toml` file is configured correctly for GitHub Pages.

#### Setting up Github Custom Domain

Place to buy domain: [namecheap](https://www.namecheap.com/). I am not affiliated in any way; it is just what I used… You can also get 1 year free with the GitHub Student Dev Pack mentioned in the prerequisites.

[Configuring a custom domain for your GitHub Pages site](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)

[Managing a custom domain for your GitHub Pages site](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site)

- **Youtube Tutorial for Hosting and Custom Domain Name**: https://www.youtube.com/watch?v=e5AwNU3Y2es&t=78s
---

### Resources & Tips

- **HTML5 UP Documentation**: [HTML5 UP](https://html5up.net/)
- **Jekyll Documentation**: [Jekyll Docs](https://jekyllrb.com/docs/)
- **Hugo Documentation**: [Hugo Docs](https://gohugo.io/documentation/)

For help, reach out via email: mstearns1@umassd.edu

---

### Final Words

Congratulations on setting up your academic portfolio website! 🎉 🎉 🎉 🎉 <br>
<br>
This website will help showcase your work, so you can refine it over time!! <br>
<br>
Have fun coding and playing around with the HTML and CSS files!!! Best of luck with your research, capstone and general schooling!<br>

---

*Last updated: February 2026*
