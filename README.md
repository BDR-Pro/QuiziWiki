# Quizify: Revolutionizing Learning with AI-Powered Wiki Summaries and Bilingual Quizzes

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
---

## 🧠 pageFiller: The Engine Behind Content Creation

At the heart of Quizify lies `pageFiller`, an innovative script designed to seamlessly bridge the worlds of philosophy, technology history, and the future with our learning platform. It dives into Wikipedia, fetching article summaries, categorizing knowledge, and dissecting sections to fuel our quiz-generation engine.

### How It Works:
- **Fetch and Analyze**: `pageFiller` taps into Wikipedia, extracting summaries, categories, and key sections from articles, starting with a deep dive into "Philosophy".
- **MongoDB Integration**: It doesn't just stop at analysis. Each piece of information, from article summaries to categories, is meticulously organized and stored in MongoDB, ensuring a rich database of knowledge.
- **Expand Your Horizon**: With `pageFiller`, we're constantly expanding our repository, covering everything from the roots of philosophical thought to the cutting-edge future of technology.

### Dive Deeper:
Our journey begins with an exploration of "Philosophy", where `pageFiller` meticulously categorizes each subdomain and fetches detailed summaries. This process not only enriches our content but also lays the groundwork for quizzes that challenge and inspire.

By integrating MongoDB, `pageFiller` ensures that every piece of knowledge is preserved, categorized, and ready to transform into engaging quizzes. It's how we're building a dynamic, ever-growing platform for learning.



## Update 2

---

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

---

**Quizify**: Redefining learning, one question at a time. Join us on this exciting journey of knowledge exploration and discovery.

---


🚀 **Quizify**: Ignite your curiosity and embark on a journey of discovery, one quiz at a time! 🌌

<img src="https://github.com/BDR-Pro/QuiziWiki/assets/91114465/e253b3e5-93b2-44e5-82ea-856256187382" width="1024" height="720" alt="Sophisticated humanoid robot thinking">

