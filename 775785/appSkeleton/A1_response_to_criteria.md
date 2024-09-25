Assignment 1 - Web Server - Response to Criteria
================================================

Overview
------------------------------------------------

- **Name:** Max Stanes
- **Student number:** n10884670
- **Application name:** ConVIDEOter
- **Two line description:** ConVIDEOter is a web-based video conversion and management system that allows users to upload, transcode and download videos via an intuitive interface. The application provides upload and transcoding progress feedback and user-specific download capabilities.


Core criteria
------------------------------------------------

### Docker image

- **ECR Repository name:** assignment1
- **Video timestamp:** 00:24
- **Relevant files:** 
    - /Dockerfile

### Docker image running on EC2

- **EC2 instance ID:** i-0ab9a84eafffa22f7
- **Video timestamp:** 00:41

### User login functionality

- **One line description:** Allows users to log in with credentials and receive a JWT token for authentication.
- **Video timestamp:** 00:45
- **Relevant files:**
    - /auth.js
    - /public/index.html
    - /routes/webclient.js
    - /routes/api.js

### User dependent functionality

- **One line description:** Displays user-specific content that being videos based on the logged-in user’s credentials.
- **Video timestamp:** user A: 00:56, user B: 01:52
- **Relevant files:**
    - /auth.js
    - /public/myVideos.html
    - /routes/webclient

### Web client

- **One line description:** A user interface allowing users to log in, upload videos, and view transcoding progress.
- **Video timestamp:** 00:45
- **Relevant files:**
    - /public/index.html
    - /public/myVideos.html
    - /public/login.html
    - /public/upload.html
    - /public/styles.css

### REST API

- **One line description:** REST API with endpoints for user login, uploads, downloads via hoppscotch testing
- **Video timestamp:** 02:44
- **Relevant files:**
    - /routes/api.js
    - /routes/webclient.js
    - /auth.js

### Two kinds of data

#### First kind

- **One line description:** Metadata of video files and hardcoded user login.
- **Type:** Structured
- **Rationale:** This data has a clear structure, such as user credentials and video metadata (like upload date and file names) that can be stored and queried using a structured database.
- **Video timestamp:** 00:57, 02:22
- **Relevant files:**
    - /routes/api.js
    - /auth.js

#### Second kind

- **One line description:** Video files uploaded by users.
- **Type:** Unstructured
- **Rationale:** Video files are large, complex, and stored as binary files on disk, without a schema that can be queried or indexed by conventional databases.
- **Video timestamp:** 01:04
- **Relevant files:**
  - /routes/api.js
  - /uploads/

### CPU intensive task

- **One line description:** Video transcoding using FFmpeg, which converts uploaded videos into mp4.
- **Video timestamp:** 01:08
- **Relevant files:**
    - /routes/api.js
    - /uploads/

### CPU load testing method

- **One line description:** htop was used to monitor CPU usage during the video transcoding process to test the load placed on the server.
- **Video timestamp:** 04:43
- **Relevant files:**
    - htop tool (used in video demo, no specific file)

Additional criteria
------------------------------------------------

### Extensive REST API features

- **One line description:** Not attempted
- **Video timestamp:**
- **Relevant files:**
    - 


### Use of external API(s)

- **One line description:** Not attempted
- **Video timestamp:**
- **Relevant files:**
    - 


### Extensive web client features

- **One line description:** Not attempted
- **Video timestamp:**
- **Relevant files:**
    - 


### Sophisticated data visualisations

- **One line description:** Not attempted
- **Video timestamp:**
- **Relevant files:**
    - 


### Additional kinds of data

- **One line description:** Not attempted
- **Video timestamp:**
- **Relevant files:**
    - 


### Significant custom processing

- **One line description:** Not attempted
- **Video timestamp:**
- **Relevant files:**
    - 


### Live progress indication

- **One line description:** Attempted
- **Video timestamp:** 01:08
- **Relevant files:**
    - /public/index.html
    - /routes/api.js


### Infrastructure as code

- **One line description:** Not attempted
- **Video timestamp:** 
- **Relevant files:**
    - 


### Other

- **One line description:** Not attempted
- **Video timestamp:**
- **Relevant files:**
    - 

