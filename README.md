# HurricaneAnalysis
A different solution to The Hurricane Analysis from Code Academy using Python.

My initial solution was to define a function to be used recurringly regardless if the keys were to change. My goal was to keep the function as short as possible. 

headings = ['Name', 'Month', 'Year', 'Max Sustained Wind', 'Area Affected', 'Damage', 'Death']
hurricane_data = list(zip(names, months, years, max_sustained_winds, areas_affected, updated_damages, deaths))
def make_dictionary(keys, values):
    library = {}
    for i in range(len(values)):
        library[keys[i]] = dict(list(zip(headings, values[i])))
    return library
hurricanes = make_dictionary(names, hurricane_data)
