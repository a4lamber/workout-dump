# Workout organizer

For this project, it has been created with the intention of  
- a data storage to hold my daily workout session, climbing session data in `.json` format
- available for future analysis on the workout session to fine tuning
  - tuning workout volume or intensity if plateau
  - spot the weakness
- visualization of the workout + climbing

## Data Entry template

Store the daily training log in `.json` format. The raw data in stored in the `./raw` named after the day of exerercise in `.json` format like `20220505.json`. An example schema looks like

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
The structure of the data is mainly for tracking
- the working set
  - get total reps, total work volume
- track body weight
- track contribution

[Click here for data entry template](./data_template.md)


## Roadmaps
- [x] create a `json` file manually
- [ ] create an information for the metadata of each individual workout, similar to the work [here](https://github.com/wrkout/exercises.json/tree/master/exercises)
- [ ] figure out a file strcture similar to Azure namespace hierarchy for security and quicker data ingestion
- [ ] create an API to automatically generate json files 
- [ ] build a dashbord in `plotly` with heatmaps feature to track my activities
- [ ] figure out how to pus