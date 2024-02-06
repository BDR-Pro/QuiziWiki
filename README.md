# Quizify: Revolutionizing Learning with AI-Powered Wiki Summaries and ~~Bilingual~~ Quizzes

<a target="_blank" href="https://colab.research.google.com/github/BDR-Pro/QuiziWiki/blob/main/QuiziWiki.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

## 🚀 Introduction
Welcome to Quizify - the future of interactive learning! Dive into the world of knowledge with our AI-driven tool that transforms Wikipedia articles into captivating quizzes. Quizify isn't just a tool; it's an educational revolution. It summarises complex topics into crisp content and spins them into intriguing questions, all in not just one, but two languages. 

## 🌟 Features
- **AI-Powered Summaries**: Leveraging cutting-edge NLP, Quizify distills Wikipedia articles into concise summaries.
- **Bilingual Question Generation**: Get ready for a mind-bending quiz experience with questions generated in both English and French.
- **Seamless MongoDB Integration**: All this magic is neatly packed and stored in MongoDB, ensuring smooth access and management.
- **Dive into Learning**: Experience the thrill of mastering topics in both English ~~and French~~, enhancing your language skills as you learn.

## 🛠 Installation
Embark on the Quizify journey with a few simple steps:
```bash
!pip install wikipedia-api
!pip install gradio_client
!pip install "pymongo[srv]"
```

## 📖 How to Use
- **Step 1**: Fire up Quizify and feed it a Wikipedia page title.
- **Step 2**: Watch as it fetches summaries, morphs them into questions, and ~~cleverly translates them.~~
- **Step 3**: All this rich content is automatically organized and stored in MongoDB for you.

## 🌍 An Example Adventure
Let's take "Artificial Intelligence" for a spin. Quizify grabs the article, churns out thought-provoking questions, ~~translates them for a bilingual twist~~, and neatly files everything in MongoDB. 

## 💡 Contribute
Got a spark of genius? We welcome all trailblazers! Fork our repository, make your magic, and hit us with a pull request.

## 📜 License
Dive into the details of our project's license, and join us on this journey of knowledge and innovation.

🌌 **Quizify**: Where curiosity meets technology, creating a universe of learning without limits. Let's redefine the way the world learns, one quiz at a time. 🌠


# 🌟 Example Showcase: AI Unleashed in Quizzes

Dive into a vibrant example of Quizify's prowess: our journey through the "Artificial Intelligence" article. We've spun the complex world of AI into an interactive quiz, ready to challenge and intrigue!

### 🧠 From Article to Insight
- **Topic**: Artificial Intelligence
- **Summary**: From machines mimicking human intelligence to the evolution of AI, we cover the groundbreaking journey of AI. Discover its widespread use, from Google Search to self-driving cars, and explore the minds like Alan Turing who propelled this field forward.

### 🏛️ Categories and Sections
- Categories: A diverse array from AI basics to complex computational neuroscience.
- Sections: Delve into Goals, Techniques, Applications, and more, each a gateway to new knowledge.

### ❓ Quizzes: A Bilingual Brain Tease
- ~~French Queries: "Qu'entend-on par intelligence artificielle?" to "Quel est l'année où l'architecture de transformer a été développée?"~~
- English Translations: Tackling questions like "What defines artificial intelligence?" to "When was the transformer architecture developed?"

### 📚 MongoDB: Our Knowledge Repository
Each piece of this enlightening puzzle, from summaries to translated questions, finds a home in our MongoDB database, ready for your exploration and learning.


## Update 1

# 🧠 pageFiller: The Engine Behind Content Creation

At the heart of Quizify lies `pageFiller`, an innovative script designed to seamlessly bridge the worlds of philosophy, technology history, and the future with our learning platform. It dives into Wikipedia, fetching article summaries, categorizing knowledge, and dissecting sections to fuel our quiz-generation engine.

### How It Works:
- **Fetch and Analyze**: `pageFiller` taps into Wikipedia, extracting summaries, categories, and key sections from articles, starting with a deep dive into "Philosophy".
- **MongoDB Integration**: It doesn't just stop at analysis. Each piece of information, from article summaries to categories, is meticulously organized and stored in MongoDB, ensuring a rich database of knowledge.
- **Expand Your Horizon**: With `pageFiller`, we're constantly expanding our repository, covering everything from the roots of philosophical thought to the cutting-edge future of technology.

