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

Source code: https://github.com/MAT496-Monsoon2025-SNU/adilmuhammed-langgraph-mat496/blob/a07f800a72e487e709e38d07dd047902239bd746/Sourcecodes/router.ipynb

Edited code: https://github.com/MAT496-Monsoon2025-SNU/adilmuhammed-langgraph-mat496/blob/a07f800a72e487e709e38d07dd047902239bd746/Module1/router.ipynb

Video 6 — Agents

Learnings:

In this video we learned about using tools recursively in other words instead of after the a tool gives output instead of going to end it comes back to caller till desired output is produced. We also included tracing in this code so that we can see the process and details in langsmith trace simila to what we did in langchain.

<img width="2012" height="1026" alt="Screenshot 2025-10-16 222531" src="https://github.com/user-attachments/assets/ff2c0979-6882-410a-88d0-250d74e2f3d2" />

Code Changes:

Made neccessary changes for code to run and changed the question

Notebooks:

Source code: https://github.com/MAT496-Monsoon2025-SNU/adilmuhammed-langgraph-mat496/blob/a07f800a72e487e709e38d07dd047902239bd746/Sourcecodes/agent.ipynb

Edited code: https://github.com/MAT496-Monsoon2025-SNU/adilmuhammed-langgraph-mat496/blob/a07f800a72e487e709e38d07dd047902239bd746/Module1/agent.ipynb

Video 7 — Agents with memory

Learnings:

In this video we just introduced memory to previous code by persistance. Checkpoints were implemented for memory using thread id to save the state. In this way memory was achieved using common thread.

Code Changes:

Made neccessary changes for code to run and added new function

Notebooks:

Source code: https://github.com/MAT496-Monsoon2025-SNU/adilmuhammed-langgraph-mat496/blob/a07f800a72e487e709e38d07dd047902239bd746/Sourcecodes/agent-memory.ipynb

Edited code: https://github.com/MAT496-Monsoon2025-SNU/adilmuhammed-langgraph-mat496/blob/a07f800a72e487e709e38d07dd047902239bd746/Module1/agent-memory.ipynb

Video 8 — Intro to Deployment (Optional)

Learnings:

This was just a optional video on intro to different aspects of final deployment of our agent. Cloud deployment was shown but was not able to do it because it was not free.<br><br><br>

Module 2

Video 1 — State Schema

Learnings:

In this video we primarily did an overview of what we are going to do in module 2 and then revisited creating basic graph from module 1 simple graph and then added some more details to it. We learned to implement dataclass of python for concise syntax for creating classes that are primarily used on storing data. We then also added pydantic state so that we can catch errors when passing keys to our state on runtime.

Code Changes:

Created a new node for on the  same level as node 2 and 3 called node 4 for empty mood.

Created a new cell block at end to test pydantic state 

Notebooks:

Source code: https://github.com/MAT496-Monsoon2025-SNU/adilmuhammed-langgraph-mat496/blob/a2f93a40300da113eafb991983f41df584c6b9ef/Sourcecodes/state-schema.ipynb

Edited code: https://github.com/MAT496-Monsoon2025-SNU/adilmuhammed-langgraph-mat496/blob/a2f93a40300da113eafb991983f41df584c6b9ef/Module2/state-schema.ipynb

Video 2 — State Reducers

Learnings:

In this video we learned to update value of nodes on same level by appending instead of overwriting as that leads to problems. This was achieved by using reducers. Then we used custom reducers to handle edge cases. We then messagestate. We then did rewriting and removal of messages using id. This is very useful as we can now have full control of what stays in memory.

Code Changes:

Deleted more messages and made required changes for code to run

Notebooks:

Source code: https://github.com/MAT496-Monsoon2025-SNU/adilmuhammed-langgraph-mat496/blob/a2f93a40300da113eafb991983f41df584c6b9ef/Sourcecodes/state-reducers.ipynb

