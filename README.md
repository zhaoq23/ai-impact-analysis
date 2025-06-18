# Beyond Moravec's Paradox
## A Data-Driven Analysis of AI's Transformative Impact Across Industries
<img src="https://github.com/user-attachments/assets/0719938a-9ef0-41dd-90ea-1cc003016e06" width="400"/>

# Problem Statement
As AI rapidly transforms key industries, public and institutional perceptions play a crucial role in shaping its adoption and regulation. Yet, current understanding of how AI is portrayed in media—especially in terms of sentiment and topic focus—remains fragmented and anecdotal. This project addresses that gap by systematically analyzing over 160,000 AI-related articles using advanced NLP methods, revealing how sentiment varies across time, sectors, technologies, and regions. The goal is to provide actionable insights for policymakers, businesses, and researchers navigating the evolving AI landscape.

# Executive Summary
🔧 **Data Processing and Methodology**
- Initial dataset of ~200,000 articles was systematically cleaned and filtered to 167,763 relevant samples through a three-stage process incorporating linguistic analysis, feature engineering, and topic modeling
- Implemented a sophisticated sentiment analysis pipeline, starting with VADER analysis for baseline establishment, followed by data enhancement through manual annotation and BLOOM model labeling, then advanced model fine-tuning with RoBERTa and transformer ensemble architecture, ultimately achieving 82% macro-F1 score through class weight and learning rate optimization.
- Enhanced data quality through entity recognition (SpaCy, NER-BERT) and temporal analysis (LDA, BERTopic).
  
📊 **Sentiment Analysis Results**
- Final sentiment distribution showed balanced coverage: 56.1% neutral (88,344 samples), 42.0% positive (66,060 samples), and 1.9% negative (3,045 samples). This balanced distribution effectively separates genuine AI breakthroughs from general market speculation, ensuring more accurate analysis.
- Peak positive sentiment (60%) observed during May-July 2022, indicating significant AI breakthroughs
- Positive sentiments strongly associated with technological advancement and market growth
- Negative sentiments primarily linked to privacy concerns and data security issues

👉 Notes: My initial methodology aimed to combine manual annotation with ChatGPT-3.5 labeling (15,000 samples, $70 investment) for enhanced accuracy. However, due to a Colab system crash after a full day of training, resulting in data loss, which forced me to adapt to use the free BLOOM model for labeling. This limitation presents an opportunity for future improvements.

🏭 **Industry and Technology Impact**
- Finance, healthcare, and media sectors demonstrate highest AI automation potential while facing rigorous scrutiny
- Computer Vision dominates positive coverage (40-70%), while Natural Language Processing shows increasing negative sentiment trends
- Major cloud providers (Vertex AI, Azure AI, Google Cloud AI) lead both positive and negative coverage
- Executive positions (CTO, CEO) show increasing AI impact compared to operational roles

🌍 **Regional and Organizational Trends**
- Developed countries, particularly European nations, lead AI discussions and implementation
- Tech giants (Microsoft, Google) dominate positive coverage while facing increased scrutiny over AI monopoly concerns
- Regulatory bodies, especially in the EU, emerge prominently in negative coverage, indicating growing oversight focus

