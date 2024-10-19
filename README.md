# Internshala_Automation
Internshala Automation Script automates the internship application process on the Internshala platform. Using Puppeteer, it logs in, fills out forms, and submits applications, saving time for users. Easily customize application data through a data.js file.
Here's the complete `README.md` file template formatted for easy copying and pasting into your GitHub repository:

```markdown
# Internshala Automation Script

### Overview
This project automates the process of applying for internships on the Internshala website. It eliminates the repetitive task of filling out the same details multiple times by using Puppeteer, a Node.js library, to automatically log in and submit forms on behalf of the user.

### Motivation
Internshala requires students to manually fill in a set of repetitive details for each internship application, which can be time-consuming. This script was created to automate the process, saving time and ensuring accuracy.

### Features
- **Automated Login**: Logs in to the Internshala website using stored credentials.
- **Automated Form Filling**: Automatically fills out fields like education details, training, and work samples.
- **Multi-Internship Application**: Automatically applies to multiple internships by navigating through the available internships.
- **Customizable Data**: User-specific data like college, degree, work experience, and more are customizable via a `data.js` file.

---

### Prerequisites
To run this script, you'll need to have the following installed:

1. **Node.js** (v14 or higher) - [Download Node.js](https://nodejs.org/)
2. **Puppeteer** - Puppeteer is a Node library that provides a high-level API to control Chrome or Chromium over the DevTools Protocol.

---

### Setup

#### 1. Clone the repository
```bash
git clone https://github.com/your-username/internshala-automation.git
cd internshala-automation
```

#### 2. Install dependencies
```bash
npm install
```

#### 3. Create a `secret.js` file
Create a file named `secret.js` in the root directory to store your Internshala login credentials.

```js
module.exports = {
    id: "your-email@example.com", // Enter your Internshala email ID
    pass: "your-password"         // Enter your Internshala password
}
```

#### 4. Customize the `data.js` file
This file contains the details required to fill out the application. You can modify the content to suit your personal details.

```js
module.exports = [
    {
        "College": "Your College Name",
        "Degree": "Your Degree Name",
        "Stream": "Your Stream",
        "Percentage": "Your Percentage",
        "Training": "Your Training Name",
        "Organization": "Training Organization",
        "description": "Description of the training or work sample",
        "link": "Your portfolio or work sample link",
        "hiringReason": "Why should we hire you?",
        "availability": "Your availability for the internship",
        "rating": "Your rating of the internship"
    }
];
```

---

### Running the Script

1. Open your terminal or command prompt.
2. Navigate to the project directory.
3. Run the following command to start the script:

```bash
node index.js
```

The script will launch a browser window and start interacting with Internshala, filling out forms, and submitting internship applications automatically.

---

### How It Works
- **Login**: The script first logs you in using the email and password from the `secret.js` file.
- **Profile Navigation**: It navigates to your profile and selects the appropriate sections (education, training, etc.) to fill.
- **Internship Application**: It will navigate through the available internships and apply automatically.

---

### Future Improvements
- Add error handling to ensure smoother execution in case of network issues.
- Allow dynamic selection of internships instead of hardcoding the application URLs.
- Implement headless mode for faster execution without browser visibility.

---

---

### Contribution
Feel free to open issues or submit pull requests if you have any improvements or suggestions.
```

You can replace `your-username` in the clone command with your GitHub username. Once you've pasted this into your `README.md` file, make any necessary adjustments to fit your project specifics.
