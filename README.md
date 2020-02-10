# Float API

A Python wrapper of the project management service at float.com.

The API is documented here:
Float API at https://dev.float.com/api_reference.html

# Example of use
To use the API, you must pass the FLOAT_ACCESS_TOKEN to the FloatAPI
object when instantiating it.

```python
  # Import the API
  from float_api import FloatAPI
  
  # Instantiate API object
  api = FloatAPI(FLOAT_ACCESS_TOKEN)
  
  # Get a list of all people
  p = api.get_all_people()
```

# Calls
These are the calls implemented in this wrapper. If the input to a function
is DATA, it means a list of relevant arguments. See the
[Float documentation](https://dev.float.com/api_reference.html)
for details. get_all_* calls returns lists, delete_* returns True or False.
Other calls return dictionaries. On error, the wrapper will return empty
lists, False and empty dictionaries respectively.

## Clients

* get_all_clients()
* create_client(data)
* get_client(client_id)
* update_client(data)
* delete_client(client_id)


## People

* get_all_people()
* create_person(data)
* get_person(people_id)
* update_person(data)
* delete_person(people_id)


## Projects

* get_all_projects()
* create_project(data)
* get_project(project_id)
* update_project(data)
* delete_project(project_id)


## Tasks

* get_all_tasks()
* create_task(data)
* get_task(task_id)
* update_task(data)
* delete_task(task_id)

## Time off types

* get_all_timeoff_types()
* create_timeoff_type(data)
* get_timeoff_type(timeoff_type_id)
* update_timeoff_type(data)
* delete_timeoff_type(timeoff_type_id)