### Dive Deeper:
Our journey begins with an exploration of "Philosophy", where `pageFiller` meticulously categorizes each subdomain and fetches detailed summaries. This process not only enriches our content but also lays the groundwork for quizzes that challenge and inspire.

By integrating MongoDB, `pageFiller` ensures that every piece of knowledge is preserved, categorized, and ready to transform into engaging quizzes. It's how we're building a dynamic, ever-growing platform for learning.



## Update 2



## 🎓 Advanced Content Generation with Hugging Face API

Quizify has evolved! We're now harnessing the power of the Hugging Face API to elevate our quiz content creation. This cutting-edge tool allows us to generate detailed questions and answers based on Wikipedia summaries, complete with distractors for a comprehensive quiz experience.

### How It Works:
- **Hugging Face Integration**: Utilizing `https://huggingface.co/spaces/bader4k/question-gen-en`, Quizify dynamically generates quiz questions and multiple-choice answers directly from Wikipedia article summaries.
- **JSON-Powered Insights**: Each quiz question is crafted with precision, offering insights like this:
```json
{
  "page_title": "-ene",
  "summary": "The suffix -ene is used in organic chemistry...",
  "question": "Why would a Greek number suffix be inserted before the suffix -ene?",
  "choices": ["[A] to say that the double bond is between that atom and the next number up", "[B]...", "[C]...", "[D] to say that the double bond is between that atom and the atom with the next number up [ANSWER]"]
}
```
- **Loop Through Documents**: Our script navigates through all MongoDB documents, extracting titles and summaries to feed into the Hugging Face API, enriching our database with ready-to-use quiz content.

### Step into the Future of Learning:
With this update, Quizify not only brings knowledge to your fingertips but also challenges your understanding in fun, interactive ways. Dive into topics ranging from science to history and test your knowledge like never before.



## Update 3



## 🌐 Quizify Expands: Introducing Duplicate Removal and Enhanced Learning

Quizify is on a relentless mission to refine and expand its educational horizon. Our latest update introduces a sophisticated feature aimed at enhancing the quality and variety of our quizzes: the dynamic removal of duplicate choices in quiz questions.

### Highlighting Innovation: Removing Duplicate Choices

In our continuous quest to perfect Quizify, we've identified and addressed a crucial aspect that impacts the learning experience: duplicate choices within quiz questions. With our innovative `removeDublication` script, Quizify now automatically identifies and rectifies any redundancies, ensuring each quiz offers a unique and challenging learning opportunity.

### How It Works:
- **Detect and Rectify**: Leveraging advanced algorithms, `removeDublication` meticulously scans each quiz question for duplicate choices. Upon detection, it strategically replaces duplicates with unique, contextually relevant options.
- **Enhance Learning**: This process not only eliminates confusion but also enriches the quiz content, making every question a distinct learning moment.
- **Seamless Integration**: Operating in harmony with our MongoDB database, `removeDublication` ensures that all quizzes stored and retrieved are free from duplicates, maintaining the integrity and educational value of our platform.

### Example Transformation:
```python
@time_it
def removeDublication():
    # Script logic to detect duplicates and update questions
```
- **Before**: A quiz question might inadvertently contain duplicate choices, reducing its educational effectiveness.
- **After**: With `removeDublication`, each choice is unique, challenging learners to think critically and enhance their understanding.

### Join the Evolution of Quizify

This update signifies more than just a technical enhancement; it embodies our commitment to delivering an unparalleled learning experience. By eliminating duplicates, we not only refine our quizzes but also fortify Quizify's role as a beacon of interactive education.

### Contribute to the Future of Learning

Are you passionate about education and technology? Do you have ideas to make Quizify even better? We invite you to contribute to our journey. Whether it's through suggesting new features, improving existing ones, or offering feedback, your input is invaluable.

### 🚀 Ready for a Unique Challenge?

Embark on a learning adventure with Quizify today. Explore diverse topics, test your knowledge, and enjoy a quiz experience like no other. With Quizify, every question is a step towards new insights and discoveries.

