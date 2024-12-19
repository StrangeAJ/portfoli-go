---
title: "Room8"
date: 2022-12-01
description: "An application made with Flutter for listing PG rooms uploaded by tenants for specific organizations."
tech: ["Flutter", "Node.js", "MongoDB", "Imgur"]
source: "https://github.com/StrangeAJ/Room8"
live: "https://room8build-production.up.railway.app/"
---

## Overview

Room8 is an application built with Flutter that allows tenants to list PG rooms for specific organizations, simplifying the process of finding accommodations.

### Key Features
- **User-Friendly Interface**: Easy navigation and intuitive design for both tenants and seekers.
- **Real-Time Listings**: Immediate updates to room availability and details.
- **Image Uploads**: Integrated with Imgur for efficient image storage and retrieval.

### Technical Implementation
- **Frontend**: Developed using Flutter for cross-platform compatibility.
- **Backend**: Implemented with Node.js and hosted on Cyclic.sh and Railway.app.
- **Database**: Utilized MongoDB for data storage.
- **Image Storage**: Integrated Imgur API for handling image uploads and storage.

### Challenges & Solutions
- **Challenge**: Ensuring real-time updates and synchronization across platforms.
  - **Solution**: Implemented real-time database listeners and optimized API calls.
- **Challenge**: Managing image uploads efficiently.
  - **Solution**: Integrated Imgur API to handle image storage, reducing server load.
