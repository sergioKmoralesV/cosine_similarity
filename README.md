# cosine similarity
Cosine similarity to compare two sentences

### Observations
* Before processing the data is important to **eliminate the special characters** to not to take them into consideration. That's why we use the regex expression `[,.!?]`. We use the library `re` that gives a better functionality than the normal replace of the type `string`.
* We manage **dataframes** from `pandas` in order to create vectors that take into consideration the unique words in each one of the sentences. It accelerates the manipulation of data.
* We use the library `numpy` so we can do the **dot** and **norm** operations that were necessary to calculate the **cosine similarity**.
* This program doesn't take into consideration the difference between the grammar specifications of _"it's"_ for example that could be either **_it is_** or **_it has_**. This would be an interesting upgrade if we want to really get to language processing.
* This program doesn't deletes the `'` because of it's relevance for the English language in the creation of words. The same as the`-` symbol.