## Amazon ML - Comprehend

**Input**

_Social media posts, emails, web Pages, documents and Phone Transcriptions_


**Comprehend**

_Automatically extract Jey Phrases, entities, sentiment, Lannuguage, and topics_


**Output**

Entities
Key Phrases
Language
Sentiment
Topics

_Extracted data and topics, with confidece scores_


### Comprehend User Case : Call Center

_Input_ -> Support Communications are generated across email, chat, social and phone calls

Sends input to  **S3** (Test data and call transcriptions are stored in an amazon S3 Data lake)

_Comprehend_ -> Processes the text to extract key phrases, entities, and sentiment for further analysis.


_Redshift_ --> Extracted data is analysed to identify what actions lead to the most positive customer outcomes.

_Output_ --> Insights are applied to customer service training to improve the rate of positive outcomes in less time,





