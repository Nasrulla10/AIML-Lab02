# <div align="center">IT2011 - Artificial Intelligence and Machine Learning</div>
## <div align="center">Lab 02</div>

## Objectives:  
* Learn about using different types of prompting styles
* Use OpenAI's API
* Calling Hugging Face and its APIs



## Exercise 1:
Use the provided AWS Academy Generative AI Foundations course provided https://awsacademy.instructure.com/courses/129069 and complete the two activities in Module 04 - Using prompts and prompt engineering 

![lab2](/resources/lab.png)

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

