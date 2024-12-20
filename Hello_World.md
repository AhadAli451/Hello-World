### basically langchain contect the any LLM and langchain is a peekage

```! pip install langchain langchain-google-genai```

### basically it is a simple chatbord

``` python
import langchain_google_genai as genai

from langchain_google_genai import ChatGoogleGenerativeAI

from google.colab import userdata
GOOGLE_API_KEY = userdata.get('GOOGLE_API_KEY')


model : ChatGoogleGenerativeAI = ChatGoogleGenerativeAI(
    model ='gemini-1.5-flash',
    api_key=GOOGLE_API_KEY,
)


response1 = model.invoke('How many country in the world')


print(response1.content)
```