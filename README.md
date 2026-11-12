# ResumeCraft Pro | Advanced Resume & CV Builder

A modern, responsive, and feature-rich **Resume and CV Builder** built with **HTML5, CSS3, and JavaScript**.

ResumeCraft Pro helps job seekers, students, and professionals create attractive, ATS-friendly resumes using professional templates, guided writing suggestions, live previews, and an interactive dashboard.

The application includes an ATS readiness checker, job description keyword comparison, and a smart writing assistant to help users improve their resumes.

**No backend, database, registration, or API key required.**

## Features

### 1. Professional Dashboard

- View and manage saved resumes
- Monitor resume completion scores
- Create multiple CVs for different job applications
- Access recently edited resumes
- Duplicate, edit, and delete resumes

### 2. Advanced Resume Builder

- Add personal information and contact details
- Write a professional summary
- Add work experience and responsibilities
- Include education and qualifications
- Add technical and professional skills
- Showcase personal and professional projects
- Add certifications and achievements
- View resume changes instantly

### 3. ATS Readiness Checker

- Analyze resume completeness
- Generate a readiness score out of 100
- Identify missing or incomplete sections
- Highlight opportunities to improve resume content
- Check for measurable achievements
- Provide recommendations for improvement

**Note:** The ATS score is an educational estimate, not an official score from an applicant tracking system. No tool can guarantee acceptance by an employer's ATS.

### 4. Job Description Keyword Checker

- Paste a job description
- Compare job requirements against resume content
- Identify matching keywords
- Highlight potential missing keywords
- Help users tailor resumes for specific positions

### 5. Smart Resume Writing Assistant

- Improve descriptions of job responsibilities
- Generate three alternative bullet-point drafts
- Suggest clearer professional wording
- Help organize existing experience and achievements
- Improve readability and presentation

The writing assistant uses built-in templates and rules. It does not require an external AI API and does not invent work experience or achievements.

### 6. Professional Resume Templates

Three customizable resume layouts are available:

- **Classic ATS:** A simple, readable layout designed with ATS compatibility in mind
- **Modern Professional:** A contemporary resume layout
- **Compact:** A space-efficient layout for presenting experience concisely

Users can also customize the resume accent color.

### 7. PDF Export

- Preview resumes before downloading
- Generate print-ready layouts
- Export resumes using the browser's Save as PDF feature
- Create professional PDF documents suitable for job applications

### 8. Local Storage and Backup

- Automatically save resume information
- Create and manage multiple resume versions
- Export saved data as JSON backups
- Restore previously exported resume data
- Continue editing resumes without creating an account

### 9. Responsive Design

- Modern dashboard interface
- Mobile-friendly layouts
- Responsive forms and navigation
- Clean typography and interactive controls
- Supports desktop, tablet, and mobile browsers

## Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Application structure |
| CSS3 | Styling, layout, and responsiveness |
| JavaScript | Resume creation and application functionality |
| Local Storage | Saving resumes in the browser |
| JSON | Data backup and restoration |
| Browser Print API | PDF export |
| Node.js | Optional automated testing |

## Installation and Setup in VS Code

### Step 1: Download the Project

1. Click the green **Code** button on this GitHub repository.
2. Select **Download ZIP**.
3. Extract the downloaded ZIP file.
4. Open Visual Studio Code.
5. Select **File > Open Folder**.
6. Choose the extracted `resumecraft-pro` folder.

### Step 2: Run the Application

No installation is required.

1. Open the extracted project folder.
2. Locate `index.html`.
3. Double-click `index.html` to open the application in your browser.
4. The ResumeCraft Pro dashboard will appear.
5. Click **New resume** to begin creating your CV.

The application does not require Python, Node.js, or a backend server to run.

### Alternative: Run Using Live Server

1. Open Visual Studio Code.
2. Navigate to the Extensions panel.
3. Search for **Live Server** by Ritwick Dey.
4. Install the extension.
5. Right-click `index.html`.
6. Select **Open with Live Server**.

The application will typically open at:

`http://127.0.0.1:5500`

### Alternative: Run with Python

If Python is installed, open the VS Code terminal and execute:

```bash
python -m http.server 8000
```

Then visit:

`http://localhost:8000`

## How to Use

### Create a New Resume

1. Launch ResumeCraft Pro.
2. Click **New resume** on the dashboard.
3. Enter your name, professional title, and contact details.
4. Add a professional summary.
5. Enter your work experience and achievements.
6. Add education, skills, projects, and certifications.
7. Select a resume template.
8. Customize the accent color.
9. Review the live resume preview.

