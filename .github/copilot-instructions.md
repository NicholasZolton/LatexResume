# Resume Writing Rules
- Never use periods at the end of the bullet points.
- Always use XYZ, CAR, or STAR format for bullet points
- Be specific and quantify accomplishments; if you don't have numbers, ask the user
- Be concise and avoid unnecessary words
- Never, ever hallucinate information for the resume; if you do not know, or need more info, ask the user
- Always refer to [EngineeringResumes Wiki](https://www.reddit.com/r/EngineeringResumes/wiki/index/) using fetch for best practices regarding resume writing
- If you use something from the EngineeringResumes wiki, cite it using Markdown links
- When finishing your response, always check for accuracy and completeness throughout the resume
- Ensure that all LaTeX correctly escapes the necessary special characters such as %, $, #, &, _, {, }, ~, ^, and \
- Note that all builds of the LaTeX will be executed automatically on save; if you want to ensure that the LaTeX built correctly, you can check the *.log file in the same directory as the .tex file
- NEVER run the LaTeX build yourself; always let the automated system handle it
- ALWAYS ensure that the resume is exactly 1 page long, unless the user explicitly requests otherwise
- If you need to remove content to keep the resume to 1 page, do your best to prioritize keeping the most relevant, recent, and impressive content
- When reviewing your work, pretend that you are a hiring manager at a top tech company, and ensure that the resume meets the highest standards
- Ensure that you keep in mind the "F" pattern of reading (meaning that humans tend to read in an "F" shape, focusing on the top and left side of the page more than the bottom and right side)
- ALWAYS optimize the resume for keywords. If the user provides a job description, pretend that you are the hiring manager for that job, and ensure that the resume is optimized for the keywords in that job description. Use info from `resume_info.json` to help with this
- Do not worry about the https:// in the URLs; this will be removed visually when the resume is compiled

# Resume Info
- Always ensure that any information about the user is stored in `resume_info.json`, so that if we remove it from the resume, we still have it for future reference
- DO NOT remove things from `resume_info.json` unless the user explicitly requests it. This should act as a database for all of the user's resume information, regardless of whether or not it is currently on the resume
- Context fields that are stored in `resume_info.json` should be used to help write better bullet points and improve the resume overall, but are not to be included on the resume itself unless the user explicitly requests it