# Assignment Improvements for JOUR405

## General Observations

The assignments follow a clear progression from basic R skills through descriptive statistics, inferential statistics, and regression. They use journalism-relevant datasets and scenarios, which helps students connect statistical concepts to their future work.

## Specific Improvements by Assignment

### HW1: R Basics

**Current strengths:**
- Introduces R fundamentals with clear, incremental steps
- Links to R4DS book for reference

**Suggested improvements:**

1. **Add a data inspection task:** After loading students.csv, have them answer specific questions about the data:
   - How many rows are in this dataset?
   - What are the column names?
   - Pick one column and describe what values it contains.

2. **Add a troubleshooting section:** Include one intentionally problematic code block (like missing a parenthesis) and ask students to fix it. This builds debugging skills early.

3. **Make the connection explicit:** Add a brief explanation of why journalists need to write code rather than just using Excel. Keep it practical: "You'll work with datasets too large for Excel" or "Code lets you document every step of your analysis."

### HW7: M&Ms

**Current issue:** This assignment is very sparse - just task titles with no scaffolding.

**Suggested improvements:**

1. **Add context:** Start with a brief paragraph explaining why random sampling matters for journalism (polling, auditing, data verification).

2. **Provide starter code blocks:** Students at this stage still need structure. Include empty code blocks under each task.

3. **Add intermediate questions:**
   - Task 3: "How many rows did you get? Run this code block three times. Did you get the same rows each time?"
   - Task 4-5: "Which measure (blue or white) did you choose? Why might the results differ between the two?"

4. **Make Task 7 more specific:** Replace "Write a few sentences" with targeted questions:
   - "How close was your sample mean to the population mean?"
   - "What does this tell you about whether a small sample can represent a larger population?"
   - "If you were sampling voters for a poll, what would this exercise suggest about sample size?"

### HW9: Test Scores