### Everthing in json

```

{
  "_id": "65be47637a752d35e56fd1f2",
  "page_title": "-ene",
  "summary": "The suffix -ene is used in organic chemistry to name compounds with a -C=C- group, deriving from 'ethylene'. A number may precede '-ene' to indicate the double bond's position. The suffix also varies with the following letter (vowel or consonant) and indicates the number of double bonds in a compound, as seen in 'butadiene'. In inorganic chemistry, '-ene' denotes a one-atom thick layer, as in graphene.",
  "categories": {
    "Chemistry Suffixes": "https://en.wikipedia.org/wiki/Category:Chemistry_suffixes",
    "English Suffixes": "https://en.wikipedia.org/wiki/Category:English_suffixes",
    "Organic Chemistry Stubs": "https://en.wikipedia.org/wiki/Category:Organic_chemistry_stubs",
    "Articles Needing Additional References": "https://en.wikipedia.org/wiki/Category:All_articles_needing_additional_references",
    "Articles with Short Description": "https://en.wikipedia.org/wiki/Category:Articles_with_short_description"
  },
  "question": "Why would a Greek number suffix be inserted before the suffix -ene?",
  "choices": {
    "A": "to say that the double bond is between that atom and the next number up",
    "B": "to say there are -C=C- bonds in the compound",
    "C": "None Of The Above",
    "D": "to say that the double bond is between that atom and the atom with the next number up [ANSWER]"
  }
}




```


## Update 4

# Wikipedia Image Fetcher

Wikipedia Image Fetcher is a simple, efficient tool designed to retrieve the main image URL associated with a specific Wikipedia page title. Utilizing the Wikipedia API, this Python script offers an easy way to programmatically access visual content from the vast repository of Wikipedia articles. Whether you're building educational content, need images for a project, or simply exploring Wikipedia's rich database, Wikipedia Image Fetcher streamlines the process, delivering high-quality images directly to you.

## Features

- **Simple Integration**: Easily incorporate into any Python project to fetch Wikipedia images.
- **Customizable Image Size**: Specify the desired thumbnail size for the perfect fit.
- **Efficient and Fast**: Quickly retrieves image URLs with minimal overhead.

## Prerequisites

Before you begin, ensure you have the following installed:
- Python 3.x
- `requests` library

## Installation

1. **Python Installation**: Make sure Python 3.x is installed on your system. If not, download and install it from [python.org](https://www.python.org/downloads/).

2. **Install Requests Library**: If you haven't installed the `requests` library yet, you can do so by running the following command in your terminal:

   ```bash
   pip install requests
   ```

## Usage

To use the Wikipedia Image Fetcher, follow these steps:

1. **Import the Function**: Include the `get_wikipedia_image_url` function in your Python script.

2. **Call the Function**: Pass the title of the Wikipedia page to the function as a string. Ensure the title accurately matches the Wikipedia page.

   ```python
   page_title = "Python (programming language)"
   image_url = get_wikipedia_image_url(page_title)
   print(image_url)
   ```

3. **Retrieve the Image URL**: The function returns the URL of the main image. If no image is found, it returns a message indicating so.

## Example

Here's a quick example demonstrating how to fetch the image URL for the Wikipedia page on "Python (programming language)":

```python
from get_wikipedia_image_url import get_wikipedia_image_url

# Specify the Wikipedia page title
page_title = "Python (programming language)"

# Fetch and print the image URL
image_url = get_wikipedia_image_url(page_title)
print(f"Image URL: {image_url}")

```

**Happy Image Fetching!** Explore the visual side of Wikipedia with ease and bring knowledge to life in your projects.





**Quizify**: Where learning meets innovation. Together, let's build a smarter future. 🌟


**Quizify**: Redefining learning, one question at a time. Join us on this exciting journey of knowledge exploration and discovery.

---


🚀 **Quizify**: Ignite your curiosity and embark on a journey of discovery, one quiz at a time! 🌌

<img src="https://github.com/BDR-Pro/QuiziWiki/assets/91114465/e253b3e5-93b2-44e5-82ea-856256187382" width="1024" height="720" alt="Sophisticated humanoid robot thinking">

