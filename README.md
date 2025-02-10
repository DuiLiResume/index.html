<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI Resume & Cover Letter Generator</title>
    <style>
        body { font-family: Arial, sans-serif; margin: 0; padding: 0; background-color: #f4f4f4; }
        .container { width: 60%; margin: 50px auto; background: white; padding: 20px; border-radius: 10px; box-shadow: 0 0 10px rgba(0,0,0,0.1); }
        h1 { text-align: center; }
        form { display: flex; flex-direction: column; gap: 15px; }
        label { font-weight: bold; }
        input, select, textarea { width: 100%; padding: 10px; border: 1px solid #ccc; border-radius: 5px; }
        button { padding: 10px; background: #007BFF; color: white; border: none; border-radius: 5px; cursor: pointer; }
        button:hover { background: #0056b3; }
    </style>
</head>
<body>
    <div class="container">
        <h1>Get Your AI-Generated Resume & Cover Letter Instantly</h1>
        <form action="/generate" method="POST">
            <label for="name">Full Name</label>
            <input type="text" id="name" name="name" required>
            
            <label for="email">Email</label>
            <input type="email" id="email" name="email" required>
            
            <label for="job">Job Title</label>
            <input type="text" id="job" name="job" required>
            
            <label for="industry">Industry</label>
            <input type="text" id="industry" name="industry" required>
            
            <label for="experience">Work Experience</label>
            <textarea id="experience" name="experience" placeholder="List your work experience, roles, and achievements"></textarea>
            
            <label for="skills">Skills & Competencies</label>
            <textarea id="skills" name="skills" placeholder="List your technical and soft skills"></textarea>
            
            <label for="education">Education</label>
            <textarea id="education" name="education" placeholder="Your degree, university, and year of graduation"></textarea>
            
            <label for="certifications">Certifications (Optional)</label>
            <textarea id="certifications" name="certifications" placeholder="List any professional certifications"></textarea>
            
            <label for="cover_letter">Do you need a cover letter?</label>
            <select id="cover_letter" name="cover_letter">
                <option value="yes">Yes</option>
                <option value="no">No</option>
            </select>
            
            <button type="submit">Generate My Resume</button>
        </form>
    </div>
</body>
</html>
