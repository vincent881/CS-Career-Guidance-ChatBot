# Write Up  
## A.	Explain the functionalities of the chatbot and how they will meet the needs described in the scenario.  
- The chatbot provides interest to role mapping. It asks the student for their strengths and interests and provides them with matching computer science roles. Students often struggle to see the link between skill sets and career paths. The bot provides the link between the two.
- The chatbot uses AIML <pattern> to handle a variety of synonymous inputs. This ensures the chat bot can handle student inputs to reduce frustration of unrecognized phrases.
## B.	Identify five computing job types that your chatbot can recommend based on student interaction with the chatbot.  
- Software Engineer
- Data Analyst
- Cybersecurity Analyst
- UI/UX Designer
- System Administrator

## C.	Explain how the chatbot training cases were selected and how you used artificial intelligence markup language (AIML) to enhance the functionality of the chatbot. Provide examples of the chatbot’s functionality that represent the selected cases at the end of the training process in support of your explanation.  
- I started by researching entry level Computer Science job descriptions and common academic interests (programming, math, data, security, design, systems. For each interest area, I chose the job that correlated with the interest the most.
- AIML’s pattern template structure allows for precise mapping from each keyword to a career recommendation. I grouped synonyms into multiple <category> entries pointing to the same <template>. For example, this ensures that both data and numbers will point to Data Analyst.
- The training cases were derived from core interest areas students commonly express when exploring computer science careers: programming, math, data, security, design, systems. For each of these, multiple representative input variations were selected so the bot could be trained and tested on realistic students.
### Why They Were Chosen  
- The five job types correlate directly to common student strengths and are broad enough to be meaningful starting points.
- Students rarely use identical wording, so including cases like “numbers”, “data”, or “I love designing” ensures the bot recognizes varied expressions of the same intent.
- Command inputs like “I like programming and security” test whether the bot can either surface multiple relevant roles or prompt for classification. This improves the conversational experience.
- Inputs with minor typos or unexpected formats were included to evaluate if normalization is needed.
- Cases like “I want to cook” confirm that the bot does not give misleading career advice.
### Examples of Training Cases  
| User Input | Chatbot Response |
| :---: | :---: |
| "I love numbers" | If you enjoy working with Data or Numbers, consider a Data Analyst role. To see other interests, type "Interests" |
| "Interests" | What is another interest you have? (Programming, Math, Data, Numbers, Security, Networks, Design, Servers, Systems) |  
| "I like to cook" | That does not match the computer science interests. Would you like to rephrase with one? (Programming, Math, Data, Numbers, Security, Networks, Design, Servers, Systems) |
| "I enjoy math" | With interests in math or programming, a Software Engineer role will be a great fit. To see another role, type "Roles" |
| "I want to work on servers" | If you enjoy managing systems or servers, a System Administrator would be a good role for you. To see other interests, type "Interests" |
