## Wilkommen

You can use the [editor on GitHub](https://github.com/untitled-soundtrack/digitalebastelenzyklopaedie.github.io/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Tests

GENERATE THUMBNAIL

	1. Create one frame video with video stream and silent audio stream
	ffmpeg -f lavfi -i anullsrc=channel_layout=stereo:sample_rate=48000  -loop 1 -i frame_01.png -c:v libx264 -crf 18 -t 0.01  -pix_fmt yuv420p thumbnail_frame.mp4
	
	2. Concat the one frame video with normal video content
	ffmpeg -i thumbnail_frame.mp4  -i input_video.mp4 -filter_complex "[0:v:0][0:a:0][1:v:0][1:a:0]concat=n=2:v=1:a=1[v][a]" -map "[v]"  -map "[a]" -crf 18 -b:a 320K video_with_thumbnail.mp4
  
### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/untitled-soundtrack/digitalebastelenzyklopaedie.github.io/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.

### Adobe Premiere

#### WINDGERÄUSCHE ENTFERNEN

```markdown
1. Filter "Highpass" einsetzen
2. Cutoff "170 Hz" Yeah
```
![This is an image](https://64.media.tumblr.com/8ea82c8b5a98becaa49cd637d0d8f612/e99c2b06d934ab05-d4/s500x750/9dd9d5fa6b664eced9df0f43dd64c2a0115d4428.jpg)

Song anhören ([per Youtube](https://www.youtube.com/watch?v=9FFo21LlrWk))

| Song | Artist |
| --- | --- |
| Remotely Close: Silkyway | Kutiman & Elif Çağlar Muslu |




