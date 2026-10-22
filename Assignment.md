 Assignment 6.5 — Profile Card / Product Card Mini-Project.1. HTML file — Assignment-6.5.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Assignment 6.5 - Profile Card</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <main class="profile-container">
        <div class="profile-card">

            <span class="profile-badge">Available for Work</span>

            <div class="profile-image-container">
                <img
                    src="https://i.pravatar.cc/300?img=12"
                    alt="Profile portrait of Alex Morgan"
                    class="profile-image"
                >
            </div>

            <h1 class="profile-name">Alex Morgan</h1>
            <h2 class="profile-role">Frontend Developer</h2>

            <p class="profile-description">
                Passionate developer who creates modern, responsive,
                and user-friendly websites using the latest web technologies.
            </p>

            <div class="skills-section">
                <h3 class="skills-heading">My Skills</h3>

                <div class="skills-list">
                    <span class="skill-tag">HTML</span>
                    <span class="skill-tag">CSS</span>
                    <span class="skill-tag">JavaScript</span>
                    <span class="skill-tag">React</span>
                </div>
            </div>

            <a href="mailto:alex@example.com" class="contact-button">
                Contact Me
            </a>

        </div>
    </main>

</body>
</html>
2. CSS file — style.css

css

/* Reset and box model */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Page styling */
body {
    font-family: Arial, sans-serif;
    background: linear-gradient(135deg, #dbeafe, #ede9fe);
    color: #1e293b;
    min-height: 100vh;
}

/* Center the profile card */
.profile-container {
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 30px 16px;
}

/* Main profile card */
.profile-card {
    position: relative;
    width: 100%;
    max-width: 380px;
    padding: 35px 25px;
    background-color: #ffffff;
    border: 1px solid #e2e8f0;
    border-radius: 20px;
    text-align: center;
    box-shadow: 0 12px 30px rgba(15, 23, 42, 0.12);
}

/* Positioned availability badge */
.profile-badge {
    position: absolute;
    top: 15px;
    right: 15px;
    padding: 7px 10px;
    background-color: #dcfce7;
    color: #166534;
    border-radius: 20px;
    font-size: 11px;
    font-weight: bold;
}

/* Profile image */
.profile-image-container {
    margin: 30px auto 20px;
    width: 120px;
    height: 120px;
}

.profile-image {
    display: block;
    width: 100%;
    height: 100%;
    object-fit: cover;
    border: 4px solid #c4b5fd;
    border-radius: 50%;
}

/* Name and role */
.profile-name {
    margin-bottom: 8px;
    font-size: 28px;
    color: #1e1b4b;
}

.profile-role {
    margin-bottom: 18px;
    font-size: 16px;
    font-weight: normal;
    color: #7c3aed;
}

/* Description */
.profile-description {
    margin-bottom: 22px;
    color: #64748b;
    font-size: 14px;
    line-height: 1.7;
}

/* Skills */
.skills-section {
    margin-bottom: 25px;
}

.skills-heading {
    margin-bottom: 12px;
    font-size: 16px;
}

.skills-list {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 8px;
}

.skill-tag {
    padding: 8px 12px;
    background-color: #f1f5f9;
    border: 1px solid #e2e8f0;
    border-radius: 8px;
    color: #334155;
    font-size: 12px;
}

/* Contact button */
.contact-button {
    display: block;
    width: 100%;
    padding: 13px 20px;
    background-color: #7c3aed;
    color: #ffffff;
    border-radius: 10px;
    text-decoration: none;
    font-size: 15px;
    font-weight: bold;
    transition: background-color 0.3s, transform 0.3s;
}

.contact-button:hover {
    background-color: #5b21b6;
    transform: translateY(-2px);
}

/* Responsive design for mobile screens */
@media (max-width: 480px) {
    .profile-card {
        max-width: 340px;
        padding: 25px 18px;
    }

    .profile-badge {
        top: 12px;
        right: 12px;
        font-size: 10px;
    }

    .profile-name {
        font-size: 24px;
    }

    .profile-image-container {
        width: 100px;
        height: 100px;
    }
}