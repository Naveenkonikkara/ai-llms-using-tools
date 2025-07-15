Learn how to use a tool from scratch and integrate it with LLMs
Interacting with OpenAI's Function Calling Feature

###### UV Commands ######
uv init
uv add python-dotenv openai
uv run main.py

##### OUTPUT ######
Your question (type 'exit' to end the conversation): What can you do for me?    
I can help you with a wide range of tasks, including:

1. **Answering Questions:** I can provide information on a variety of topics.
2. **Weather Information:** I can get you the current temperature for a specific location.
3. **Image Understanding:** I can analyze and understand images you share with me.        
4. **Learning and Tutoring:** I can assist with educational inquiries and explanations.   
5. **Recommendations:** Whether it's books, movies, or restaurants, I can suggest options.
6. **Language Help:** I can assist with translations and language learning tips.

Feel free to ask if you have something specific in mind!
Your question (type 'exit' to end the conversation): What's the temperature in Kerala?
Fetching temperature for: Kerala
The current temperature in Kerala is 20°C. If you need more details or forecasts, just let me know!
Your question (type 'exit' to end the conversation): exit
[{'role': 'developer', 'content': "You are a helpful assistant. Answer the user's question in a friendly way."}, {'role': 'user', 'content': 'What can you do for me?'}, ResponseOutputMessage(id='msg_68765ae3d81481929b13313e691f876e02e5a536067cae65', content=[ResponseOutputText(annotations=[], text="I can help you with a wide range of tasks, including:\n\n1. **Answering Questions:** I can provide information on a variety of topics.\n2. **Weather Information:** I can get you the current temperature for a specific location.\n3. **Image Understanding:** I can analyze and understand images you share with me.\n4. **Learning and Tutoring:** I can assist with educational inquiries and explanations.\n5. **Recommendations:** Whether it's books, movies, or restaurants, I can suggest options.\n6. **Language Help:** I can assist with translations and language learning tips.\n\nFeel free to ask if you have something specific in mind!", type='output_text', logprobs=[])], role='assistant', status='completed', type='message'), {'role': 'user', 'content': "What's the temperature in Kerala?"}, ResponseFunctionToolCall(arguments='{"city":"Kerala"}', call_id='call_6078NvJgjNc3idJsNxSEa96F', name='get_temperature', type='function_call', id='fc_68765b02dc6c8192874f82514383d7d502e5a536067cae65', status='completed'), {'type': 'function_call_output', 'call_id': 'call_6078NvJgjNc3idJsNxSEa96F', 'output': '20.0'}]