Tvarit Assignment Task 2

Problem Statement: 
Convert the script from task 1 to a REST API that accepts json input and returns json output with appropriate error handling

Examples
Replace {INPUT} in the curl command below with inputs in the table
curl -H 'Content-Type: application/json' -X PUT -d '{INPUT}’ http://localhost:5000/sum

I have created a django environment for a local webserver which once run with the command "python manage.py runserver 5000". 
One would be able to make such requests on the server. A preqrequisite for that is to activate the virtual environment venv
with command "source venv/bin/activate"
For example. "curl -X PUT   http://127.0.0.1:5000/sum   -H 'content-type: application/json'   -d '[1,2,3]'"

The request travels to the route of /sum and checking that the method is put, it runs the code similar to task 1 and returns the desired output.
If the request is of any other method than an error is raised with "Invalid request method".

No database or db connection is required for this particular environment.

After activating the venv, to run the tests, use command "python manage.py test"