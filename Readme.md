# <div align="center">IT2011 - Artificial Intelligence and Machine Learning</div>
## <div align="center">Lab 02</div>

## Objectives:  
* Learn about using different types of prompting styles
* Use OpenAI's API
* Calling Hugging Face and its APIs



## Exercise 1:
Use the provided AWS Academy Generative AI Foundations course provided https://awsacademy.instructure.com/courses/129069 and complete the two activities in Module 04 - Using prompts and prompt engineering 


<img src="/resources/lab.png" alt="Alt text" style="width: 50%;"/>


1. Provide Screen shots of you doing the two labs as evidence.
2. Submit your answers under Exercise 1

## Exercise 2:
Look at the LLM Leaderboard - https://artificialanalysis.ai/leaderboards/models

1. Where does your favourite LLM rank currently?
2. Try out at least two models that you haven't tried before (you will have to do a seperate google search to find these products)
3. Run two prompts of your choice
4. Submit the model, the prompt and the responses you have got.

## Exercise 3:
Use the following large language models, enabling the reasoning model of the platform and generate a detail report on "How you can use generative AI as a university student to learn subjects like probability and statistics, data base management systems and software engineering"

1. https://chat.deepseek.com - Deepthing R1
2. https://chat.qwen.ai - Thinking
3. https://x.com/i/grok - DeepSearch

In your submission, mention the LLMs used, the report, and a reflection of anything useful you have found, in your opinion which tool produced the best results

## Exercise 4:

1. Create an account at https://www.deeplearning.ai
2. Register to the free course at https://learn.deeplearning.ai/courses/chatgpt-building-system
3. Select the second activity
   

<img src="/resources/lab02.png" alt="Alt text" style="width: 60%;"/>

4. Execute the first code line in Jupiter notebook
5. Add the following code and in a codeblock and run

```
# Define system prompt (initial behavior) 
system_prompt = {"role": "system", "content": "You are a helpful assistant with deep knowledge in physics."} 
 
# Define user prompt (specific query) 
user_prompt = {"role": "user", "content": "Explain how black holes are formed."} 
 
# Send prompt to API 
response = openai.ChatCompletion.create( 
    model="gpt-3.5-turbo", 
    messages=[system_prompt, user_prompt] 
) 
print(response['choices'][0]['message']['content'])
```
Please see the figure below if you have issues running this</br>

<img src="/resources/lab03.png" alt="Alt text" style="width: 45%;"/>



6. Copy the codeblock given above again to the next cell and perform the following changes
7. Give a System Prompt for a chatbot to behave as an expert event planner
8. Give a User Prompt asking for advice how to plan for an event you have to do, maybe your friends Birthday Party, or a Batch Outing
9. Tryout a unique System prompt and User Prompt for a problem of your choice.
10. Share screen shots and upload the prompts and responses for activities 7,8,9

## Exercise 5.
1. Create an account in https://huggingface.co
2. Select any AI project of your liking under Spaces
3. Tryout the AI project and generate the output
4. Share screenshots of your usage of the AI project
5. Under Models select a Model of your choice to find more details about it
6. Create an account in https://colab.research.google.com
7. Change Runtime to GPU

<img src="/resources/lab04.png" alt="Alt text" style="width: 30%;"/>

9. Run the summarization example in a codeblock
10. 




```c
#include <stdio.h>
#include <omp.h>

int main() {
    // Start of parallel region
    #pragma omp parallel
    {
        int thread_id = omp_get_thread_num();     // Get the current thread ID
        int total_threads = omp_get_num_threads(); // Get total number of threads

        printf("Hello from thread %d out of %d threads!\n", thread_id, total_threads);
    }

    return 0;
}
```
To compile your program
```
gcc -fopenmp hello.c -o hello
./hello
```

Commit the code and add the output to a file output.txt 

## Exercise 4:

Complete the self assessment quiz for Module 6

Attach a screen shot of your completed self assessment for Module 6 and commit it

