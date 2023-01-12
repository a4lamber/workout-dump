# Data entry template

For this project, since my training program has been developed into either train, climb or rest, we need to formalize the data entry as shown in the json template below

```json
{
    "date":"1111-11-11",
    "weight":85.4,
    "weight_unit":"kg",
    "workout":[
      {
        "name": "pull up",
        "note": "slightly tired",
        "details": 
        [
          {"weight": 0,"unit": "lb","reps": 8},
          {"weight": 0,"unit": "lb","reps": 8},
          {"weight": 0,"unit": "lb","reps": 5},
          {"weight": 25,"unit": "lb","reps": 3},
          {"weight": 25,"unit": "lb","reps": 3}
        ]
      }
    ],
      "climb": null,
      "daily reflection":null
  }
  ```
  
  The nested json could be exploded at the `workout` key word, from there you could entry your set and rep.