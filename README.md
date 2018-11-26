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
This data can be helpful to create a chit-chat dialogue system. You can use ranking like architecture like DSSM.

# Ranking Architectures

| Name                                                                                   | Url                                                                                               |
|----------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|
| Learning Deep Structured Semantic Models for Web Search using Clickthrough Data (DSSM) | https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/cikm2013_DSSM_fullversion.pdf |
| Applying Deep Learning to answer selection: a study and an open task                   | https://arxiv.org/pdf/1508.01585.pdf                                                              |
| LSTM-Based Deep Learning Models for Nonfactoid answer selection                        | https://arxiv.org/pdf/1511.04108.pdf                                                              |
| Universal Sentence Encode                                                              | https://arxiv.org/pdf/1803.11175.pdf                                                              |