Edited code: https://github.com/MAT496-Monsoon2025-SNU/adilmuhammed-langgraph-mat496/blob/a2f93a40300da113eafb991983f41df584c6b9ef/Module2/state-reducers.ipynb

Video 3 — Multiple Schemas

Learnings:

In this video we used multiple schemas which is a very simple but useful tool to restrict what is present in input and output schemas of a graph and if we want them to be different we can apply input and output filter on our overall state.

Code Changes:

No changes were made to the code as this was just a code to show using multiple schemas and any changes would get in the way of demonstration

Notebooks:

Source code: https://github.com/MAT496-Monsoon2025-SNU/adilmuhammed-langgraph-mat496/blob/a2f93a40300da113eafb991983f41df584c6b9ef/Sourcecodes/multiple-schemas.ipynb

Edited code: https://github.com/MAT496-Monsoon2025-SNU/adilmuhammed-langgraph-mat496/blob/a2f93a40300da113eafb991983f41df584c6b9ef/Module2/multiple-schemas.ipynb

Video 4 — Trim and Filter Messages

Learnings:

In this video we learned about editing messages to reduce our token usage which is very important to be cost efficient. First we revisited removing messages we used earlier. We can also filter what messages llm see without editing messagestate so that token usage go down but still preserve the messages we saved. There is also trim messages where we directly control token usage by number and have further control like strategy used and whether to allow partial message or not to be included.

Code Changes:

I changed some deletion of messages, filtering of messages and then changed and added trimming. Different token usage and strategies were tried for trimming messages.

Notebooks:

Source code: https://github.com/MAT496-Monsoon2025-SNU/adilmuhammed-langgraph-mat496/blob/a2f93a40300da113eafb991983f41df584c6b9ef/Sourcecodes/trim-filter-messages.ipynb

Edited code: https://github.com/MAT496-Monsoon2025-SNU/adilmuhammed-langgraph-mat496/blob/a2f93a40300da113eafb991983f41df584c6b9ef/Module2/trim-filter-messages.ipynb

Video 5 — Chatbot w/ Summarizing Memory and Messages

Learnings:

In this video we learned to set up summary where it will save summary of the messagestate and we can control on how many messages should the summary start. We can also do this while using thread so the messages doesn't have to be appended at same time for it to be summarized. The summary lives in its own state.

Code Changes:

The messages were changed and the message threshold for starting the summary was changed.

Notebooks:

Source code: https://github.com/MAT496-Monsoon2025-SNU/adilmuhammed-langgraph-mat496/blob/a2f93a40300da113eafb991983f41df584c6b9ef/Sourcecodes/chatbot-summarization.ipynb

Edited code: https://github.com/MAT496-Monsoon2025-SNU/adilmuhammed-langgraph-mat496/blob/a2f93a40300da113eafb991983f41df584c6b9ef/Module2/chatbot-summarization.ipynb

Video 6 — Chatbot w/ Summarizing Messages and External Memory

Learnings:

In this video we used Sqlite to set up external memory so that the lifetime of the saved messages and other states were not just the lifetime of the notebook kernel. Now even if we close the kernel we were able to verify that the information was stillsaved through Sqlite. We then also viewed the summarization working in langgraph studio


<img width="2028" height="1092" alt="image" src="https://github.com/user-attachments/assets/328975ab-2493-46e5-a060-dd5754e1dfeb" />

Code Changes:

The message threshold for starting the summary was changed and the context also was changes.

Notebooks:

Source code: https://github.com/MAT496-Monsoon2025-SNU/adilmuhammed-langgraph-mat496/blob/a2f93a40300da113eafb991983f41df584c6b9ef/Sourcecodes/chatbot-external-memory.ipynb

Edited code: https://github.com/MAT496-Monsoon2025-SNU/adilmuhammed-langgraph-mat496/blob/a2f93a40300da113eafb991983f41df584c6b9ef/Module2/chatbot-external-memory.ipynb




















