# Multi-Agent Blog Generation System

## Overview
This project is a Python-based **multi-agent system** designed to generate high-quality, SEO-optimized blog posts on trending HR topics. The system consists of multiple agents, each responsible for a specific task:

1. **Research Agent** - Fetches trending HR topics from the NewsAPI.
2. **Content Planning Agent** - Creates a structured blog outline based on the topic.
3. **Content Generation Agent** - Uses GPT-2 for generating a detailed blog post.
4. **SEO Optimization Agent** - Enhances content using TF-IDF keyword optimization.
5. **Review Agent** - Assesses readability and suggests improvements.
6. **Storage Module** - Saves the final blog post in Markdown format.

## Installation
### Prerequisites
Ensure you have **Python 3.8+** installed on your system.

### Setup Instructions
1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/multi-agent-blog.git
   cd multi-agent-blog
   ```
2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
3. **Set up API keys:**
   - Obtain an API key from [NewsAPI](https://newsapi.org/).
   - Set it as an environment variable:
     ```bash
     export NEWS_API_KEY="your_api_key_here"
     ```

## Usage
Run the blog generation script:
```bash
python main.py
```
This will generate an SEO-optimized blog post and save it as a Markdown file.

## System Architecture
### Workflow
1. **ResearchAgent** fetches trending HR topics.
2. **ContentPlanningAgent** structures the outline.
3. **ContentGenerationAgent** writes a detailed article using GPT-2.
4. **SEOOptimizationAgent** highlights key terms for better search visibility.
5. **ReviewAgent** checks readability and suggests improvements.
6. **Storage Module** saves the final blog as a Markdown file.

### Technologies Used
- **NLP & AI:** `transformers` (GPT-2)
- **Web Scraping:** `requests`, `BeautifulSoup`
- **SEO Optimization:** `sklearn.feature_extraction.text.TfidfVectorizer`
- **Readability Analysis:** `textstat`
- **Markdown Conversion:** `markdown`

## File Structure
```
multi-agent-blog/
│── main.py  # Entry point for blog generation
│── research_agent.py  # Fetches trending topics
│── planning_agent.py  # Creates blog outline
│── generation_agent.py  # Generates blog content
│── seo_agent.py  # Optimizes blog for SEO
│── review_agent.py  # Checks readability & suggests improvements
│── storage.py  # Saves blog as Markdown
│── requirements.txt  # List of dependencies
│── README.md  # Project documentation
│── blog_output/  # Directory where generated blogs are stored
```

## Example Output
A sample blog post is saved in `blog_output/blog_post.md`.

## Contributing
Feel free to fork and enhance the project. Contributions are welcome!

## License
This project is licensed under the MIT License.
