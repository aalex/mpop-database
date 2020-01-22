# mpop-db

## Setup

```
docker-compose up -d
./sh_setup.sh
```

Prisma can be reached at http://localhost:4466

Open http://localhost:4466/_admin in a browser.



## Todo

Secure it with managementApiSecret: __YOUR_MANAGEMENT_API_SECRET__

Use a .env file for the environment variables.


## FIXME

```
[
  "Argument 'data' expected type 'AnswerCreateInput!' but got: {question_identifier: \"test_happy\", question: {connect: {id: \"ck5p85c4d001h08449wzkzc73\"}}, answer_value: 23}. Reason: 'user' Not-null field 'user' of type 'UserCreateOneWithoutAnswersInput!' defined in the 'AnswerCreateInput' input type is missing. (line 1, column 73):\nmutation { createAnswer_ck5p85yc400043r5mhvtcv16d: createAnswer(, data: { question_identifier: \"test_happy\", question: { connect: { id: \"ck5p85c4d001h08449wzkzc73\" } }, answer_value: 23 }) { __typename __typename id question_identifier question { __typename id id } answer_value }  }\n                                                                        ^"
]
```
