# Day 5

Today I want to create a solution to a real-life problem with the knowledge accumulated so far. In [Day 4](../4/README.md), I used a podcast transcript as an example of a large document. This is the fundamental building block for today's project.

## Project Purpose

This tool will generate a customizable report for each episode in a podcast.

## Project Technologies

- [Python RSS feedparser](https://pypi.org/project/feedparser/)
- [OpenAI's Whisper Model](https://github.com/openai/whisper)
- Google's Gemini Model (💭 Not required -- can use whatever LLM you want)

## Notebooks

### 1-download-podcasts.ipynb

[View Notebook](./1-download-podcasts.ipynb) &nbsp; • &nbsp; [Open Notebook in Collab](https://colab.research.google.com/github/jacobbridges/100-Days-Of-AI/blob/main/day/5/1-download-podcasts.ipynb)

Download the podcast episodes into the following folder structure:

```
CONFIG["output_dir"]
└── YYYY-MM-DD TITLE
    ├── YYYY-MM-DD TITLE.mp3
    └── metadata.json
```

Each episode will get a folder within the output directory. This will be useful in future notebooks for saving the transcription and report next to the correct audio file.

### 2-caption-podcast-episodes.ipynb

[View Notebook](./2-caption-podcast-episodes.ipynb) &nbsp; • &nbsp; [Open Notebook in Collab](https://colab.research.google.com/github/jacobbridges/100-Days-Of-AI/blob/main/day/5/2-caption-podcast-episodes.ipynb)

Short notebook, loop through each episode's audio file and transcribe via the whipser model. Save the transcription to the episode directory. Now the episode directory looks like:

```
CONFIG["output_dir"]
└── YYYY-MM-DD TITLE
    ├── YYYY-MM-DD TITLE.mp3
    ├── transcript.txt
    └── metadata.json
```

