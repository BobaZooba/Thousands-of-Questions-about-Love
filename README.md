# Thousands of Questions about Love

# Context
RUSSIAN LANGUAGE

This dataset collected from real answers to questions of the mail.ru service: https://otvet.mail.ru/   
Category: Love

# Content
## Data Description
We have 82628 questions and 530511 answers!

```json
{
    "question": string, which contains question,
    "comment": string, sometimes question have comment better reveals the essence of the issue,
    "sub_category": string of sub category,
    "author": string contains author nickname,
    "author_rating": {
        "category": string - type of author rating,
        "value": string with rating,
    },
    "answers": [
        "text": string - text,
        "author_rating": ... same to author_rating
    ],
    "poll": [
        "text": string - text,
        "score": string - how many points scored this option
    ]
}
```

Answers or poll can be empty. Sometimes user chooses to make a poll and sets the options themselves. First answer is the best answer.

# Inspiration
This data can be helpful to create a chit-chat dialogue system. You can you ranking like architecture like DSSM.


