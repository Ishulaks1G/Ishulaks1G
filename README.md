from moviepy.editor import *

# Define text scenes for the story
scene1 = TextClip("Late one night, Arun stayed back at his campus lab...", fontsize=50, color='white', size=(1280, 720))
scene2 = TextClip("The clock struck 11:59 PM... The building was eerily silent.", fontsize=50, color='white', size=(1280, 720))
scene3 = TextClip("As he opened the storeroom, a cold breeze swept past...", fontsize=50, color='white', size=(1280, 720))
scene4 = TextClip("A shadow moved across the wall... It didn't belong to him.", fontsize=50, color='white', size=(1280, 720))
scene5 = TextClip("The shadow grew and whispered: 'Leave... or stay forever...'", fontsize=50, color='white', size=(1280, 720))

# Create background clips
background_clip = ColorClip(size=(1280, 720), color=(0, 0, 0), duration=10)

# Add text to scenes
text_scenes = [
    CompositeVideoClip([background_clip, scene1.set_position("center")], duration=4),
    CompositeVideoClip([background_clip, scene2.set_position("center")], duration=4),
    CompositeVideoClip([background_clip, scene3.set_position("center")], duration=4),
    CompositeVideoClip([background_clip, scene4.set_position("center")], duration=4),
    CompositeVideoClip([background_clip, scene5.set_position("center")], duration=5),
]

# Concatenate all scenes
final_video = concatenate_videoclips(text_scenes)

# Add background music or effects
audio_clip = AudioFileClip("whispers.mp3")  # Add a spooky background audio
final_video = final_video.set_audio(audio_clip)

# Export the video
final_video.write_videofile("whispering_shadows.mp4", fps=24) 👋 Hi, I’m @Ishulaks1G
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Ishulaks1G/Ishulaks1G is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
