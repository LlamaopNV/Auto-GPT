Thanks
========

For Orginal post and readme to assist with Setup please see the Orignal post for AutoGPT from user https://github.com/Significant-Gravitas/ : 
https://github.com/Significant-Gravitas/Auto-GPT


For a brief summary of what the code does Here is a helpful post : 
https://github.com/Torantulino/Auto-GPT/discussions/1239

A User just used AutoGPT to break down and understand AutoGPT

Current Fork was created on 15th of April 2023. 

Overview of current issues : 
============================

Web_browser function improvement.
AI hallucination management system.
Goal-oriented task system.
JSON data handling.
Separate actor for external data access.
Shared database for summarized data.

Thoughts on the current build
==============================


While the current AutoGPT project is impressive, it tends to lose focus on its goals. This fork aims to investigate weak points and build upon the application to assist the original project in becoming a more effective solution.

As GPT-4's full suite of functions becomes available, applications like AutoGPT will become even more powerful. The ability to understand images, for example, would significantly enhance the core offering.

Currently, the web_browser function faces issues with understanding websites and their content. Some examples include:

Receiving a 404 error and interpreting the website as only having information about a 404 error.
Failing to access information that requires user sign-up and considering the URL for sign-up as learned data.
Repeating the same process on the same website while altering the question parameter of the "browse_website" command, leading to inefficiencies and token count issues.
To address these concerns, the following improvements are suggested:

External data access:
Develop a separate actor trained to interpret HTTP response codes and understand website content more effectively.
Consider creating a shared, community-driven database of pre-"chunked" data to reduce costs and improve efficiency.
Implement basic HTTP response understanding, focusing on distinguishing between HTTP 200 - OK and other responses.
Shared Database:
A mutual shared database would benefit the community by providing a core checking point for data and reducing costs through pre-summarized data.
This would require significant effort to establish and maintain but could greatly enhance the AutoGPT ecosystem.

Reason :
The Database would act as a core checking point for a data point, for example lets say I am training an AutoGPT to be an assistant on the OpenAI API so it can just quikcly answer my questions on an API query. 

If we had a shared community Database we could reduce costs greatly by just checking the database first and already having summarized data. Users could all benefit form such a Dataset but granted this would be a mamouth task. 


