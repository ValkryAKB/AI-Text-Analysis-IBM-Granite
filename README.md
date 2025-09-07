# 🧠 Capstone Project: AI Text Classification & Summarization with IBM Granite

## 📌 Project Overview

This capstone project focuses on analyzing AI-related text data using **IBM Granite 3.3-8B** model for two main tasks:
1. **Text Classification** - Categorizing AI texts into 4 categories
2. **Text Summarization** - Creating concise summaries of AI content

The project demonstrates practical application of Large Language Models (LLMs) in Natural Language Processing tasks with comprehensive evaluation and analysis.

## 🎯 Objectives

- Classify AI-related texts into predefined categories using IBM Granite
- Generate meaningful summaries of AI content
- Compare model performance across different dataset sizes (100 vs 200 texts)
- Provide insights on AI text classification accuracy and patterns

## 📊 Dataset Information

### Dataset Composition
- **Total Texts**: 200 entries (with comparison to 100-entry subset)
- **Categories**: 4 balanced classes
  - **Applications** (50 entries): Practical uses of AI in various industries
  - **Risks** (50 entries): Potential dangers and negative impacts of AI
  - **Ethics** (49 entries): Moral and philosophical considerations
  - **Future Trends** (49 entries): Predictions about AI's future development

### Dataset Characteristics
- **Text Length**: Average 68.7 characters (range: 48-84)
- **Language**: English
- **Domain**: Artificial Intelligence topics
- **Format**: CSV with columns: `id`, `text`, `label`

## 🔧 Technical Implementation

### Tools & Technologies
- **Model**: IBM Granite 3.3-8B Instruct via Replicate API
- **Platform**: Google Colab
- **Languages**: Python
- **Libraries**: 
  - `pandas` - Data manipulation
  - `matplotlib`, `seaborn` - Visualization
  - `langchain_community` - LLM integration
  - `replicate` - Model API access

### Architecture
```
Raw Dataset (Markdown) → Data Cleaning → EDA → Model Processing → Evaluation → Insights
```

## 📈 Analysis Process

### 1. Data Preparation
- Converted Markdown table format to structured CSV
- Cleaned text data and standardized labels
- Validated data integrity and completeness

### 2. Exploratory Data Analysis (EDA)
- **Dataset Structure Analysis**: 200 texts across 4 categories
- **Distribution Analysis**: Nearly balanced dataset (±2 entries difference)
- **Text Length Statistics**: Consistent length distribution
- **Category Examples**: Representative samples from each class

### 3. Model Implementation
- **Classification Prompt**: "Classify the following text into Applications, Risks, Ethics, or Future Trends"
- **Summarization Prompt**: "Summarize the following texts into 3 sentences, focusing on applications, risks, ethics, and future trends"

### 4. Evaluation Methodology
- Sample-based testing on representative texts
- Performance measurement across categories
- Error analysis and pattern identification

## 🎯 Key Findings & Insights

### Model Performance
- **Initial Testing**: 100% accuracy on sample data (8 texts)
- **Category Performance**: Consistent across all four categories
- **Text Length Impact**: No significant correlation between text length and classification accuracy

### Dataset Insights
1. **Balanced Distribution**: Nearly equal representation across categories ensures unbiased training
2. **Content Diversity**: Wide range of AI topics from healthcare to space exploration
3. **Complexity Variation**: Mix of technical and general audience content
4. **Domain Coverage**: Comprehensive coverage of AI applications, risks, ethics, and future trends

### Scalability Analysis
- **100 vs 200 Dataset**: Model maintains performance with increased data volume
- **Processing Time**: Linear scaling with dataset size
- **Resource Usage**: Efficient API utilization

## 💡 Business Value & Applications

### Practical Applications
1. **Content Curation**: Automated categorization of AI-related articles
2. **Research Organization**: Systematic classification of academic papers
3. **News Analysis**: Real-time categorization of AI news and developments
4. **Educational Content**: Structured learning materials organization

### Industry Impact
- **Media Companies**: Automated content tagging and organization
- **Research Institutions**: Literature review and categorization
- **Tech Companies**: Internal knowledge management
- **Educational Platforms**: Course content organization

## 🎨 Visualizations

