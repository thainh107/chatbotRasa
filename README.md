
Chat bot get ketqua.net

-- install pip ( package manager of python )
easy_install pip  
-- install virtualenv from pip
 pip install virtualenv 

https://virtualenv.pypa.io/en/latest/userguide/

enable virtualenv 

 ---- source [/path/to/ENV/bin/activate]

https://rasa.com/docs/rasa/user-guide/installation/


-- run actions

python -m rasa_sdk.endpoint --actions actions

-- train bot

rasa train

-- run bot on server

python -m rasa run -m ./models --log-file out.log -vv --enable-api

rasa run

/conversations/<conversation_id>/messages          POST                           add_message
/conversations/<conversation_id>/tracker/events    POST                           append_events
/webhooks/rasa                                     GET                            custom_webhook_RasaChatInput.health
/webhooks/rasa/webhook                             POST                           custom_webhook_RasaChatInput.receive
/webhooks/rest                                     GET                            custom_webhook_RestInput.health
/webhooks/rest/webhook                             POST                           custom_webhook_RestInput.receive
/model/test/intents                                POST                           evaluate_intents
/model/test/stories                                POST                           evaluate_stories
/conversations/<conversation_id>/execute           POST                           execute_action
/domain                                            GET                            get_domain
/                                                  GET                            hello
/model                                             PUT                            load_model
/model/parse                                       POST                           parse
/conversations/<conversation_id>/predict           POST                           predict
/conversations/<conversation_id>/tracker/events    PUT                            replace_events
/conversations/<conversation_id>/story             GET                            retrieve_story
/conversations/<conversation_id>/tracker           GET                            retrieve_tracker
/status                                            GET                            status
/model/predict                                     POST                           tracker_predict
/model/train                                       POST                           train
/model                                             DELETE                         unload_model
/version                                           GET                            version

