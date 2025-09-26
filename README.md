# tep-website-data
This repo is served as database for member and project info for TEP members.


## TEP member Instructions

As a team member, you can edit your profile directly:

1. Navigate to the data file (`data/members.json`).
2. Click the pencil icon to edit the json, you can add a new entry, and the id should be incremented.
3. Upload your photo to `assets/members_pic/` and add the path `./assets/members_pic/your-name.png"` to your json entry. The photo should be a square image.
4. The project field, if any, should be an array of project ids from `data/projects.json`.
5. Commit directly to the main branch.

Example entry:
```json
{
    "id": 1,
    "name": "Meichen Ji",
    "photo": "./assets/members_pic/meichen-ji.png",
    "programName": "Software Technology",
    "degreeLevel": "Master",
    "yearOfStudy": "1",
    "description": "Hi, I am Meichen Ji, a first-year Master's student in Software Technology at LNU. I'm particularly interested in machine learning and exploring how AI technologies can solve complex problems across various domains.",
    "projects": [1, 2]
  },
```

What it looks like on the website:
![member_example](./readme_img/member_example.png)


## TEP project Instructions
As a team member, you can edit your project directly:
1. Navigate to the data file (`data/projects.json`).
2. Click the pencil icon to edit the json, you can add a new entry, and the id should be incremented.
3. Upload your project image to `assets/projects_pic/` and add the path `./assets/projects_pic/your-project.png"` to your json entry. The image should be a horizontal rectangle.
4. Commit directly to the main branch.

Example entry:
```json
{
    "id": 1,
    "title": "Teaching Assistant",
    "date": "2025-09-01",
    "description": "Assisting in grading assignments, holding office hours, and supporting students in understanding course material.",
    "category": "Education",
    "image": "./assets/projects_pic/ta.jpg"
  },
```

What it looks like on the website:
![project_example](./readme_img/project_example.png)


## TODO
- [ ] Make the info automatically update on the website, currently it needs to be manually deployed.
- [ ] Add more fields to member and project info, e.g., social media links, project links, etc.