Resume information is automatically saved in your browser.

### Check ATS Readiness

1. Open the **ATS checker**.
2. Review your resume's readiness score.
3. Identify missing or incomplete sections.
4. Follow the improvement recommendations.
5. Return to the resume editor to make changes.

### Compare a Resume with a Job Description

1. Open the ATS checker.
2. Copy a job description from a vacancy.
3. Paste the description into the comparison field.
4. Review matching keywords and potential gaps.
5. Update your resume using truthful, relevant experience.

### Use the Writing Assistant

1. Open the **Writing assistant**.
2. Enter your actual job responsibilities.
3. Add relevant tools and measurable results where available.
4. Generate improved bullet-point suggestions.
5. Review the suggestions for accuracy.
6. Copy suitable wording into your resume.

### Export Your Resume as PDF

1. Open the resume you want to export.
2. Review the live preview.
3. Click **Save as PDF**.
4. Select **Save as PDF** in your browser's print dialog.
5. Disable browser headers and footers for a cleaner document.
6. Save the PDF to your computer.

### Backup and Restore Resumes

To back up your resumes:

1. Open the application's backup controls.
2. Select the JSON export option.
3. Save the downloaded backup file.

To restore resumes:

1. Open the backup import option.
2. Select your previously exported JSON file.
3. Restore the saved resume information.

## Project Structure

```text
resumecraft-pro/
├── index.html
├── assets/
│   ├── app.js
│   ├── core.js
│   └── styles.css
├── tests/
│   └── core.test.cjs
├── .gitignore
├── LICENSE
└── README.md
```

### File Descriptions

- **index.html:** Main application interface, dashboard, and navigation
- **assets/styles.css:** Responsive styling, resume templates, and print layouts
- **assets/app.js:** User interactions, resume management, storage, and PDF printing
- **assets/core.js:** ATS scoring, keyword comparison, resume models, and writing suggestions
- **tests/core.test.cjs:** Automated tests for the core application logic
- **.gitignore:** Excludes unnecessary development files
- **LICENSE:** MIT License information

## Running Automated Tests

Node.js version 18 or newer is required only for automated testing.

Open the VS Code terminal and run:

```bash
node --test tests/core.test.cjs
```

The automated tests cover:

- Resume data creation
- ATS checklist scoring
- Job description keyword matching
- Writing assistant suggestions
- HTML escaping
- Backup data validation

Node.js is not required to run the actual web application.

## Deploying on GitHub Pages

ResumeCraft Pro can be hosted for free using GitHub Pages.

### Deployment Steps

1. Create a public GitHub repository named `resumecraft-pro`.
2. Upload all extracted project files and folders.
3. Ensure `index.html` is located in the repository's root directory.
4. Open the repository's **Settings**.
5. Select **Pages**.
6. Under **Build and deployment**, choose **Deploy from a branch**.
7. Select the `main` branch.
8. Select the `/(root)` directory.
9. Click **Save**.

Once deployment finishes, GitHub Pages will provide your live application URL.

No backend hosting or database configuration is required.

## Privacy and Data Storage

- Resume data is processed locally in the browser.
- Information is stored using Local Storage.
- No resume information is automatically uploaded to an external server.
- Resume data does not synchronize between devices.
- Clearing browser storage may remove saved resumes.
- JSON backups can be used to restore saved information.
- Browser Local Storage is not encrypted.
- Avoid saving sensitive personal information on shared computers.

## Important Limitations

- ATS scoring is a simplified readiness checklist, not a guarantee of passing an employer's screening system.
- Job description comparison uses keyword matching and may not recognize every relevant synonym.
- The writing assistant uses local templates rather than a generative AI model.
- Writing suggestions should be reviewed before being added to a resume.
- The application does not verify employment history or qualifications.
- Resume PDF export depends on the browser's print functionality.
- Local Storage does not provide cloud synchronization or multi-user accounts.
- Users should verify the accuracy and formatting of their resumes before submitting job applications.

## Browser Compatibility

ResumeCraft Pro is designed for modern browsers, including:

- Google Chrome
- Microsoft Edge
- Mozilla Firefox
- Safari

## Contributing

Contributions, feature requests, and suggestions are welcome.

1. Fork this repository.
2. Create a new branch.
3. Make your changes.
4. Test your changes.
5. Submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

You are free to use, modify, and distribute the source code according to the license terms.
