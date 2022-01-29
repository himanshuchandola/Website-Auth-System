# Website-Auth-System
Simple Website Auth System uses MongoDB as Database and Heroku for Application Hosting

This little auth system uses MongoDB as database and Heroku for application hosting

This is a pretty secure system it logs, ip and the key, so basically it will check the app and the key of what's being inputted

![Image of Simple Website-Auth-System](https://raw.githubusercontent.com/himanshuchandola/Website-Auth-System/main/img1.png?token=AIGH7INULX76LTXWCZXHKQDAZVIMO)


The database struct looks like so:

```
id:ObjectID("5e971bfe1c9d440000c4e781") //just a value mongo uses to track users/data
ip:"73.100.40.21" //sample ip of the user
key:"eqieq9eqe-qeqeqeq" //sample key
__v:"0" //anothor value uses for mongo

```
Connecting to the DB in user js

```
// Init
const app = express();
app.use(bodyParser.json());
app.use(bodyParser.urlencoded({ extended: true }));
mongoose
.connect(
'', //line where you add your mongo connection value if your connecting via mongo
{ useNewUrlParser: true, useUnifiedTopology: true }
)
.then(() => {
console.log('Connected to DB');

```
This was a little script/snippet I used for processing users, just a cool way on showing people that you don't need to use a forum software to protect downloads

## Instructions:

1. upload the frontend and backend files with Heroku
2. make a table on mongo or SQL your choice connect it
3. make a sample table with the code I provided above
4. upload your file into the "download" folder