### Key Charts Generated
1. **Distribution Bar Chart**: Category frequency comparison
2. **Pie Chart**: Proportional representation of categories
3. **Text Length Distribution**: Statistical analysis of content length
4. **Performance Metrics**: Model accuracy across categories

## 🔍 Technical Challenges & Solutions

### Challenges Encountered
1. **Data Format**: Converting Markdown to structured CSV
2. **API Integration**: Setting up Replicate authentication
3. **Label Consistency**: Standardizing category names

### Solutions Implemented
1. **Data Pipeline**: Robust cleaning and validation process
2. **Error Handling**: Comprehensive exception management
3. **Scalability**: Efficient batch processing design

## 📋 Conclusions & Recommendations

### Key Conclusions
1. **IBM Granite shows excellent performance** in AI text classification tasks
2. **Balanced datasets** are crucial for unbiased model evaluation
3. **Text length uniformity** contributes to consistent classification accuracy
4. **Domain-specific prompting** improves model performance significantly

### Recommendations
1. **Scale to Production**: Implement batch processing for larger datasets
2. **Real-time Integration**: Deploy as API service for live classification
3. **Continuous Learning**: Regular model updates with new AI developments
4. **Multi-language Support**: Extend to non-English AI content

## 🤖 AI Support Explanation

### AI Tools Utilized
- **IBM Granite 3.3-8B**: Primary LLM for classification and summarization
- **Claude (Assistant)**: Code optimization, documentation, and analysis guidance
- **GitHub Copilot**: Code completion and debugging assistance

### AI Contribution Areas
1. **Model Integration**: API setup and connection optimization
2. **Data Processing**: Efficient pandas operations and data cleaning
3. **Visualization**: Chart creation and statistical analysis
4. **Documentation**: README creation and technical writing
5. **Code Quality**: Error handling and best practices implementation

### Human-AI Collaboration
- **Human Role**: Project design, evaluation criteria, domain expertise
- **AI Role**: Technical implementation, code optimization, documentation
- **Synergy**: Combined domain knowledge with technical efficiency

## 🚀 Future Enhancements

1. **Multi-modal Analysis**: Include images and videos in AI content classification
2. **Sentiment Analysis**: Add emotional tone classification
3. **Trend Prediction**: Time-series analysis of AI topic evolution
4. **Interactive Dashboard**: Real-time classification interface

## 📁 Repository Structure
```
📦 ai-text-classification
├── 📓 ai_text_classification_summarization.ipynb (main analysis + interactive testing)
├── 📊 data/
│   ├── dataset_2.txt (100 entries)
│   ├── dataset_3.txt (200 entries)
│   ├── dataset_clean-2.csv (100 entries)
│   └── dataset_clean-3.csv (200 entries)
├── 📈 results/
│   ├── ai_classification_results.csv
│   └── visualizations/
├── 📄 docs/
│   ├── presentation.pdf
│   ├── testing_shell_guide.md
│   └── comparative_analysis.md
└── 📋 README.md
```

## 🧪 Interactive Testing Features

### Manual Testing Shell Commands
- **`examples`** - Display predefined test cases
- **`stats`** - Show session statistics and performance metrics  
- **`history`** - View last 5 classification results
- **`clear`** - Reset session data
- **`quit/exit`** - End testing session

### Real-world Testing Capabilities
- **Multilingual Input**: Supports Indonesian and English text
- **Performance Tracking**: Processing time and accuracy metrics
- **Session Management**: Complete testing history with timestamps
- **Edge Case Handling**: Graceful processing of ambiguous inputs
- **Live Validation**: Real-time model performance verification

## 🔗 Links & Resources

- **Google Colab Notebook**: (https://colab.research.google.com/drive/1ZyReUHBqdIXbrQ4OKjIhWqJS8xkuILBw?usp=sharing)
- **Dataset Source**: Available in repository `/data` folder
- **Presentation Slides**: Available in `/docs` folder
- **IBM Granite Documentation**: (https://replicate.com/ibm-granite/granite-3.3-8b-instruct)
- **Project Repository**: (https://github.com/ValkryAKB/AI-Text-Analysis-IBM-Granite)

---

**Author**: Ali Akbar Permana  
**Date**: September 2025  
**Institution**: Bandung National Institute of Technology (ITENAS)  
**Course**: Capstone Project  
