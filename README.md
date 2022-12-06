# Workout organizer
---
## Description
---
Store the daily training log in `.json` format. The raw data in stored in the `./raw` named after the day of exerercise in `.json` format like `20220505.json`. An example schema looks like

```json
{
  "date":"2022-12-05",
  "weight":85.4,
  "weight_unit":"kg",
  "workout":[
    {
      "exercise": "pull up",
      "note": "slightly tired",
      "details": [
        {
          "weight": 0,
          "unit": "lb",
          "reps": 8
        },
        {
          "weight": 0,
          "unit": "lb",
          "reps": 8
        }
      ]
    },
    {
      "exercise": "barbell row",
      "note": "getting started!",
      "details": [
        {
          "weight": 95,
          "unit": "lb",
          "reps": 10
        },
        {
          "weight": 95,
          "unit": "lb",
          "reps": 10
        }
      ]
    }
  ]
}

    
```
The structure of the data is mainly for tracking
- the working set only
  - get total reps, total work volume
- track body weight


## Roadmaps
- [x] create a `json` file manually
- [ ] create an information for the metadata of each individual workout, similar to the work [here](https://github.com/wrkout/exercises.json/tree/master/exercises)
- [ ] figure out a file strcture similar to Azure namespace hierarchy for security and quicker data ingestion
- [ ] create an API to automatically generate json files 
- [ ] build a dashbord in `plotly` with heatmaps feature to track my activities
- [ ] figure out how to pus