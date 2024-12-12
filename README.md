#  YouTube Playlist AI Chatbot 🤖🎥
Quickly summarizes the contents of YouTube videos in a public playlist and answers questions based on it.

## Brief Summary
This project focuses on building an AI-powered chatbot that interacts with YouTube playlists, offering intelligent insights and conversational capabilities for video content. The pipeline involves transcript processing, embedding generation, and retrieval-based augmented generation (RAG) for natural language responses.

<div style="display: flex; justify-content: space-between;">
   <img src="https://avatars.githubusercontent.com/u/25750857?s=200&v=4" alt="Image 1" style= "width: 30%; height: auto;"/> 
   <img src="https://www.docker.com/wp-content/uploads/2023/08/logo-guide-logos-1.svg" alt="Image 1" style = "width: 30%; height: auto;"/>
    <img src="https://w1.pngwing.com/pngs/835/530/png-transparent-python-logo-programming-language-computer-programming-python-programming-basics-for-absolute-beginners-scripting-language-source-code-php-code-climate-inc.png" alt="Image 2" style = "width: 30%; height: auto;"/>
</div>

## Workflow
1. **Fetch Transcripts**  
   Extract video transcripts from a YouTube playlist.  
   ![Fetching Transcripts](https://cdn.prod.website-files.com/634e7aa49f5b025e1fd9e87b/664e41b6eda3d7487ae3c577_descript_s_youtube_description_generator_writing_a_2e1c.webp)

2. **Data Cleaning**  
   Remove unnecessary data for clean processing.  
   ![Cleaning Process](https://datascientest.com/en/files/2023/04/illu_data_cleaning_blog_2-07.jpg)

3. **Chunk and Generate Embeddings**  
   Split transcripts into manageable chunks and use embeddings for semantic understanding.  
   ![Embeddings](https://miro.medium.com/v2/resize:fit:717/1*2G5plo83o4l9PcriBG4ncA.png)

4. **AI-Powered Responses**  
   Use RAG (Retrieval Augmented Generation) model for chatbot conversations.  
   ![Chatbot Interaction](https://pub-e93d5c9fdf134c89830082377f6df465.r2.dev/2024/02/The-RAG-Processs-1024x356.webp)


# Demo
Working of the tool
[Screencast from 14-04-24 08:31:23 AM IST.webm](https://github.com/SaumyaRR8/Youtube-playlist-chat/assets/97652981/0874ecb1-3bb8-4369-9b2c-eead3b039546)

## Running the tool
Create `.env` file in the root directory of the project, copy and paste the below config. Replace the `OPENAI_API_TOKEN` configuration value with your key `{OPENAI_API_KEY}`. Other properties are optional to change and be default.

```bash
OPENAI_API_TOKEN={OPENAI_API_KEY}
EMBEDDER_LOCATOR=text-embedding-ada-002
EMBEDDING_DIMENSION=1536
MODEL_LOCATOR=gpt-3.5-turbo
MAX_TOKENS=200
TEMPERATURE=0.0
```

2. From the project root folder, open your terminal and run `docker-compose up`.
3. Navigate to `localhost:8501` on your browser when docker installion is successful.

#### Prerequisites

1. Make sure that [Python](https://www.python.org/downloads/) 3.10 or above installed on your machine.
2. Download and Install [Pip](https://pip.pypa.io/en/stable/installation/) to manage project packages.
3. Create an [OpenAI](https://openai.com/) account and generate a new API Key: To access the OpenAI API, you will need to create an API Key. You can do this by logging into the [OpenAI website](https://openai.com/product) and navigating to the API Key management page.

Then, follow the easy steps to install and get started using the app.


## Features 🌟
- [x] Fetch YouTube transcripts
- [x] Clean and preprocess data
- [x] Generate embeddings
- [x] Interactive chatbot using RAG models


