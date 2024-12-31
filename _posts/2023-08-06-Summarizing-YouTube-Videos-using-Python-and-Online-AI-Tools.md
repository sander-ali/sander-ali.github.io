---
layout: post
title: "Summarizing YouTube Videos using Python and Online AI Tools"
date: 2023-08-06 09:00:00-0400
tags: [Text Summarization, Video Summarization, ChatGPT, Whisper Api, Python]
thumbnail: assets/img/blog/Summarize_Youtube_2023.JPG
---

If you have a lot of videos to transcribe and summarize, using speech-to-text technology can be a time-consuming and tedious process. OpenAI’s Whisper technology has made it easier to transcribe your videos into an audio file, and then use ChatGPT’s advanced summarization algorithm to create concise summaries. Let’s take a look!

## Introduction to Summarization of YouTube Videos using Google Chrome Extension and ChatGPT

ChatGPT is an impressive and powerful AI chatbot that is capable of effectively summarizing Youtube videos. The summarization process is quick and straightforward when utilizing ChatGPT. It is worth noting that the summarization process is even more efficient when a transcript of the video is available. However, the absence of a video transcript poses a challenge for ChatGPT.

The Youtube Summary with ChatGPT Chrome extension is a valuable tool for summarizing Youtube videos. With the assistance of the AI chatbot ChatGPT, the extension can even transcribe any Youtube video. The extension simplifies the summarization process, allowing users to summarize any video with just a click of a button. By utilizing this extension, users can stay informed and up-to-date with current events. The extension saves time that would otherwise be spent watching videos, enhancing the overall Youtube experience.

To install Youtube Summary with ChatGPT, follow these steps:

- Install the Youtube Summary with ChatGPT code from GitHub.

- Unzip the file and open it in an IDE of your choice.

- In the terminal, run “npm install”.

- Run webpack to generate the ‘dist’ folder by running “npm run build” or “npm run build-release”.

- Open Chrome extensions and enable developer mode.

- Click on “Load unpacked” and select the “dist directory”.

- You can now install and run Youtube Summary with ChatGPT on your device.

## Summarization of YouTube video with Python and ChatGPT

If you find yourself fatigued from viewing numerous videos on YouTube and attempting to retain information from each one, utilizing ChatGPT to condense the content is the optimal solution for you. Following is a quick way to summarize YouTube Videos with speech-to-text API and ChatGPT technology.

First, identify the video of your choice on Youtube.

