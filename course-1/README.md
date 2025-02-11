# IBM - Generative AI for Data Engineers Specialization

## Course 1 - Generative AI: Introduction and Applications

I'll add two new columns with practical examples and relevant documentation/tools for each concept. This will help provide a more comprehensive understanding of these AI/ML terms.

| Term | Definition | Example | Tools/Documentation |
|------|------------|---------|-------------------|
| Data augmentation | A technique commonly used in machine learning and deep learning to increase the diversity and amount of training data. | For image data: rotating, flipping, or adding noise to existing images. For text: translating sentences to another language and back, or replacing words with synonyms. | TensorFlow Image Augmentation API (tensorflow.org/api_docs/python/tf/image), Albumentations library (albumentations.ai), NLTK for text augmentation |
| Deep learning | A subset of machine learning that focuses on training computers to perform tasks by learning from data. It uses artificial neural networks. | Image recognition system that can distinguish between different breeds of dogs by learning from millions of labeled dog photos. | TensorFlow (tensorflow.org), PyTorch (pytorch.org), Keras (keras.io) |
| Diffusion model | A type of generative model that is popularly used for generating high-quality samples and performing various tasks, including image synthesis. They are trained by gradually adding noise to an image and then learning to remove the noise. This process is called diffusion. | Stable Diffusion generating photorealistic images from text descriptions by gradually denoising random noise into coherent images. | Hugging Face Diffusers (huggingface.co/docs/diffusers), Stable Diffusion (stability.ai) |
| Discriminative AI | A type of artificial intelligence that distinguishes between different classes of data. | Spam filter that classifies emails as either spam or not spam based on their content. | Scikit-learn classification algorithms (scikit-learn.org/stable/supervised_learning.html) |
| Discriminative AI models | Models that identify and classify based on patterns they observe in training data. In general, they are used in prediction and classification tasks. | Credit card fraud detection system that identifies suspicious transactions based on historical fraud patterns. | TensorFlow Classification tutorials, scikit-learn classifiers |
| Foundation models | AI models with broad capabilities that can be adapted to create more specialized models or tools for specific use cases. | GPT-3 being fine-tuned for specific tasks like medical diagnosis assistance or legal document analysis. | Hugging Face Transformers (huggingface.co), OpenAI API documentation |
| Generative adversarial network (GAN) | A type of generative model that includes two neural networks: generator and discriminator. The generator is trained on vast data sets to create samples like text and images. The discriminator tries to distinguish whether the sample is real or fake. | StyleGAN generating photorealistic human faces that don't exist in reality. | TensorFlow GAN tutorial, PyTorch GAN implementation guides |
| Generative AI | A type of artificial intelligence that can create new content, such as text, images, audio, and video. | DALL-E creating original artwork based on text descriptions, or ChatGPT generating human-like text responses. | OpenAI API (openai.com), Google Cloud AI (cloud.google.com/ai) |
| Generative AI models | Models that can understand the context of input content to generate new content. In general, they are used for automated content creation and interactive communication. | AI music composer generating original melodies based on a specific genre or style. | MuseNet (openai.com/research/musenet), Anthropic Claude API |
| Generative pre-trained transformer (GPT) | A series of large language models developed by OpenAI. They are designed to understand language by leveraging a combination of two concepts: training and transformers. | GPT-4 engaging in complex dialogue, writing code, or analyzing text in multiple languages. | OpenAI API documentation (platform.openai.com/docs) |
| Large language models (LLMs) | A type of deep learning model trained on massive amounts of text data to learn the patterns and structures of language. They can perform language-related tasks, including text generation, translation, summarization, sentiment analysis, and more. | Claude translating technical documentation between languages while maintaining technical accuracy. | Hugging Face Transformers library, LangChain framework (langchain.com) |
| Machine learning | A type of artificial intelligence that focuses on creating algorithms and models that enable computers to learn and make predictions or decisions. It involves designing systems that can learn from training data. | Netflix recommendation system learning from user viewing habits to suggest new shows. | scikit-learn (scikit-learn.org), TensorFlow (tensorflow.org) |
| Natural language processing (NLP) | A branch of artificial intelligence that enables computers to understand, manipulate and generate human language (natural language). | Google Translate converting text between languages, or sentiment analysis of customer reviews. | NLTK (nltk.org), spaCy (spacy.io), Stanford NLP |
| Neural networks | Computational models inspired by the structure and functioning of the human brain. They are a fundamental component of deep learning and artificial intelligence. | Image recognition network that processes pixels through layers of neurons to identify objects in photographs. | TensorFlow Neural Network Guide, PyTorch Documentation |
| Prompt | Instructions or questions that are given to a generative AI model to generate new content. | "Write a poem about autumn in the style of Robert Frost" given to a language model. | OpenAI Prompt Engineering Guide, Anthropic Claude Documentation |
| Training data | Data (generally, large datasets that also have examples) used to teach a machine learning model. | ImageNet dataset containing millions of labeled images used to train computer vision models. | Kaggle Datasets (kaggle.com/datasets), Google Dataset Search |
| Transformers | A deep learning architecture that uses an encoder-decoder mechanism. Transformers can generate coherent and contextually relevant text. | BERT model understanding the context in search queries to provide more relevant results. | Hugging Face Transformers Documentation, "Attention Is All You Need" paper |
| Variational autoencoder (VAE) | A type of generative model that is basically a neural network model designed to learn the efficient representation of input data by encoding it into a smaller space and decoding back to the original space. | Face generation system that can create new faces by interpolating between learned facial features. | TensorFlow VAE Tutorial, PyTorch VAE Implementation Guide |

