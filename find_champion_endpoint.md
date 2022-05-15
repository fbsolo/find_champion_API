### find_champion(name=None, role=None, origin=None)

#### Parameters

##### name *string*
##### role *string*
##### origin *string*
---
#### Description

1. **find_champion** depends on two-dimensional array **champion_data**; the nested array element(s) must have three elements of these names and types:

   **name** *string*
   
   **role** *string*
   
   **origin** *string*

2. Depending on parameter values, **find_champion** returns an empty array, or one nested array element of the **champion_data** array

3. If parameter **name** matches one or more **champion_data.name** elements, **find_champion** returns the first **champion_data** array element whose **name** element it matches, and ignores the remaining parameters

   a. if parameter **name** has a **None** value, or does not match a **champion_data.name** element, **find_champion** tries to use the *role* and *origin* parameters to match a **champion_data** row

4. If the **role** and **origin** parameters match corresponding values in the same **champion_data** array element, **find_champion** returns that specific **champion_data** array element. Otherwise, **find_champion** returns an empty array
