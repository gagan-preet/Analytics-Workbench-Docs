## Use Cases

### Stats Enthusiast

```uml
@startuml

actor :Statistics\nEnthusiast: as StatsGuy

rectangle Profile {
StatsGuy -> (Profile Management)
(Profile Management) -|> (Login / logout)
(Profile Management) --|> (Group Admin Functions)
(Profile Management) ---|> (Profile modifications)
(Profile Management) ----|> (Mailing)
}

rectangle Usability {
StatsGuy --> (Usability Features)
(Usability Features) -|> (Search Operations)
(Usability Features) --|> (Documentation)
}

rectangle DataPortability {
StatsGuy ---> (Data Portability)
(Data Portability) -|> (Import projects)
(Data Portability) --|> (Export projects)
}

rectangle Preprocessing {
StatsGuy ----> (Data Preprocessing)
(Data Preprocessing) -|> (Data cleaning)
(Data Preprocessing) --|> (Data preparation)
(Data Preprocessing) ---|>  (Exploratory Data Analysis)
}

rectangle BatchStatistics {
StatsGuy -----> (Batch Statistics)
(Batch Statistics) -|> (Modeling)
(Batch Statistics) --|> (Segmentation)
(Batch Statistics) ---|> (Machine Learning)
(Batch Statistics) ----|> (Factor Analysis)
(Batch Statistics) -----|> (Time series operation)
}

rectangle UnstructuredStatistics {
StatsGuy ------> (Unstructured Statistics)
(Unstructured Statistics) -|> (Text Mining)
}

rectangle StreamingStatistics {
StatsGuy -------> (Streaming Statistics)
(Streaming Statistics) -|> (Image/Video Processing)
(Streaming Statistics) --|> (Voice processing)
}

rectangle Modules {
StatsGuy --------> (Modules)
(Modules) -|> (Batch process creation)
(Modules) --|> (Custom module generation)
}

rectangle UI{
StatsGuy ---------> (UI)
(UI) -|> (Visualizations)
(UI) --|> (Report generation)
}


@enduml
```

