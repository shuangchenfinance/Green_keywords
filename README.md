# List of green keywords

Shuang Chen creates this dataset in her following paper:	

Chen, Shuang, Green Investors and Green Transition Efforts: Talk the Talk or Walk the Walk? (June 21, 2024). Available at SSRN: https://ssrn.com/abstract=4254894 or http://dx.doi.org/10.2139/ssrn.4254894

To evaluate whether the context of a job position is eco-friendly, the most transparent and fundamental method is to summarize a list of keywords whose appearances signify the eco-friendly context. The list of green keywords starts from Wikipedia words and phrases under the tag “List of environmental organisations topics” and “List of environmental issues”. Each word or phrase on these two web pages has a dedicated Wikipedia page. On the one hand, they provide a comprehensive scope of important environmental topics. On the other hand, these words or phrases express environmental concerns and signify the word user’s supportive attitude towards environmental responsibility.

I remove words that are often used in contexts beyond the environment, such as “Population growth” and “Agricultural subsidy”, and words that are related to the environment but are too general to signify the word user’s attitude towards the environment, such as “Mining” and “Coal”. There are still 294 seed words or phrases.

For each seed word or bigram of phrases, I select the top 40 closest synonyms with a word embedding model (details in Appendix B in the working paper) and remove those that do not express environmental concerns or support based on Google search results. There are 764 green keywords in total in the combination of seed words and synonyms. Table A3 in the working paper's appendix lists the top 120 most frequent green keywords among job postings belonging to context-dependent green occupations.
