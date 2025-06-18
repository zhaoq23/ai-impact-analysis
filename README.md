# Beyond Moravec's Paradox
## A Data-Driven Analysis of AI's Transformative Impact Across Industries
<img src="https://github.com/user-attachments/assets/0719938a-9ef0-41dd-90ea-1cc003016e06" width="400"/>

# Problem Statement
The rapid advancement of artificial intelligence (AI) technologies has triggered intense public discourse across media, regulatory, and corporate domains. However, the sentiment surrounding these discussions remains poorly understood, often obscured by hype, misinformation, or fragmented reporting. Despite the growing societal and economic implications of AI—particularly in sectors such as finance, healthcare, and media—there exists a significant gap in systematically mapping and interpreting the sentiment dynamics that shape public and institutional perceptions of AI.

This project was initiated to address this gap by building a robust, large-scale sentiment analysis pipeline tailored to AI-related content. By curating and analyzing over 160,000 high-quality media articles using advanced NLP techniques—including transformer-based models, entity recognition, and temporal-topic modeling—this research reveals how sentiment patterns correlate with technological breakthroughs, industry adoption, regulatory scrutiny, and regional trends.

Understanding these sentiment dynamics is critical for policymakers, industry leaders, and researchers. It enables more informed decision-making, helps forecast societal readiness and resistance, and sheds light on the nuanced narratives—both optimistic and cautionary—that accompany the rise of AI. The insights also lay the groundwork for early warning systems for policy backlash, guide responsible innovation, and identify areas where public trust needs to be strengthened.

# Executive Summary
## Data Processing and Methodology
- Initial dataset of ~200,000 articles was systematically cleaned and filtered to 167,763 relevant samples through a three-stage process incorporating linguistic analysis, feature engineering, and topic modeling
- Implemented a sophisticated sentiment analysis pipeline, starting with VADER analysis for baseline establishment, followed by data enhancement through manual annotation and BLOOM model labeling, then advanced model fine-tuning with RoBERTa and transformer ensemble architecture, ultimately achieving 82% macro-F1 score through class weight and learning rate optimization.
- Enhanced data quality through entity recognition (SpaCy, NER-BERT) and temporal analysis (LDA, BERTopic).
  
## Sentiment Analysis Results
- Final sentiment distribution showed balanced coverage: 56.1% neutral (88,344 samples), 42.0% positive (66,060 samples), and 1.9% negative (3,045 samples). This balanced distribution effectively separates genuine AI breakthroughs from general market speculation, ensuring more accurate analysis.
- Peak positive sentiment (60%) observed during May-July 2022, indicating significant AI breakthroughs
- Positive sentiments strongly associated with technological advancement and market growth
- Negative sentiments primarily linked to privacy concerns and data security issues

👉 Notes: My initial methodology aimed to combine manual annotation with ChatGPT-3.5 labeling (15,000 samples, $70 investment) for enhanced accuracy. However, due to a Colab system crash after a full day of training, resulting in data loss, which forced me to adapt to use the free BLOOM model for labeling. This limitation presents an opportunity for future improvements.

## Industry and Technology Impact
- Finance, healthcare, and media sectors demonstrate highest AI automation potential while facing rigorous scrutiny
- Computer Vision dominates positive coverage (40-70%), while Natural Language Processing shows increasing negative sentiment trends
- Major cloud providers (Vertex AI, Azure AI, Google Cloud AI) lead both positive and negative coverage
- Executive positions (CTO, CEO) show increasing AI impact compared to operational roles

## Regional and Organizational Trends
- Developed countries, particularly European nations, lead AI discussions and implementation
- Tech giants (Microsoft, Google) dominate positive coverage while facing increased scrutiny over AI monopoly concerns
- Regulatory bodies, especially in the EU, emerge prominently in negative coverage, indicating growing oversight focus

