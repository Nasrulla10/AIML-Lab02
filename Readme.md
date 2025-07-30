# <div align="center">IT2011 - AIML</div>
## <div align="center">Lab 01</div>

## Objectives:  
* Learn about using different types of prompting styles
* Use OpenAI's API
* Calling Hugging Face and its APIs



## Exercise 1:
Use the provided AWS Academy Generative AI Foundations course provided https://awsacademy.instructure.com/courses/129069 and complete the two activities in Module 04 - Using prompts and prompt engineering 

![lab2](/resources/ec2lab.png)

1. Provide Screen shots of you doing the two labs as evidence.
2. Submit your answers under Exercise 1

## Exercise 2:


Complete the following program in the same Lab Instance

```c
#include <stdio.h>
#include <unistd.h>

int main() {
  char hostname[100];
  int ncpus;

  gethostname(hostname,100);
  ncpus = sysconf(_SC_NPROCESSORS_ONLN);
  printf("Hello World, I am running on host %s with %d logical cpus\n", hostname, ncpus);
  return 0;
}
```

6.	Compile the above program using the gcc C compiler - gcc (```gcc exercise01 -otest.o```)
7.	Run the above program in the AWS Linux Instance
8.	How many logical cores are there?
9.  Answer these questions in a text file called exercise02.txt
10. Commit and push the code to your repo.

```
git add .
git commit -m "<put a message here>"
git push
```
This is how you should commit your code back to your repo.  Please remember to this at the end of your lab session.  You can go back and continue to work on your solution within the given deadline.  If you are going to use a different folder to work on your program you can always get your code from your repo using the ```git clone``` command that you used earlier

## Exercise 3:


Complete the following program in the same Lab Instance, you will have to install openmp in your linux enviroment.

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

