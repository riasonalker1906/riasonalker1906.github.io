---
title: "Identifying Anxiety Behaviour in Children with Computer Vision"
date: 2024-10-28
layout: single
collection: projects
---
Powering researchers to automate behavioral analysis.

**Project Motivation:** Traditionally, child psychology researchers spend many hours manually labeling behavior in videos – watching each experiment video, pausing every second of the frame, recording behaviour observation according to a coding scheme (e.g.: 0 for no/low signs of fear, 1 for increased signs of fear), and having to repeat this tedious process for 600+ videos. 

**Solution proposed:** A computer vision pipeline using OpenPose and MediaPipe that brings down labeling time from days to minutes. The pipeline was integrated into a web app where researchers can upload a video, our models detect fear/freeze behavior, outputting a labeled CSV file.

### Key Highlights
- Collaborated with psychology researchers to validate behavioral assumptions.
- Detects the child, parent, and stranger using YOLOv8
- Tracks postural changes with YOLO Pose
- Analyzes facial expressions using MediaPipe
- Applies temporal rule-based logic to flag freeze behavior (≥ 2 seconds of stillness)
- Outputs a labeled CSV mapped to behavioral coding metrics (e.g., fear score 0–2, proximity, binary freeze flag)

### Impact
- Transform a multi-year annotation effort into just 30 hours for 600+ videos (584× faster labeling).
- Save thousands of dollars in hourly research labor costs.
- Allows researchers to use saved time to advance behavioural analysis and collect more data.

### User Experience Summary
![User Journey]({{ site.baseurl }}/assets/images/user-journey.png)



