Module 1
Video 1 — Motivation

Learnings:

In video 1 we got a brief explanation of why langgraph is used in the first place, its to balance reliabity and control of the llm. There were no specific topics covered in this video just a overview of what we are going to do in each module. No codes were given in this video.

Video 2 — Simple graph

Learnings:

In this video I learned how the basics of nodes and graph workings and how to create them. In the code we used we still haven't used llm to decide which node to choose. For now we used random number generation for outcome. The general idea was similar to neural networks.

Code Changes:

Added a new block to test the selection of node by random generation

Notebooks:

Source code: https://github.com/MAT496-Monsoon2025-SNU/adilmuhammed-langgraph-mat496/blob/757a5f3a914556c8ca534e8c8f3cf76a3ef4c398/Sourcecodes/simple-graph.ipynb

Edited code: https://github.com/MAT496-Monsoon2025-SNU/adilmuhammed-langgraph-mat496/blob/5e7ea19c04b575540684b250e8183befbdd27bfb/Module1/simple-graph.ipynb

Video 3 — LangSmith Studio

Learnings:

In this video we used the studio interface in langsmith for first time. This is used for debugging and reviewing different cases, to get a better understanding of our structure at t gives a great visual repsentation etc.
There was no code in this video

<img width="2018" height="1095" alt="image" src="https://github.com/user-attachments/assets/c6d4c1de-2f33-48af-818c-44a8251e8d63" />


Video 4 — Chain

Learnings:

In this video we learned to build simple chain in graph using chat messages. We also learned implementing tool calling which we had learned before to graph.

Code Changes:

Made neccessary changes for code to run and changed the tool which was used

Notebooks:

Source code: https://github.com/MAT496-Monsoon2025-SNU/adilmuhammed-langgraph-mat496/blob/757a5f3a914556c8ca534e8c8f3cf76a3ef4c398/Sourcecodes/chain.ipynb

Edited code: https://github.com/MAT496-Monsoon2025-SNU/adilmuhammed-langgraph-mat496/blob/5e7ea19c04b575540684b250e8183befbdd27bfb/Module1/chain.ipynb

Video 5 — Router

Learnings:

In this video I learned about about how the llm decide whether to call the tool or not, its visual represantaion by seeing it taking different node route depending on its decision. This is provided by the studio


<img width="2036" height="1017" alt="image" src="https://github.com/user-attachments/assets/a0015cad-b2f7-4e5a-b1bc-e8294edcb7f2" />

Code Changes:

Made neccessary changes for code to run and changed the tool which was used

Notebooks:

Source code: 

Edited code: 

Video 6 — Agents

Learnings:

In this video we learned about using tools recursively in other words instead of after the a tool gives output instead of going to end it comes back to caller till desired output is produced. We also included tracing in this code so that we can see the process and details in langsmith trace simila to what we did in langchain.
I
<img width="2012" height="1026" alt="Screenshot 2025-10-16 222531" src="https://github.com/user-attachments/assets/ff2c0979-6882-410a-88d0-250d74e2f3d2" />

Code Changes:

Made neccessary changes for code to run and changed the question

Notebooks:

Source code: 

Edited code: 

Video 7 — Agents

Learnings:

In this video we just introduced memory to previous code by persistance. Checkpoints were implemented for memory using thread id to save the state. In this way memory was achieved using common thread.

Code Changes:

Made neccessary changes for code to run and added new function

Notebooks:

Source code: 

Edited code: 

Video 7 — Intro to Deployment

Learnings:

I










