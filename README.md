# Multi-Agent SEO Blog Generator

## Overview
This repository contains a multi-agent system that generates high-quality, SEO-optimized blog posts on trending HR topics. It consists of multiple agents handling research, content planning, generation, SEO optimization, and review.

## Features
- **ResearchAgent**: Fetches trending HR topics from NewsAPI.
- **ContentPlanningAgent**: Creates a structured blog outline.
- **ContentGenerationAgent**: Generates detailed blog content using GPT-2.
- **SEOOptimizationAgent**: Enhances content for SEO using TF-IDF.
- **ReviewAgent**: Assesses readability and suggests improvements.
- **Markdown Export**: Saves the final content as a markdown file.

## Installation

Clone the repository:
```bash
git clone https://github.com/charu1605/multi_agent_seo_blog_generator.git
cd multi_agent_seo_blog_generator
```
```bash
git clone https://github.com/charu1605/multi_agent_seo_blog_generator.git
cd multi_agent_seo_blog_generator
```

Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage
Run the script to generate a blog post:
```bash
python main.py
```

## File Structure
```
multi_agent_seo_blog_generator/
│── agents/
│   ├── research_agent.py
│   ├── content_planning_agent.py
│   ├── content_generation_agent.py
│   ├── seo_optimization_agent.py
│   ├── review_agent.py
│── main.py
│── requirements.txt
│── README.md
│── output/
│   ├── blog_post.md
```

## Requirements
- Python 3.8+
- Transformers
- Requests
- BeautifulSoup4
- Scikit-learn
- Textstat
- Markdown

## System Architecture
1. **Research Agent**: Retrieves trending HR topics.
2. **Content Planning Agent**: Structures blog content.
3. **Content Generation Agent**: Writes the blog.
4. **SEO Optimization Agent**: Enhances content for search visibility.
5. **Review Agent**: Checks readability.
6. **Final Markdown Export**: Saves the blog post in Markdown format.

## Output
The generated blog post is saved as `blog_post.md`.

## Contribution
Feel free to fork this repository and contribute improvements.

## License
This project is licensed under the MIT License.

