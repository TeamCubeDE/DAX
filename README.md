# DAX

## Circular dependency Issue

 ```
CrossEmpl = 

SUMMARIZECOLUMNS(Empl[Emplid] -- Trans[Emplid] would work
, 'Date'[Month]  -- group by month
, FILTER(Projects, Projects[ProjType]="Fix")
, "CE Hours", [TR Hours]
) 

```

![image](https://user-images.githubusercontent.com/84174814/118242261-6c9c9b80-b49d-11eb-8049-29b2a1edcddd.png)

![image](https://user-images.githubusercontent.com/84174814/118242524-bab19f00-b49d-11eb-9352-ea75cbdfcf30.png)

