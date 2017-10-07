<div width="100%" style="margin: 0 auto"><a class="linkedin-button" href="https://ca.linkedin.com/in/mrdavidgrant" target="blank"><img width="30%" height="28px" alt="View David R. Grant's profile on LinkedIn" src="https://static.licdn.com/scds/common/u/img/webpromo/btn_viewmy_160x25.png" border="0" height="28px"></a><a href="https://twitter.com/ITDaveG" target="blank"><img height="28px" src="images/twitterFollow.png" border="0"></a><a class="github-button" aria-label="Follow @mrdavidgrant on GitHub" href="https://github.com/mrdavidgrant" data-size="large" width="30%">Follow @mrdavidgrant</a></div>

> David, I just wanted to take a moment and appreciate you taking initiative and thinking outside of the box to ensure efficiency and success. Nicely done!
~ Dyan L, Metrolinx

# About Me

<img src="./images/myAvatar.svg" width="100px" height="100px" style="float: left; margin-right: 12px">

I am a Full Stack Web Developer and Problem Solver with experience programming in Multiple Languages and frameworks.  My background is in IT System Administration and Support with an extensive client list ranging from ISPs to large Provincial Corporations.  I wrote my first line of code in 1984, and am finally making the turn to doing it professionally. 

In addition to web development, I have experience working and maintaining Active Directory, Exchange servers, and ServiceNow (Administration and Development).


> Wanted to just give you a big kudos for what you've done on this - great initiative! Hope you don't mind that I brought it to [management]'s attention today to help expedite this... It's looking very polished... I will line up our internal change management folks... on this initiative (look at you...making a different[sic] company wide!)
~ Greg E, Price Waterhouse Coopers

***************

## Node.js/Express/PostgreSQL
- <a href="https://mrdavidgrant.github.io/the-eating-place">TWILIO API</a> 

A simple front-end designed to allow a user to order food online.  The backend then enters the information into a Postgresql database, and institutes an API call to TWILIO which calls the restaurant to place the order. The system receives phone input from the restaurant, and sends an SMS to the customer to inform them when the order will be ready for pickup.

- <a href="https://mrdavidgrant.github.io/tweeter/">TWEETER</a>

Twitter clone, using Nodejs, Express, EJS, and Mongo

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
- <a href='https://mrdavidgrant.github.io/chatty/'>CHATTY</a>

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
- <a href="https://mrdavidgrant.github.io/workspace_token_test/">Active Directory token Test</a>

Quick file io script to test to see if an AD user has an active VPN token and company assigned notebook.

```python
with open ('Workspace.csv') as original:
  with open('Workspace_Results.csv', 'w', newline='') as output:
    fieldnames = ['Name', 'AD Account', 'Email', 'Laptop', 'Active Token', 'WebEx']
    writer = csv.DictWriter(output, fieldnames=fieldnames)
    writer.writeheader()
    queryname = csv.DictReader(original)
```
## C# #
- <a href="https://mrdavidgrant.github.io/infopath_forms/">Infopath Form Fill in C#</a>

Quick script to autofill information on a Service Desk submission form with information obtained through Active Directory

```c#
string FirstName = employee.Properties["givenName"].Value.ToString();
string LastName = employee.Properties["sn"].Value.ToString();
string CommonName = employee.Properties["cn"].Value.ToString();
string Mail = employee.Properties["mail"].Value.ToString();
string Location = employee.Properties["extensionAttribute10"].Value.ToString();
string Title = employee.Properties["title"].Value.ToString();
```

## Ladder Logic
- <a href="https://www.youtube.com/watch?v=bZGecEJN5HI">View on YouTube</a>
<div width="100%" margin="0 auto">
<a href="https://www.youtube.com/watch?feature-player_embedded&v=bZGecEJN5HI" target="_blank"><img src="https://img.youtube.com/vi/bZGecEJN5HI/3.jpg" width="240px" height="180px" border="10" style="margin: 0 auto" /></a></div>

A 2006 project with the NSCC and Brain Repair Center for the QEII Health Sciences center in Halifax, Nova Scotia to create a robotic injection device for neurosurgery.  Device is currently in use at multiple hospitals worldwide.

<!-- Place this tag in your head or just before your close body tag. -->
<script async defer src="https://buttons.github.io/buttons.js"></script>
