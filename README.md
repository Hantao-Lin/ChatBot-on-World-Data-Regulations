# ChatBot on World Data Regulations
## Introduction 
In the rapidly evolving arena of international business, the comprehension of diverse laws and
regulations becomes essential for business owners to circumvent potential penalties. However,
not every business owner has the luxury of time or resources to delve into these complex legal
frameworks, especially when considering the significant variations in laws across different
countries. Although many enterprises might have specialized legal teams, a foundational
understanding of pertinent laws and regulations remains invaluable for business owners
overseeing their operations.
This research paper introduces 'Alex', an innovative world data policy chatbot, engineered to
promptly equip stakeholders with pertinent global data regulation information. Alex is designed
to narrow the informational divide and simplify legal data accessibility, thereby enhancing
decision-making for business owners and stakeholders alike.
## Research 
In our research, we leveraged the hierarchical structure of ontologies as our logical foundation
for developing the chatbot. The dataset employed encompasses a comprehensive array of data
regulation elements, including definitions, laws, and online privacy policies from 158 countries.
Our research unfolds in several phases, each exploring different methodologies to ascertain the
most relevant country, section, and content. We employed various models, including TF-IDF,
Multi-QA (multi-qa-MiniLM-L6-cos-v1), and Distilled BERT
(distilbert-base-uncased-distilled-squad), to enhance the chatbot's capabilities. These models
were qualitatively evaluated based on their output relevance and accuracy. The findings suggest
that the Multi-QA model is optimal for identifying relevant countries and content, while TF-IDF
excels in pinpointing pertinent sections.
## Stucture of the ChatBot
## Ontology of United States (One country of many others) 
## Result 
## Conclusion & Recommendation
Throughout our research, which involved visualizing ontologies for 158 countries' data policies
and identifying the best models for country, section, and context relevancy, we have identified
key findings and recommendations for each part:
### Part I - Knowledge Graphs:
Our ontology visualization process provided valuable insights, particularly in potential
refinements such as customizing sentence breakpoints. It also highlighted the effectiveness of
NER (Named Entity Recognition) in identifying law entities. While not flawless, NER was
reasonably effective in identifying most laws present in the text. Further enhancement of the
ontology is recommended through additional data cleaning, especially since some laws were
incompletely extracted or truncated. Additionally, incorporating OSCR (Ontology-based
Semantic Composition Regularization) could significantly improve our model’s ability to
recognize entity relationships, resulting in a cleaner and more effective model, as opposed to
relying solely on hard coded logic.
### Part II - Country:
The experiments conducted demonstrated that both TF-IDF and the Multi-QA model are
excellent choices for accurately identifying countries from user input. Future analyses involving
more complex questions are suggested to further assess their capabilities.
### Part III - Section:
Our evaluation of five specific questions revealed that both TF-IDF and Multi-QA are effective
for identifying sections within user input, with TF-IDF having a slight performance edge.
However, the Distilled BERT-Based model was not a suitable option for this task. Introducing
more complex questions in future studies could help differentiate which model performs best. It
is hypothesized that TF-IDF might struggle when the target section name is shorter in word
count than non-target section names. Therefore, exploring additional refinements or alternative
models is necessary to address these challenges.
### Part IV - Content:
Qualitatively evaluating the results produced by all three models was challenging. Both
Multi-QA and TF-IDF slightly outperformed the Distilled BERT-Based Model, particularly on
question 5, where Multi-QA provided more detailed and subjectively more accurate information.
A common issue with all models was the unclean formatting of output, primarily due to the
initial conversion of PDFs into dataframes, where words were not properly segmented. Further
data cleaning is required for clearer results. To enhance accuracy and relevance, the use of
ChatGPT, an NLU (Natural Language Understanding) level model, is proposed. Furthermore,
implementing OSCR could notably improve semantic understanding.

In summary, this research venture offers a profound exploration into the integration of
Knowledge Graphs and advanced natural language processing techniques within a
question-answering chatbot framework. The findings not only underscore the efficacy of these
technologies but also illuminate their transformative impact in the realm of information retrieval.
By leveraging these sophisticated tools, stakeholders can now access pertinent data with
unprecedented speed and precision, thereby revolutionizing the way information is consumed
and utilized in decision-making processes. This study paves the way for future innovations in the
field, heralding a new era of intelligent information systems that are more intuitive, responsive,
and user-centric.

