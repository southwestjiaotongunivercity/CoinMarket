# CoinMarket

curl http://localhost:5000/todos -d "task=something new" -X POST -v

curl http://localhost:5000/todos/todo3 -d "task=something different" -X PUT -v

# Look only in the POST body
parser.add_argument('name', type=int, location='form')

# Look only in the querystring
parser.add_argument('PageSize', type=int, location='args')

# From the request headers
parser.add_argument('User-Agent', type=str, location='headers')

# From http cookies
parser.add_argument('session_id', type=str, location='cookies')

# From file uploads
parser.add_argument('picture', type=werkzeug.datastructures.FileStorage, location='files')


http://www.pythondoc.com/Flask-RESTful/extending.html
