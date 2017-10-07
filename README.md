# Portfolio of David Grant

<img src="./images/myAvatar.svg" width="100px" height="100px" style="float: left">
I am a Full Stack Web Developer and Problem Solver with experience programming in Multiple Languages and frameworks.  My background is in IT System Administration and Support with an extensive client list ranging from ISPs to large Provincial Corporations.

## Node.js/Express/PostgreSQL
[TWILIO API Project] (https://mrdavidgrant.github.io/the-eating-place/) 

A simple front-end designed to allow a user to order food online.  The backend then enters the information into a Postgresql database, and institutes an API call to TWILIO which calls the restaurant to place the order. The system receives phone input from the restaurant, and sends an SMS to the customer to inform them when the order will be ready for pickup.

```javascript
function insertUser (submission) {
knex('users')
.returning('id')
.insert(submission.user, 'id')
.then(result => {
  submission.user.id = result[0]
})
}
```

## HTML/SASS/REACT
[Chatty] (https://mrdavidgrant.github.io/chatty/)

A basic chatroom application, designed to showcase REACT and SASS.
```javascript
handleKeyDown(e) {
  if(e.key == "Enter"){
    const newMessage ={ type: 'postMessage', userid: this.state.userid, username: this.state.currentUser.name, content: e.target.value}
    this.sendMessage(newMessage)
    e.target.value = ''
  }
}
```

## Python
```python
with open ('Workspace.csv') as original:
  with open('Workspace_Results.csv', 'w', newline='') as output:
    fieldnames = ['Name', 'AD Account', 'Email', 'Laptop', 'Active Token', 'WebEx']
    writer = csv.DictWriter(output, fieldnames=fieldnames)
    writer.writeheader()
    queryname = csv.DictReader(original)
```