# Reddit Post Classification with Fine-tuned Llama 3.1

This project fine-tunes Llama 3.1 (8B) on Reddit data to classify posts into six broad categories.

## Overview

We leverage the Llama 3.1 8B model with Alpaca-style fine-tuning to create a specialized classifier for Reddit posts. The model is trained on curated datasets from various Reddit communities to accurately categorize content based on its primary topic.

## Categories

- **Entertainment**: Posts related to movies, TV shows, music, and general entertainment content
- **Health**: Medical advice, fitness tips, mental health discussions, and wellness topics
- **Comedy**: Jokes, humor, memes, and funny stories
- **Professional**: Career advice, workplace discussions, business topics, and professional development
- **Travel**: Travel tips, destination recommendations, trip reports, and tourism-related content
- **Education**: Academic discussions, learning resources, study tips, and educational content

## Dataset

The training data consists of Reddit posts collected from relevant subreddits for each category. The data is stored in both pickle (`.pkl`) and CSV formats:

- Original data: `Reddit_{category}_original.pkl`
- Processed data: `{category}_dataset.csv`

### Data Structure

- `data/`: Contains the standard dataset for all six categories
- `data_large/`: Contains expanded datasets for the categories

## Model

- **Base Model**: Llama 3.1 (8B parameters)
- **Fine-tuning Method**: Alpaca-style instruction tuning
- **Implementation**: `CSS488_Llama3_1_(8B)_Alpaca.ipynb`

## Files

- `CSS488_Llama3_1_(8B)_Alpaca.ipynb`: Main notebook for model fine-tuning and evaluation
- `data_collect.ipynb`: Data collection script for gathering Reddit posts
- `proDataCollect.ipynb`: Enhanced data collection for larger datasets

## License

This project is licensed under the MIT License.