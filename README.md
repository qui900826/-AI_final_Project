# AI_final_Project

Video Description based on OpenCLIP

Overview
- video-text retrieval is becoming an emerging requirement for people
- LAION-5B: open/public dataset for image-text model
- use the OpenCLIP image-text model on videos
- descriptive results that encapsulate the content of the video

Main Approach
1. The video is processed and transformed into frames.
2. From all the frames, one frame is selected from every 24 frames.
3. Tokenize the descriptions.
4. Both the images and descriptions are encoded using an encoder.
5. Cosine similarity is calculated between the encoded image and description pairs.
6. Select the description with the highest similarity as the label for each frame.
7. For each frame, select the description from the extracted frame that is closest to it, and merge them to create the video.
8. Merge video and audio to create the new video.

Prerequisite
- colab

Usage
- Quickly understand the content of the video through text.

Experiment results
- output_new.mp4
- output_interpolate_2.mp4
