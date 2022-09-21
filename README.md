## scada
### RU

Демо чат-бот `chatbotserver` обменивается данными по tls с чат-клиентами `chatbotclient`.    


***Схема обмена данными (scheme exchange of data):***


```mermaid
graph TB

  SubGraph3 --> SubGraph3Flow
  subgraph "SCADA Chat"
  SubGraph3Flow(ChatbotServer)
  SubGraph3Flow -- Message --> ChatBotClient-1
  SubGraph3Flow -- Message --> ChatBotClient-2
  SubGraph3Flow -- Message --> ChatBotClient-3
  end

  subgraph "SENDER"
  SubGraph3[Message of broadcast]
end
```  			

Для проверки, запустить модуль `chatbotserver` и клиентские модули `chatbotclient`. 


### EN

Demo chatbot `chatbotserver` exchange  data via tls with chat-clients `chatbotclient`.   

To test, run the `chatbotserver` module and the `chatbotclient` client modules.