Create a python project to begin, you can use your own choice of IDE, it can be visual studio code, PyCharm or any other. We need to install a python package pytube [https://pytube.io/en/latest/]. Create a virtual environment and run the following command:

```shell
pip install pytube 
```
In order to download the video of your choice from youtube, copy-paste the following code snippet and run it, accordingly.

```shell
from pytube import YouTube

def ytvd(url_s):
    YTObj = YouTube(url_s)
    YTObj = YTObj.streams.get_highest_resolution()
    try:
        YTObj.download()
    except:
        print("There was an error while downloading")
    print("Download is completed successfully")


url_s = "Paste your YouTube video link here"
ytvd(url_s)
```
The video will be now downloaded and saved to your device.

## Convert Video to Audio

In order to perform video to audio conversion, we need another python package, i.e. moviepy.

Install the package by running the following command.

```shell
pip install moviepy
```

After installing, run the following code snippet to extract audio from the video.

```shell
from moviepy.editor import *
video_name = "Write the name of the video you have download"
vid = VideoFileClip(f"{video_name}.mp4")
vid.audio.write_audiofile(f"{video_name}.mp3")
```

An audio file of the same name will be saved to your device.

## Convert Audio to Text

With the progression of Generative AI, several tools are now available that can convert the audio file to its textual counterpart. However, in this article, we consider the use of Whisper API from OpenAI.

In order to utilize Whisper API you need to visit the website [https://openai.com/index/openai-api/] and create an account. Whisper API provides $18 worth of credit to every new account as they have a Free Tier. For this demo, the number of credits obtained with the free account are enough, however, to be safe, you can check the usage of your credits on your personal page. The option for usage statistics will be available on the top right corner.

You will require an API key to access Whisper API from python IDE. You can navigate to “API Keys” page from “User” tab and press generate a new key. From the settings section, you also need to retrieve the organization ID.

Once you are done with the logistics of the keys and information available to you, you can proceed further.

First, you need to install the OpenAI package by using the following command:

```shell
pip install openai
```

Its recommended to keep the information acquired from OpenAI account to a json file, i.e. key.json, as shown below:

```shell
{
    "key": "YOUR-PERSONAL-KEY-HERE",
    "organization_id" : "YOUR-PERSONAL-ORGANIZATION-ID-HERE"
}
```

The following code snippet reads the local mp3 file and calls OpenAI service to convert audio file into text. It should be noted that Whisper can directly convert video files to text as well, so you can try that feature as well.

```shell
import openai
import json

aud_name = "The name of the audio file.mp3"
aud_file= open(aud_name, "rb")

# Reading keys
api_info_path = "key.json"
with open(api_info_path, "r") as f:
    keys = json.load(f)
whisp_key = keys["key"] 
org_id = keys["organization_id"] 

# Settings keys to the API module
openai.organization = org_id
openai.api_key = whisp_key

print("Be Patient ... Converting your audio to text")
tp = openai.Audio.transcribe("whisper-1", aud_file)
txt = tp["text"]
print(txt)
```

Once the text is available, it is easy to summarize it using ChatGPT, all you need to do is to run the following set of commands.

## Summarizing the Text

Copy the text you obtained from the previous step and paste it in place of {text}

Code Snippet

```shell
print("Be Patient ... ChatGPT is summarizing your text")
response = openai.ChatCompletion.create(
model="gpt-3.5-turbo",
messages=[
        {"role": "system", "content": "You are ChatGPT, a large language model trained by OpenAI. Answer as concisely as possible."},
        {"role": "user", "content": f"Summarize the following text: {text}"}
    ]
)

print(response['choices'][0]['message']['content'])
```

and Voila ! the summarized text is ready.

## Text Summarization Tools

The last step uses ChatGPT to summarize the text, however, if you would like to use other AI tools that can summarize the text obtained from the second-last step, you can use the following but not limited to:

#### Quill Bot

Quilllbot is a summarizing tool that gives you creative freedom with how much or little of your writing you need to summarize or paraphrase. It can be used within the Quillbot platform or integrated into Word and Google Docs. Quilllbot uses machine learning to scan text, suggesting synonyms, and checking for plagiarism. This is helpful when you’re writing content for a client or if you are writing college-level essays.

#### Genei

Genei is an artificial intelligence summary tool that can extract keywords from any long article or research paper and summarize it into easily digestible content. It’s used by college students when conducting research, as well as people who write longer content and aren’t quite sure what to emphasize with a bullet list in their own summaries. Genei is trusted by thought leaders and experts such as Berkeley university, Harvard, Oxford, Stanford and more.

#### Study Crumb

Study Crumb is an AI tool specifically designed for students who need help writing academic works. From book reports to term papers, Study Crumb lets you order essays and different reports based on what you need. The AI program matches you with a writer who’s an expert at the writing you need to be completed.

#### Jasper

Jasper is an extremely useful writing tool, because it provides a large number of features for writers. For example, Jasper has a text summarizer that allows you to pick out the most important lines of text.

#### Paraphraser.io

Paraphraser.io strives to provide high-quality paraphrasing, with a human feel, despite being an AI tool. The company’s program runs faster than other AI-based summary generators because of its grammatically correct and more readable content.

and many many many more…

## Summarizing YouTube Videos using Websites

The article already discussed one extension that allows the user to summarize YouTube Videos. The implications for such summarization can be extended to student learning process, teachers and researchers for expanding their knowledge base, and Content Creators.

This article presents three more extensions that can be used to summarize the YouTube videos among many that are available.

#### Glasp

Glasp extension is extremely useful in summarizing any video. It uses AI technology and advanced machine learning techniques first to generate a transcript, which it then uses to create a summary that includes certain phrases from the Youtube video.

#### Glairty

Introducing Glairty, a Chrome extension designed to enhance your Youtube experience. This innovative tool automatically generates video summaries as soon as you start playing a video. Additionally, you have the flexibility to tailor the prompts sent to ChatGPT for more personalized video summaries.

With Glairty, you are in control. You can easily toggle between automatic and manual summary generation for any video, allowing you to choose the method that suits your preferences. Whether you prefer to utilize your ChatGPT account or OpenAI’s API key, Glairty provides a seamless integration for a customized summarization experience.

#### YouTube Digest

This extension offers a plethora of impressive features, making it a standout option among the available choices. One notable feature is its ability to summarize videos in various formats.

Users can obtain a summarized version of the video in bulleted form, as well as in the form of articles, paragraphs, or sections with headings. Additionally, the extension provides a time-stamped summary, facilitating easier navigation and enabling users to watch specific parts of interest.

Furthermore, the summary can be exported to a document or PDF format. Finally, the text-to-speech feature saves time by allowing users to listen to the summaries instead of reading them, similar to podcasts. Notably, this extension is completely free to use.
