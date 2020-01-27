
## happy path               
* greet              
  - utter_greet
* mood_great              
  - utter_happy
* mood_affirm
  - utter_happy
* mood_affirm
  - action_default_ask_affirmation
  
## sad path          
* greet
  - utter_greet             
* mood_unhappy
  - action_revert_fallback_events
* inform{"animal":"dog"}  
  - action_default_ask_rephrase
  - utter_did_that_help
* mood_affirm
  - utter_happy
