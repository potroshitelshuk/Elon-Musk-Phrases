**Collect Elon Musk phrases Dataset**

**Process description:**
1. Data{1 - 4} were collected from YouTube videos subtitles(not auto-generated). These transcripts were transformed and cleared from useless symbols to normal sentences.
	1. **Process:** Download transcripts in txt format by using free cloud service. Divide them on Elon Musk and speaker phrases if Elon Musk wasnot the only speaker.(Elon Musk - "Elon Musk:" in paragraph)
2. Data5 was collected using selenium. 
	1. **Process:** Open link, click 'read more' button, collect all paragraphs then divide them on Elon Musk and speaker phrases.(Speaker - "?" in the end of sentence and word count < 10)

**NEW!**

3. Data{6 & 7} were collected from podcasts with Joe Rogan and Elon Musk. 
	1. **Process:** Open link, collect all paragraphs, divide them into Elon Musk and speaker phrases.(Elon Musk - "Elon Musk:" in paragraph)
**NEW!**
4. Clear data(__const = 6__)
	1. Count the most frequently used words among all collected sentences and take first 80 words(**stop_words**).
	2. Delete all words from **stop_words** in result sentences.
	3. Filter result sentences by leaving only those who contain more than __const__ words.
5. Additional data clearing
	1. Replace "/" by "'".(Errors in transcripts)

**Used resources:**
1. Data1 - [link](https://www.youtube.com/watch?v=BDIRabVP24o)[ENGLISH SPEECH | ELON MUSK: Think Big & Dream Even Bigger]
2. Data2 - [link](https://www.youtube.com/watch?v=IgKWPdJWuBQ&t=21s)[Элон Маск: Элон Маск: Человек, создавший Tesla, SpaceX, SolarCity...]
3. Data3 - [link](https://www.youtube.com/watch?v=zIwLWfaAg-8)[Elon Musk: The future we're building -- and boring | TED]
4. Data4 - [link](https://www.youtube.com/watch?v=H7Uyfqi_TE8)[Making Humans a Multiplanetary Species]
5. Data5 - [link](https://www.englishspeecheschannel.com/english-speeches/elon-musk-speech/)[Elon Musk Speech: Future, A.I., and Mars]

**NEW!** 


6. Data6 - [link](https://www.rev.com/blog/transcripts/joe-rogan-elon-musk-podcast-transcript-may-7-2020)
7. Data7 - [link](https://sonix.ai/resources/full-transcript-joe-rogan-experience-elon-musk/)
Speech: Future, A.I., and Mars]


**Results:**
1. Collected around 5600 Elon Mask phrases, after clearing around 1100 phrases left.
2. Collected sentences contain not less than 7 words with a lot of scientific termins related to Elon Musk(Colonization, Mars, etc.).

**Test code**
1. To test this code you need to download and install:
	1. Google Chrome
	2. chromedriver
	3. selenium
2. Launch all cells in Parse_ElonMusk.ipynb to create Elon_Phrases.csv file with cleared Elon Musk phrases.

**More resources:**
1. Facebook/twitter
2. Other interviews
3. Books/articles
