# List of green keywords

This dataset is created by Shuang Chen in her following paper:	

Chen, Shuang, Green Investors and Green Transition Efforts: Talk the Talk or Walk the Walk? (June 21, 2024). Available at SSRN: https://ssrn.com/abstract=4254894 or http://dx.doi.org/10.2139/ssrn.4254894

To evaluate whether the context of a job position is eco-friendly, the most transparent and fundamental method is to summarize a list of keywords whose appearances signify an eco-friendly context.

If a job posting explicitly mentions environmentally friendly practices or criticizes non-environmentally friendly practices, it strongly indicates that the position has an environmentally friendly orientation. Employers may highlight these aspects to attract candidates who are aligned with their environmental values and goals. For example, when a job posting mentions "oxidizer scrubber," it suggests that the position involves work related to air pollution control or environmental compliance. While the phrase itself does not explicitly state that the position is environmentally friendly, the use of these technologies is generally associated with efforts to reduce environmental impact and comply with environmental regulations. 

However, there are some controversial areas, such as nuclear energy, transition fuels, and natural gas, regarding whether they are conducive to a better environment. To maintain a strict definition of an eco-friendly context, these are not included in the green keywords list.

I start compiling the green keyword list by generating a small list of seed words from Wikipedia entries and phrases under the tag "List of environmental organisations topics" and "List of environmental issues". Each word or phrase on these two web pages has a dedicated Wikipedia page. On the one hand, they provide a comprehensive scope of important environmental topics. On the other hand, these words or phrases express environmental concerns and signify the user's supportive attitude towards environmental responsibility. I remove seed words that are often used in contexts beyond the environment, such as "Population growth" and "Agricultural subsidy", and words that are related to the environment but are too general to signify the word user's attitude towards the environment, such as ``Mining" and ``Coal". This leaves 294 seed words or phrases in the seed word list.

For each seed word or phrase, I use a word embedding model (details in Appendix B) to select the top 40 closest synonyms. For these synonyms and seed words, I then filter out those whose Google search results do not relate to supporting environmentally friendly practices or criticizing non-environmentally friendly practices. Additionally, I remove words or phrases that appear less than ten times in the analyzed job postings, as their infrequency prevents a reliable evaluation of their effectiveness in assessing the eco-friendly context of job postings. 

The final green keyword list contains 742 keywords. List of green keywords.xlsx contains the green keywords among job postings with context-dependent green occupations.  If any of these keywords appear in a job posting, the posting is considered to have an eco-friendly context. By the end of this step, we can determine whether any job posting belongs to a walk-relevant, talk-relevant, or neither occupation, and whether the job context is eco-friendly. A job posting in a walk-relevant occupation and an eco-friendly context is classified as a walk-relevant job posting. Similarly, a job posting in a talk-relevant occupation and an eco-friendly context is classified as a talk-relevant job posting.
