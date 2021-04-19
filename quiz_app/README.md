You have to create a Quiz App.

The App should allow users to add/view quizes and questions. When adding new questions user should pick a quiz from existing quiz list to which a question will be assigned. The whole application should use separate routes for adding/viewing quizes/questions.

Add Quiz form should be accessed from `/add-quiz` link. View from `/quiz/:quiz-id`.

Structure for a quiz :
```
{
    "title": String,
    "description": String,
    "questions": Number[] // question-ids go here
}
```

Same routing approach for questions. 

Structure for a question :
```
{
    "title": String,
    "quiz": Number, // quiz id goes here
    "answers": [{
        "option": String,
        "isCorrect": ?Boolean
    }]
}
```