**Current strengths:**
- Excellent real-world scenario (superintendent's claim)
- Good progression through hypothesis testing
- Includes both statistical work and journalistic interpretation

**Suggested improvements:**

1. **Reflection Question 1:** Too open-ended. Break it into steps:
   - "Calculate the mean of the new scores in your head (or on paper). Is it higher than 72.6?"
   - "Now look at the individual scores. Are they ALL higher than 72.6, or just some of them?"
   - "Based on this, would you say scores improved? What makes you confident or uncertain?"

2. **Task 4 hypotheses:** Provide a template:
   - Null: "The new reading program has/has not [your answer] changed reading scores"
   - Alternative: "The new reading program has/has not [your answer] changed reading scores"

3. **Add a critical thinking question:** After showing the p-value result, ask: "The p-value tells you whether the difference is statistically significant. What information do you NOT have from this test? (Hint: Think about why scores might have changed besides the program.)"

4. **Reflection Question 6:** Good question, but frame it as: "List three specific metrics beyond test scores that you would want to examine before publishing a story claiming the program works."

### HW10: Car Thefts Significance

**Current strengths:**
- Excellent use of visualization to show confidence intervals
- Good progression from description to inference
- Real police data

**Suggested improvements:**

1. **Task 3:** Make the question more specific:
   - "Looking at the line chart, does the line go up, go down, or stay mostly flat?"
   - "Do you see any sudden jumps or drops, or does it change gradually?"
   - "Based on this, write one sentence describing the trend."

2. **Task 6:** Add a question before the headline request:
   - "Looking at the chart, do most months fall inside the red shaded area (confidence interval) or outside it?"
   - "What does this tell you about whether the monthly variation is normal or unusual?"

3. **Task 7:** Before the t-test, add a prediction task:
   - "Before running the t-test, look at the two halves of data. Which half appears to have higher car thefts?"
   - "Do you think this difference will be statistically significant? Why or why not?"
   - Then run the test and compare their prediction to the result.

4. **Add editor questions:** After Task 8, include: "Your editor asks: 'Could this decrease be explained by something other than an actual reduction in crime, like changes in how crimes are reported?' How would you respond?"

### HW11: Survey Weights

**Current strengths:**
- Important topic for journalists covering polls
- Clear comparison of weighted vs. unweighted results
- Good visualization

**Suggested improvements:**

1. **Task 2:** Excellent reflection question. Add one more:
   - "Why might college-educated people be more likely to respond to surveys than people with less education?"

2. **Task 10:** The visualization question is vague. Make it specific:
   - "For each education level, estimate the difference in percentage points between weighted and unweighted by looking at the bars. Which group shows the biggest difference?"
   - "Does the bar chart make it easier to see these differences than the table did? Why or why not?"

3. **Add a real-world application:** After Task 11, add: "Find a news article that cites polling data. Does the article mention whether the poll was weighted? Should it?"

### HW17: Multiple Regression

**Current strengths:**
- Introduces complex statistical concept
- Uses real Maryland voter turnout data
- Includes model comparison

**Suggested improvements:**

1. **Introduction:** Add one concrete example before diving in:
   - "Simple regression asks: 'Does income predict voter turnout?' Multiple regression asks: 'When we account for income, education, AND age together, which factors matter most?'"

2. **Task 1:** The questions are good, but add a checklist:
   - "Before answering, find these specific values in the correlation matrix:"
   - "Correlation between turnout and income: ___"
   - "Correlation between turnout and education: ___"
   - "Strongest positive correlation with turnout: ___"

3. **Task 2:** Add scaffolding for interpreting coefficients:
   - "For each coefficient, answer:"
   - "Is it positive or negative?"
   - "Is the p-value less than 0.05?"
   - "In one sentence, what does this coefficient suggest about the relationship between this variable and turnout?"

4. **Task 3:** Students often struggle here. Add guidance:
   - "Model 2 suggestion: Remove the variables with the highest p-values from the initial model"
   - "Model 3 suggestion: Keep only variables with p-values below 0.05"
   - "Model 4 suggestion: Try a model with just one or two variables you think are most important"

5. **Task 4:** This is too vague. Replace with:
   - "Write a paragraph for a news story that includes:"
   - "One finding about which factor most strongly predicts voter turnout"
   - "One example using real numbers from your model"
   - "One limitation or caveat about what your analysis can and cannot prove"

## Activity Improvements

### Wordle Activity

**Current strengths:**
- Excellent, comprehensive probability exercise
- Clear code with good explanations
- Shows probability concepts in action

**Suggested improvements:**

1. **Add checkpoints:** After each major section, add a reflection question:
   - After initial probability: "Express this probability as 'X in Y' instead of a decimal. Which is easier to understand?"
   - After comparing strategies: "In your own words, why did the strategic guess work better?"

2. **Simplify the conclusion:** The current conclusion uses technical terms (Bayes' theorem, information theory). Rewrite for journalism students:
   - "This exercise shows three key ideas:"
   - "1. Starting probability matters: With 200 options, random guessing gives you 1 in 200 odds"
   - "2. Information narrows possibilities: Each guess with feedback eliminates options"
   - "3. Strategy beats luck: Guesses using common letters eliminate more possibilities faster"

3. **Add a journalism connection:** End with: "How does this relate to reporting? When you investigate a story, you start with many possible explanations. Each piece of evidence you gather eliminates some possibilities and makes others more likely. Like Wordle, smart choices about what to investigate first get you to the truth faster."

### Sampling Activity

**Current issue:** Only task titles, no explanation or scaffolding.

**Suggested improvements:**

1. **Add an introduction:**
   - "Journalists constantly work with samples. You can't interview every voter, so you sample voters in a poll. You can't examine every government contract, so you sample contracts for investigation. This exercise shows how samples relate to populations."

2. **Add code structure:** Provide the outline:
   - Task 2: "Use read_csv() with this URL: [provide URL]"
   - Task 3: "Use the slice_sample() function with n = 100"

3. **Make Task 6 more concrete:**
   - "Calculate the difference between the sample mean and population mean"
   - "Now take a sample of only 10 rows. Calculate its mean. How different is it from the population mean?"
   - "Which sample (n=100 or n=10) was closer to the true population mean?"
   - "What does this tell you about sample size in polls?"

### Basketball Heights Activity

**Current strengths:**
- Real sports data
- Clear hypothesis testing example
- Two different calculation methods

**Suggested improvements:**

1. **Add setup:** The file jumps straight to code. Add 2-3 sentences:
   - "Statistical significance testing helps journalists determine whether a difference is real or just random chance. This exercise tests whether Maryland's women's basketball team is shorter than other Division I teams."

2. **After the hypotheses:** Add: "These hypotheses help us avoid bias. We state what we're testing before we see the results, then let the data tell us what's true."

3. **Explain the two methods:** Add a paragraph between the two examples:
   - "The first test used individual player heights. But sometimes you only have summary statistics (mean, standard deviation) without the raw data. The second example shows how to test significance using only those summaries."

4. **Add a journalism connection:** "You might encounter both situations in reporting. A school district might give you individual student test scores (raw data) or just the average score by school (summary statistics). Both can be analyzed, but the approach differs."

## New Activities and Homework: Probability and LLMs

### Activity: Text Prediction and Probability

**Learning goal:** Understand how probability underlies language model predictions

**Description:**
Students explore how LLMs use probability to predict the next word in a sequence.

**Tasks:**

1. **Manual prediction exercise:**
   - "Complete this sentence: 'The President announced ___'"
   - "List 5 possible next words"
   - "Which word do you think is most likely? Why?"

2. **Frequency analysis:**
   - Provide a dataset of news article sentences (100-200 sentences)
   - "Count how many times each word follows 'announced' in this dataset"
   - "Calculate the probability of each word: count ÷ total"
   - "Compare your probabilities to your predictions. Were the most common words the ones you guessed?"

3. **Simple language model:**
   ```r
   # Calculate word frequencies after target word
   sentences <- c("[provide 50 example sentences]")

   # Find all words that follow "announced"
   # Calculate probabilities
   # Display top 10 most likely next words
   ```

4. **Reflection:**
   - "How is this similar to what ChatGPT or other LLMs do?"
   - "What's different? (Hint: LLMs look at more than just the previous word)"
   - "Why might an LLM sometimes 'hallucinate' or make up facts?"

### Activity: Temperature and Randomness

**Learning goal:** Understand how temperature settings affect LLM outputs

**Description:**
Students experiment with different "temperature" values to see how they affect randomness in predictions.

**Tasks:**

1. **Simulate low temperature (deterministic):**
   ```r
   # Given probabilities for next word:
   words <- c("taxes", "policy", "legislation", "plans", "reform")
   probabilities <- c(0.35, 0.25, 0.20, 0.15, 0.05)

   # Low temperature: Always pick highest probability
   # What word gets chosen?
   ```

2. **Simulate high temperature (random):**
   ```r
   # High temperature: Sample based on probabilities
   # Run this 100 times, count outcomes
   # Create bar chart showing distribution
   ```

3. **Compare outputs:**
   - "With low temperature, what word appeared most often?"
   - "With high temperature, did lower-probability words appear sometimes?"
   - "When might you want low vs. high temperature in a real LLM?"

4. **Journalism application:**
   - "If you're using an LLM to help draft article text, would you want high or low temperature? Why?"
   - "If you're using an LLM to brainstorm story ideas, would you want high or low temperature? Why?"
   - "What risks come with each approach?"

### Homework: Understanding LLM Uncertainty

**Learning goal:** Students learn to evaluate LLM outputs probabilistically and understand confidence

**Scenario:**
"You're fact-checking claims made by an AI chatbot in its responses. Understanding probability helps you evaluate when an LLM is confident vs. uncertain."

**Tasks:**

1. **Load a dataset of LLM responses:**
   Provide a CSV with:
   - question
   - llm_response
   - actual_answer
   - confidence_score (0-1)

2. **Analyze confidence scores:**
   ```r
   # Calculate mean confidence for correct vs. incorrect answers
   # Create histogram of confidence scores
   # What pattern do you see?
   ```

3. **Threshold analysis:**
   - "If you only trusted responses with confidence > 0.8, how many would you trust?"
   - "Of those high-confidence responses, what percentage were actually correct?"
   - "What about low-confidence responses (< 0.5)? Were they always wrong?"

4. **Create a decision rule:**
   - "Based on your analysis, what confidence threshold would you use before trusting an LLM response in your reporting?"
   - "Even above that threshold, what additional verification would you do?"

5. **Reflection:**
   - "LLMs don't always provide confidence scores. When they don't, what signs in the response might indicate uncertainty?"
   - "List three specific ways you would verify a factual claim from an LLM before publishing it."

### Homework: Bias in Training Data

**Learning goal:** Understand how probability distributions in training data affect LLM outputs

**Scenario:**
"An LLM trained primarily on historical news articles tends to associate certain professions with certain demographics. This homework explores how training data frequencies become output probabilities."

**Tasks:**

1. **Load profession-gender dataset:**
   Dataset showing profession mentions with pronouns from historical news (1980-2020):
   ```
   profession, he_count, she_count, total_count
   doctor, 8500, 1500, 10000
   nurse, 800, 9200, 10000
   CEO, 8800, 1200, 10000
   teacher, 2200, 7800, 10000
   engineer, 8300, 1700, 10000
   ```

2. **Calculate probabilities:**
   ```r
   # For each profession, calculate:
   # P(he|profession) and P(she|profession)
   # Create visualization showing these probabilities
   ```

3. **Compare to current demographics:**
   Provide current actual percentages of each profession by gender:
   ```r
   # Calculate difference between historical probability and current reality
   # Which professions show the biggest gaps?
   ```

4. **Test an actual LLM:**
   - "Ask ChatGPT or similar to complete sentences like:"
   - "'The doctor said he/she...'"
   - "'The nurse said he/she...'"
   - "Run each prompt 10 times. What pronouns appear most often?"
   - "Do the results match the historical training data probabilities?"

5. **Reflection:**
   - "How might these biased probabilities affect LLM outputs in journalism contexts?"
   - "Give one specific example of a news article where relying on an LLM might introduce gender bias"
   - "What steps can journalists take to avoid amplifying these biases?"

### Activity: Token Probability Chains

**Learning goal:** Understand how LLMs build responses token by token using conditional probability

**Description:**
Students manually calculate probability chains to understand how LLMs generate text.

**Tasks:**

1. **Single token prediction:**
   Provide a probability table:
   ```
   Given: "The senator announced"
   Next token probabilities:
   - "new" (0.30)
   - "his" (0.25)
   - "her" (0.20)
   - "the" (0.15)
   - "plans" (0.10)
   ```
   "If we always choose the highest probability, what comes next?"

2. **Two-token sequence:**
   "Now we have: 'The senator announced new'"
   Next token probabilities:
   ```
   - "legislation" (0.40)
   - "policy" (0.30)
   - "rules" (0.20)
   - "laws" (0.10)
   ```
   "Calculate the probability of the full sequence 'announced new legislation'"
   "Hint: Multiply the probabilities: P(new|announced) × P(legislation|new)"

3. **Multiple possible paths:**
   ```r
   # Calculate probabilities for 5 different sentence completions
   # Which has the highest total probability?
   # Which would an LLM most likely generate?
   ```

4. **Understanding "hallucinations":**
   - "Even low-probability sequences can occur. Calculate the probability of: 'The senator announced purple elephants'"
   - "If each token has probability 0.01, what's the sequence probability?"
   - "LLMs sample from probability distributions. Can you see how rare but grammatical nonsense can occur?"

5. **Journalism implications:**
   - "When an LLM makes a factually incorrect but grammatical statement, is it 'lying' or following probability?"
   - "Why does this distinction matter for how journalists should use these tools?"

### Activity: Context Windows and Probability

**Learning goal:** Understand how context length affects prediction accuracy

**Description:**
Students see how more context improves predictions.

**Tasks:**

1. **Predict with minimal context:**
   - Given: "The"
   - "List 10 possible next words with estimated probabilities"
   - "Why is this difficult?"

2. **Predict with more context:**
   - Given: "The mayor announced plans to increase"
   - "List 10 possible next words with estimated probabilities"
   - "Are you more confident now? Why?"

3. **Analyze a dataset:**
   Provide sentence completion data with varying context lengths:
   ```r
   # Dataset: context_length, prediction_accuracy
   # Create scatter plot: context length vs. accuracy
   # Calculate correlation
   # What does this tell you?
   ```

4. **LLM context window limits:**
   - "Most LLMs have context limits (4K, 8K, 32K tokens). One token ≈ 0.75 words."
   - "Calculate: How many words fit in an 8K token context?"
   - "You're fact-checking a 50-page document (≈15,000 words). Will it fit in the context?"
   - "If not, what strategies could you use?"

5. **Reflection:**
   - "Why might an LLM give different answers to the same question when you provide more background information?"
   - "When using an LLM for research, what context would you include to get better results?"

## Implementation Recommendations

**Sequencing:**
1. Introduce probability basics with existing activities (sampling, Wordle)
2. Add "Text Prediction and Probability" activity
3. Add "Token Probability Chains" activity
4. Assign "Understanding LLM Uncertainty" homework
5. Add "Temperature and Randomness" activity
6. Assign "Bias in Training Data" homework
7. Add "Context Windows and Probability" activity

**Integration with existing content:**
- These activities fit naturally after probability and before/during regression
- They reinforce probability concepts while adding modern relevance
- They prepare students to use LLMs critically in their work

**Practical tips:**
- Use real LLM outputs in examples
- Have students test concepts with actual tools (ChatGPT, Claude)
- Always connect probability concepts to journalistic judgment
- Emphasize verification and skepticism

## Key Principles for All Improvements

1. **Break problems into steps:** Don't ask "analyze this" - ask specific questions that build toward analysis

2. **Provide scaffolding:** Students need structure, especially early in the semester

3. **Use concrete numbers:** "Calculate the difference" is better than "compare the statistics"

4. **Connect to journalism:** Every statistical concept should have a clear application to reporting

5. **Build debugging skills:** Include troubleshooting and error interpretation

6. **Make assumptions explicit:** When students need to fill in REPLACE_ME, tell them where to find the value

7. **Ask for predictions:** Before showing results, ask what students expect - this builds intuition

8. **Focus on interpretation:** Statistical software does calculations - journalists need to explain what they mean
