### Audio description of video for visually impaired people

The development of online movie services has revealed the problem of video content accessibility on the Internet for people with disabilities, especially for those who have vision impairments. It is very important that the video on the device screen is understandable, accessible and convenient for people suffering from the disease. With the modern development of computing resources, machine learning technologies and big data, this problem can be solved by applying the listed tools. The aim of this research is to create a tool that will help people with vision impairments understand what is happening in a specific scene of a movie.


### Overall description of our method

**Interface**: user selects processed video or uploads a new one.
**Splitting video to scenes**: video is send to served which splits it into scened with neural networks.
**Scene description**: neural networks generate a description for every scene.
**Voiceover**: neural networks generate voiceover for every scene.
**Special player**: user watches video in a special player, which plays voiceover along with the original video.

[Here is a video demonstration of our method](https://youtu.be/OANhJ0FJlQ8)

![img](readme_imgs/scheme.png)


### Suggestions for future work

- Improvement of the existing video stop system
- Inserting the background sound of a movie fragment over the voiceover of the announcer to avoid losing the atmosphere of the movie
- Better selection of model hyperparameters and model training
- Creation of a recommendation system based on the created text descriptions

### Running the system
Just install docker and run:
```bash
docker-compose up -d --build
```
The building can take quite a long time, because we use several heavy neural networks.

After that, the solution will be available at [http://localhost:1337 ](http://localhost:1337). You can upload your own video to test our system.
