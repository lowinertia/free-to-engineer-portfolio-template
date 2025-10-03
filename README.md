# Portfolio For Current and Aspiring Engineers
How do you stand out and get hired in today's market? A strong portfolio demonstrates your technical skills and problem-solving in ways a resume just can't, giving you a clear advantage in your job search. Here, Lowinertia is prociding you all the tools you need to get started! Check out <a href="https://lowinertia.github.io/" target="_blank">the free portfolio demo here</a>. Follow along the instruction below to setup and personalize your page. 

## There are two option:
### 1. Self-host on github : free-to-engineer template

**NOTE:** If you are familiar with Jekyll and Github workflows, the initial setup would take about 30 minutes. If you are not familiar with Github and config and markdown files, this could be challenging and may take more than an hour.

### 2. Free No-code Portfolio Builder at [lowinertia.com](https://lowinertia.com)

Portfolio builder made for engineers with 2 min onboarding with smart resume import. Vist [lowinertia.com](https://lowinertia.com) to find out more 


# free-to-engineer-portflio-template instructions

### 1. Setting Up Your Page on GitHub (5 min)
- [Getting Started](#getting-started)
- [Setup GitHub Account](#setup-github-account)
- [Use the template](#Use-the-template)


### 2. Personalizing Your Portfolio (10+ min)
- [Set Up Your Profile](#set-up-your-profile)
  - [Open `_config.yml`](#open-_configyml)
- [Adding Projects](#adding-projects)
  - [Creating a Markdown File in GitHub](#creating-a-markdown-file-in-github)

### 3. Understanding Markdown for Your Project Page
- [YAML Frontmatter](#yaml-frontmatter)
- [Adding Contents](#adding-contents)
  - [Section Title](#section-title)
  - [Sub-Section Title](#sub-section-title)
  - [Adding a New Line](#adding-a-new-line)
  - [Adding a Horizontal Line](#adding-a-horizontal-line)
  - [Embedding Images](#embedding-images)
  - [Embedding YouTube Video](#embedding-youtube-video)
  - [Adding Bold Text](#adding-bold-text)
  - [Adding Italic Text](#adding-italic-text)
  - [Adding Ordered List](#adding-ordered-list)
  - [Adding Unordered List](#adding-unordered-list)
  - [Adding Code Block](#adding-code-block)
  - [Adding External Links](#adding-external-links)
  - [Adding Block Quote](#adding-block-quote)
  - [Adding Table](#adding-table)




## Getting Started:

### Setup GitHub Account
1. **Visit GitHub**: If you don't have an account, go to [GitHub](https://github.com/) and sign up.
2. **Create an Account**: Fill out the registration form with your preferred username, email, and password.
3. **Verify Your Email**: Check your email to verify your account.

### Use the template
1. **Navigate to FreeToEngineer Repository**: Go to the repository where this portfolio template is [hosted](https://github.com/leea12/freeToEngineer)
2. **Use the template**: Click the "Use this template" button at the top right of the page. Then, choose create a new repository. This creates a copy under your GitHub account. If you can also click on the "star", it will help the template to get visibility to many others!

   ![GitHub Use Template](/assets/readme/github-use-template.png)

3. **[IMPORTANT] Name the repository**: in the "Repository name" field, type in `{your github id}.github.io`.This is also the url of your portfolio. You can use your custom domain as well. (change in the setting later)

   ![GitHub Use Template](/assets/readme/github-name-repository.png)
4. Click "Create repository"
5. **That's it!** Now, you have a portfolio webiste @ [your id].github.io. You may have to wait for up to 1 minute for github to finish building.
6. **[Good to know]** you can see the status of your website by going to settings - pages.
   ![GitHub Use Template](/assets/readme/github-pages.png)

## Set up Your profile

### Open `_config.yml`
This file contains the configuration settings for your site. Here's what you might want to change: 
After you are done. just click **"commit chages"** to apply. Give a minute or so for github to build your website.


- **Site Title**: Change the `title:` this is what shows up in the tab of the browser on your site
- **Name**: Change the `name:` your name will show up as seen above
- **Description**: Update the `description:` with a brief overview of your highlights and qualification
- **profile_image**: place your profile image in assets/profile folder and update the directory
- **Resume-url**: You can either link to externally stored pdf (ex. google drive) or save the pdf under assets/pdf/ folder and enter the directory  

![GitHub Use Template](/assets/readme/main-page.png)

<br>

- **External Links**: link your external accounts (linkedin, github, stackoverflow, medium, etc)
![GitHub Use Template](/assets/readme/external-link.png) 
Only the icons for the accounts that you enter will appear.
*Example*:
  ```yaml
    external-links:    # input only your own url slug. The icons with missing entries will not appear.
      linkedin: johndoe1       # https://www.linkedin.com/in/{your url slug} 
      github: johndoe1         # https://github.com/{your url slug} 
      stackoverflow: johndoe1  # https://stackoverflow.com/users/{your url slug}
  ```


- **Skills**: you can list your skills by category. It will  show up like below. Be careful with the identation.
![GitHub Use Template](/assets/readme/skills.png) 
  *Example*:
    ```yaml
      skills:
        - category: 3D Modeling
          tools:
          - Onshape
          - Solidworks
          - Creo
          - Fusion 360 
        
        - category: Prototyping
          tools:
          - SLA
          - CNC
          - FDM
          - SLS
          - DMLS
          - PolyJet Printing
          - Vacuum Casting
    ```
- **Contact Form**: you can set up the contact form to send the response to your email using [formspree](https://formspree.io/). You just need to sign up and create a new form. Then, add the 8-digit endpoint key!
 
  ![formspreeimage](/assets/readme/formspree.png)

  ```yaml
  formspree-key:   https://formspree.io/f/{8-digit key}
  ```

- **(optional)** you chan change your color theme by inputting color hex code for a few variables. Feel free to be creative!
  ```yaml
  colors: # this is the basic theme
    text: "##1a1c20"
    border: "#ddd"
    link: "#4a76ee"
    highlight: "#0c0cf2"
    background: "#ffffff"
    light_background: "#f3f5fb"
  ```
  There is a few suggested themes in `_config.yml`
  - **mint green**
  ![GitHub Use Template](/assets/readme/mint-green.png) 
  - **lemon**
  ![GitHub Use Template](/assets/readme/lemon.png) 
  - **cotton-candy**
  ![GitHub Use Template](/assets/readme/cotton-candy.png) 

## Adding projects
For each project, you need to create a markdown file within _projects folder. I recommend created a folder for each project so that it is easy to organize image files that you may want to add. To get started, follow the below steps.

#### Creating a markdown file in Github
1. Go to **_project** folder. Make sure you are in the correct level.
![GitHub Use Template](/assets/readme/go-to-project-directory.png) 
2. In the right side of the screen, click add file - create new file.  
![GitHub Use Template](/assets/readme/create-new-file.png) 
3. in the available field, enter the name of the folder: **{your-project-name}** then hit "/". This will create a folder for the project.   
![GitHub Use Template](/assets/readme/enter-folder-name.png) 
4. create a markdown file by entering index.md.   
![GitHub Use Template](/assets/readme/index-md.png) 
5. In the text field paste the below "front-matter" template and fill out the title, description, skills, and name of the main project image that you want to use. This is the summary of the project that will be used to display the project in the main page. **Be careful** not to leave any space before the front matter deliminators "---". It causes syntax error, and  your page will not be built.

    ```md
    ---
    layout: post
    title: project title
    description:  short description of the project
    skills: 
    - skill 1
    - skill 2
    main-image: /project.webp 
    ---
    ```
6. then click **Submit changes** to create the file.
7. Upload your image in the same folder by clicking **Add file - upload files**.
  
![GitHub Use Template](/assets/readme/create-new-file.png) 

8. Drag your image file, then click **commit changes**.
    
![GitHub Use Template](/assets/readme/upload-files.png) 

9. Allow a minute or so for the build. It will create a project section that looks like this below.
![GitHub Use Template](/assets/readme/project-section.png) 

### Understanding markdown file your project page
If you want to add addtional details, you can go back to the index.md file and add more contents below the front matter. It will be helpful if you become familiarized with markdown syntax. If you are interested in learning, see [markdown guide](https://www.markdownguide.org/cheat-sheet/). I set up a couple styling to allow you to embed multiple images and video easily and become responsive for mobile view. See the [demo](https://leea12.github.io/)) project. You can also add code blocks, blockquote, and tables. 

#### YAML frontmatter
YAML frontmatter gets pulled by the site to fill contents for the summary section of your project which gets displayed in the main index page and top section of the project page. 

```markdown
---
layout: post
title: Super Heavy Booster Catch (Demo Only)
description:  (I have never been employed by / affiliated with SpaceX. This is for demo use only) 
    Developing the Super Heavy booster catch project involves designing a robust launch tower with "chopstick" arms, advanced control systems for precise booster alignment, and integrating sophisticated software for real-time trajectory adjustments and structural engineering to handle immense forces.
skills: 
  - Structural analysis
  - Aerodynamic design
  - Propulsion system integration
  - Control Algorithem 
  - Welding
  - Metal forming
  - Thermal simulation

main-image: /project2.jpg
---
```
#### Adding contents
use "## (title)" as the title of each section
## Section title
```markdown
## section title
```

### sub-section title
Use this to have subsection if needed
```markdown
### sub-section title
```

#### Adding a new line
you can add 2 spaces "  " or <br> to start a new line
```markdown
<br>
```

#### Adding a horizontal line
you can add a horizontal line to separate fields by using "---"
```markdown
---
```

#### Embedding images 
Add images using the following format. You can put multiple images in a single row by putting in multiple entries for "images=". You can also overide the size of the all images in the single row setting the height in pixel.
{% include image-gallery.html images="{image1 path}, {image2 path}" height="400"%}

```markdown
{% include image-gallery.html images="project2.jpg" height="400" %}
```
#### Embedding youtube video
Add youtube video using the following format
{% include youtube-video.html id="{11-digit id}" autoplay= "false"%}
```markdown
{% include youtube-video.html id="{11-digit id}" autoplay= "false"%}
```
This is where you get the 11-digit id  

![image](https://github.com/user-attachments/assets/4ffc509a-9e22-40bc-b503-421443ab2b66)

#### Adding bold text
add bold text by wrapping with "**"
```markdown
this is how you input **bold text**
```

#### Adding italic text
add italic text by wrapping with "*"
```markdown
Italicized text is the *cat's meow*.
```

### adding underline
underline is not supported in markdown, but you can still use html within markdown
```
<u>This text is underlined</u>
```

#### Adding ordered list
```markdown
1. First item
2. Second item
3. Third item
4. Fourth item
```
1. First item
2. Second item
3. Third item
4. Fourth item

#### Adding unordered list
```markdown
- First item
- Second item
- Third item
- Fourth item
```
- First item
- Second item
- Third item
- Fourth item

#### Adding code block
To add a code block wrap your script with ```. Adding the language after ''' will activate sytax highlighting.
![image](https://github.com/user-attachments/assets/8b8a6c6a-1599-4b03-bcc3-b087bc0f5c49)

```python
def start()
  print("time to start!")
```

#### Adding external links
to add extra links, wrap the text in "[ ]" then add the add the hyperlink wrappted by "( )"
```markdown
[Wikipedia](https://en.wikipedia.org)
```
#### Adding block quote
To add a blockquote add ">" at the beginning of the text
```markdown
> A blockquote would look great if you need to highlight something
```
> A blockquote would look great if you need to highlight something

#### Adding table
To add a table, use the following format
```markdown
| Header 1 | Header 2 |
|----------|----------|
| Row 1, Col 1 | Row 1, Col 2 |
| Row 2, Col 1 | Row 2, Col 2 |
```
| Header 1 | Header 2 |
|----------|----------|
| Row 1, Col 1 | Row 1, Col 2 |
| Row 2, Col 1 | Row 2, Col 2 |

** make sure to leave a line betwen the table and the header

