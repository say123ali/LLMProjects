# LLMProjects

𝐑𝐞𝐭𝐫𝐢𝐞𝐯𝐚𝐥-𝐀𝐮𝐠𝐦𝐞𝐧𝐭𝐞𝐝 𝐆𝐞𝐧𝐞𝐫𝐚𝐭𝐢𝐨𝐧 (𝐑𝐀𝐆) 𝐔𝐬𝐢𝐧𝐠 𝐋𝐚𝐧𝐠𝐂𝐡𝐚𝐢𝐧
𝐂𝐡𝐮𝐧𝐤𝐢𝐧𝐠 𝐝𝐨𝐜𝐮𝐦𝐞𝐧𝐭𝐬 𝐚𝐧𝐝 𝐄𝐦𝐛𝐞𝐝𝐝𝐢𝐧𝐠


✳ 𝐒𝐩𝐥𝐢𝐭𝐭𝐢𝐧𝐠 𝐝𝐨𝐜𝐮𝐦𝐞𝐧𝐭𝐬: 
4 methods are detailed to chunk a text:

*   CharacterTextSplitter
*   RecursiveCharacterTextSplitter
*   TokenTextSplitter
*   HTMLHeaderTextSplitter

The last one is a context aware splitter, to chunk HTML, to extract data from a website by respecting the architecture of the html. We'll have better results when applying contextual retrieving.

✳ 𝐄𝐦𝐛𝐞𝐝𝐝𝐢𝐧𝐠 𝐚𝐧𝐝 𝐕𝐞𝐜𝐭𝐨𝐫𝐞𝐬𝐭𝐨𝐫𝐞𝐬:
Then I used the Embedding model with LangChain and exposed another way to do it with openai directly. LangChain is using the same model under the hood ‘𝘵𝘦𝘹𝘵-𝘦𝘮𝘣𝘦𝘥𝘥𝘪𝘯𝘨-𝘢𝘥𝘢-002'.

Simple article, explaining how to use it with openai: https://lnkd.in/gF6p38Ww

Then used chroma to store embedding vectors (Explained in the short course from LangChain and deeplearning.ai), and apply Similarity search to get the most related chunks to a given question.


✳𝐒𝐢𝐦𝐢𝐥𝐚𝐫𝐢𝐭𝐲 𝐬𝐞𝐚𝐫𝐜𝐡
2 methods to apply and get the score of the relatedness:
▪ similarity_search_with_relevance_scores
▪ similarity_search_with_score
