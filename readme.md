# Waterrower
Waterrower App to store and analyze Workouts
Code as been taken from the old rower app to aquire data from the waterrower interface, adding a new application and a db around.


# SQL DB (Version 0.1)
CREATE TABLE "Workout" (
	`ID`	NUMERIC UNIQUE,
	`Date`	TEXT,
	`AverageStrokeRate`	INTEGER,
	`AverageHR`	INTEGER,
	`TotalCalories`	INTEGER,
	`TotalDistance`	INTEGER,
	`Field7`	INTEGER,
	PRIMARY KEY(ID)
)

CREATE TABLE "WorkoutData" (
	`ID`	INTEGER NOT NULL PRIMARY KEY AUTOINCREMENT UNIQUE,
	`WorkoutID`	INTEGER NOT NULL,
	`TimeStamp`	INTEGER,
	`Distance`	INTEGER,
	`Ratio`	INTEGER,
	`HR`	INTEGER
)

