## happy path
* greet
  - utter_greet
* mood_great
  - utter_happy

## sad path 1
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* affirm
  - utter_happy

## sad path 2
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* deny
  - utter_goodbye

## say goodbye
* goodbye
  - utter_goodbye

## bot challenge
* bot_challenge
  - utter_iamabot

## Chào hỏi và hỏi kết quả sổ xố
* ask_lottery
  - action_get_lottery
* thankyou
  - utter_goodbye

## Chào hỏi và hỏi kết quả sổ xố 2
* greet
  - utter_greet
* ask_lottery
  - action_get_lottery

## Chào hỏi và hỏi kết quả sổ xố 3
* ask_lottery
  - action_get_lottery