### Module 1

Generative AI models can generate new content based on the data they are trained on.

While discriminative AI mimics our analytical and predictive skills, Generative AI also mimics our creative skills.

The creative skills of Generative AI are built on the use of models, such as GANs, VAEs, and transformers. 

Foundation models in Generative AI can be adapted to create specialized models or tools tailored to specific use cases. 

Generative AI can create coherent and contextually relevant content and generate realistic, high-quality images, synthetic voices, new audio, and dynamic videos. 

Generative AI models can generate and complete code and synthesize new data to augment existing datasets.

Generative AI models can create highly realistic and complex virtual worlds, including avatars and digital personalities.

### Module 2

#### Workplace Impact

Generative AI strongly impacts businesses and industries across various domains, offering increased productivity and efficiency, an improved customer experience, and opportunities for growth and innovation. Research and advisory firms like Gartner and McKinsey have been tracking the impact of generative AI on business value and its economic potential for industries.

Gartner splits the business opportunities offered by generative AI into three categories:

Revenue opportunities by enabling enterprises to create new products and generate new revenue channels.

Cost and productivity opportunities by augmenting the workers' ability to draft and edit text, images, and other media. As generative AI becomes more prevalent in the workplace, employees will be distinguished by their ability to conceive, implement, and refine ideas, projects, processes, services, and collaborations in partnership with AI.

Risk opportunities through risk mitigation. Generative AI's ability to analyze and offer more insights into data, such as customer transactions and potentially flawed software code, improves the recognition of patterns and the speed at which potential risks to the enterprise can be identified.

Further, Gartner reflects on the industries that are most impacted by generative AI. Generative AI will affect the pharmaceutical, manufacturing, media, architecture, interior design, engineering, automotive, aerospace, defense, medical, electronics, and energy industries by augmenting core processes with AI models. It will impact marketing, design, corporate communications, training, and software engineering by augmenting the supporting processes that span many organizations.

Source: https://www.gartner.com/en/topics/generative-ai

A report from McKinsey: [The economic potential of generative AI: The next productivity frontier](https://www.mckinsey.com/capabilities/mckinsey-digital/our-insights/the-economic-potential-of-generative-ai-the-next-productivity-frontier#business-value)
McKinsey provides significant insight into the business value, industry impacts, and work and productivity implications achieved through generative AI in a report.
