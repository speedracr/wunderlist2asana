# Wunderlist to Asana - Team edition
<img src="https://dr0wv9n0kx6h5.cloudfront.net/664cb69d34d0ef040ff8a446e429bce8feb54b41/site/images/logo-big.png" height="128"><img src="http://virtualmarketingpro.com/app/webroot/img/vmp/arrows/Hand%20Drawn%20Arrow%20(37).png" height="128"><img src="https://freeter.io/embedding-web-apps/project-management/asana.png" height="128">

Export your Wunderlist content to an Asana team

# What you get
- Wunderlists lists --> Asana projects
- Wunderlist tasks --> Asana tasks. Preserved are:

  - subtasks;
  - due dates;
  - completion status
  - notes.

# Usage:
1. Create your Wunderlist backup (*Account Settings --> Create backup*)
2. Create your Asana private access token (*My Profile Settings --> Apps --> Manage Developer Apps*)
3. Click the name of the team in Asana that you want to import lists and tasks
   into and note its ID (example: https://app.asana.com/0/ *123123123123123* /overview)
4. Run the following:
```sh
$ pip install -r requirements.txt
$ python wunderlist_to_asana.py <Wunderlist backup file> <Asana token> <Asana organization> <Asana team ID>
```

Example:
```sh
$ python wunderlist_to_asana.py wunderlist-20190101-01-01-01.json '0/abc123abc123abc123abc123abc123ab' 'myorganization.com' '123123123123123'
```
