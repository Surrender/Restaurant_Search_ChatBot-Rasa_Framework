# Restaurant_Search_ChatBot-Rasa_Framework
The project aims at building a restaurant search chatbot using Rasa framework that helps users to find restaurants across Indian Tier 1 and Tier 2 cities.   

# Business case - Foodie Restaurant Bot

An Indian startup named 'Foodie' wants to build a conversational bot (chatbot) which can help users discover restaurants across several Indian cities. 

The main purpose of the bot is to help users discover restaurants quickly and efficiently and to provide a good restaurant discovery experience. 

Zomato apis are used for searching the restaurants. https://developers.zomato.com/documentation#/


### Prerequisites

python 3.7.9
Visual studio for python development, VC++ Build tools 
rasa version 2.0.2
rasa-sdk version 2.0.0
spacy version 2.2.4
tensorflow version 2.3.1

### Installation Steps:

#### Create new virtual environment
`conda create -n rasa python=3.7`

#### Activate virtual environment
`conda activate rasa`

#### Install Rasa 2.0.2
`pip install rasa==2.0.2`

#### Install spacy
`pip install rasa[spacy]==2.0.2`
`python -m spacy download en_core_web_md`
`python -m spacy link en_core_web_md en`

#### Install Rasa-sdk 2.0.0
`pip uninstall rasa-sdk`
`pip install rasa-sdk==2.0.0`


## Train the nlu data & the core conversational flow using command line

$cd path <path to project>

### train the NLU
$rasa train nlu

### test the NLU
$rasa shell nlu

### train Core
$rasa train core

### test the Core
$rasa shell

### Run Dialogue management
    
    Step 1: run the action server
    ```
        $rasa run actions
    ```
    Step 2: run RASA Core
    ```
        $rasa shell
    ```

### train Rasa stories interactively
    ```
    rasa interactive
    ```


## Built With

* Rasa
* Keras Framework
* Tensorflow


## Authors

* Surender Yadaram
