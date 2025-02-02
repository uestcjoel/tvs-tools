### 设备控制指令
```json
{
    "directive": {
        "header": {
            "namespace": "DeviceControl",
            "name": "Control",
            "messageId": "{{STRING}}",
            "dialogRequestId": "{{STRING}}"
        },
        "payload": {
            "nlpInfo" {
                "domain": "{{STRING}}",
                "intent": "{{STRING}}",
            },
            "data": {
                "controlData": "{{STRING}}"
            }
        }
    }
}
```

***Header Paramters***

|    Parameter        		|    Type    	|    必选	|    描述                            	|
|    :------------------- 		|    :-------- 	|    :----- 	|    :-------------------------------- 	|
|    messageId       	 	|    string  	|    Yes 	|    消息ID                        	|
|    dialogRequestId    |    string  	|    No 	|    对话ID                       	|

***Payload Paramters***

|    Parameter                        		|    Type 	|    必选	|    描述                          	|
|    :---------------------------------------	|    :-------- 	|    :-----	|    :-------------------------------- 	|
|    nlpInfo                              	|    object	|    Yes 	|    NLP信息                     	|
|    nlpInfo.domain                	 	|    string  	|    Yes 	|    NLP领域信息               	|
|    nlpInfo.intent                       	|    string  	|    Yes 	|    NLP意图信息               	|
|    data                                    	|    object 	|    Yes  |    数据                           	|
|    data.controlData                 	|    string  	|    Yes  |    服务数据                   	|