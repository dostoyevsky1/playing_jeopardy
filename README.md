# playing_jeopardy
Analysis of a subset of Jeopardy questions data from http://www.j-archive.com/
	
	Currently contains a text analysis of questions and answers to see if answer terms are contained in question; percentage of term usage overlap between new and old questions; chi-squared test for independence between word usage and high and low value questions;

Potential pathways for further analysis:

    Find a better way to eliminate non-informative words than just removing words that are less than 6 characters long. Some ideas:
        Manually create a list of words to remove, like the, than, etc.
        Find a list of stopwords to remove.
        Remove words that occur in more than a certain percentage (like 5%) of questions.
    Perform the chi-squared test across more terms to see what terms have larger differences. This is hard to do currently because the code is slow, but here are some ideas:
        Use the apply method to make the code that calculates frequencies more efficient.
        Only select terms that have high frequencies across the dataset, and ignore the others.
    Look more into the Category column and see if any interesting analysis can be done with it. Some ideas:
        See which categories appear the most often.
        Find the probability of each category appearing in each round.
    Use the whole Jeopardy dataset (available here) instead of the subset we used in this mission.
    Use phrases instead of single words when seeing if there's overlap between questions. Single words don't capture the whole context of the question well.

