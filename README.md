# Github Issue Similarity

## Problem statement 
On various support forums like Github , Jira forums , IT support forums , Dicourse etc face a challenge of duplicate post/issues which are already been answered previously. Presently they need to have a maintainer who filters out such post. In IT support system such issues might causes unwanted delays which could have been avoided if relevent references were available at that time. 


## Our Solution

### Stage 1 : Developing our Knowledege base
- Scrap all issues from forums (Here Github Issues) using their APIs
- Generate their embeddings
- Store those embeddings in a vector database (ApertureData)

### Stage 2 : Query our Knowledege base
- Develop any bot or API service which takes user's post/issue as input
- The bot or API service will generate embeddings of input and query the vector database
- The bot will get relevant post/issues based on threshold and reply to the user.

## System design 
![plot](system_design.png)
