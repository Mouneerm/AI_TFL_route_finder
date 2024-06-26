# AI_TFL_route_finder

The aim of this project is to construct an AI route finder for the London Underground that utilizes an agenda-based search mechanism. The data provided for this task is a CSV file named ‘tubedata.csv’, which contains information about the London Tube map. 

The Tube map is represented as a logical relation called a Tube “step”. Each row in the CSV file signifies a Tube “step” and follows this format: [StartingStation], [EndingStation], [TubeLine], [AverageTimeTaken], [MainZone], [SecondaryZone]. 

StartingStation: The station where the journey begins

EndingStation: The station directly connected to the starting station

TubeLine: The tube line that connects the two stations

AverageTimeTaken: The average time, in minutes, to travel between the starting and ending station

MainZone: The primary zone of the starting station

SecondaryZone: The secondary zone of the starting station. If the station is only in one zone, this value is 0. In such cases, the main zone is used to define the zone for the ending station. Otherwise, the secondary zone is used.



IThe three main search methods: Depth-First Search (DFS), Breadth-First Search (BFS), and Uniform Cost Search (UCS) are compared and tested. The costs will be in terms of the average time (even if not considered by DFS and BFS) and the number of nodes expanded for the different methods.

In addtion, heuristic based search such as Best First Search (BFS) and A-Star(A*) have been implemented.