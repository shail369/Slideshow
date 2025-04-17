# Photo-Slideshow App

This repository contains the codebase for a web-based Photo-Slideshow application. The app empowers users to upload a sequence of images and transform them into a cohesive video, complete with customization options such as background music and transition effects. Built using HTML, CSS, JavaScript, Python (Flask), and CockroachDB, the project is deployed via Render for seamless cloud accessibility.

## Project Overview

The primary goal of this project is to deliver an intuitive and visually appealing platform where users can easily create personalized video slideshows from their own images. The application guides users through uploading images, customizing their video (choosing music, transitions, and durations), previewing the result, and finally downloading the finished video file. The focus is on providing a smooth end-to-end experience, from media upload to video generation.

## Key Features

- **Image Upload:** Users can upload multiple images in common formats such as JPG and PNG. The interface supports both traditional file selection and drag-and-drop for enhanced usability. During the initial development phase, this functionality may be demonstrated with hardcoded images, but will later be connected to actual upload logic.
- **Video Customization:** After uploading, users can select which images to include in their slideshow, set the duration each image appears, and choose from available transition effects. There is also an option to add background music, either by uploading their own audio or selecting from a preloaded library.
- **Preview and Output:** The app provides a real-time preview of the video as users make customization choices. Playback controls (play, pause, rewind) allow users to review their slideshow before finalizing. Users can also specify output settings such as video resolution and quality.
- **User Authentication:** The platform includes a secure user authentication system, allowing users to sign up, log in, and manage their projects. An admin interface is available to view all registered users.
- **Backend and Database:** The backend is powered by Flask, handling all HTTP requests, authentication (using JWT tokens), and media processing. CockroachDB stores user data, image metadata, and audio library information, ensuring reliability and scalability.
- **Video Processing:** Python scripts are used to compile the selected images and audio into a video file, applying chosen transitions and durations. The system is designed to handle additional enhancements, such as multiple audio tracks and persistent processing even if the browser is closed.
- **Deployment:** The application is deployed on Render, providing robust hosting for both the frontend and backend components.

## Development Phases

The project is structured into three main milestones, each building upon the previous:

### Milestone 1: Frontend

The first phase focuses on designing the user interface. At this stage, the website layout and interactive elements are created, including image upload, customization panels, preview area, and authentication pages. Functionality may be simulated with placeholder data, with the goal of establishing a solid foundation for later integration of backend logic.

### Milestone 2: Backend & Database

In the second phase, the backend logic is implemented. This includes setting up the Flask server, connecting to CockroachDB, and enabling real user authentication. Media upload, retrieval, and management features are developed, along with the creation of database schemas for users, images, and audio files. The backend ensures secure and efficient handling of all user data and media assets.

### Milestone 3: Python Processing & Deployment

The final phase involves developing the core video processing scripts in Python. These scripts assemble the uploaded images and selected audio into a video file, applying user-defined settings. Additional features such as advanced transitions and multi-audio support may be included. Once complete, the entire application is deployed on Render, making it accessible to users via the web.
