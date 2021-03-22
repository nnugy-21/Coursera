# System Administration Consultation

## Scenario 1

You’re doing systems administration work for Network Funtime Company. Evaluate their current IT infrastructure needs and limitations, then provide at least five process improvements and rationale behind those improvements. Write a 200-400 word process review for this consultation. Remember, there’s no right or wrong answer, but make sure to provide your reasoning.

**Software Company**:

Network Funtime Company is a small company that builds open-source software. The company is made up software engineers, a few designers, one person in Human Resources (HR), and a small sales team. Altogether, there are 100 employees. They recently hired you as a system administrator to come in and become their IT department.

When a new person is hired on, the HR person purchases a laptop for them to do their work. The HR representative is unfamiliar with what type of hardware is out there; if a new employee requests a laptop, the HR person will purchase the cheapest option for a laptop online. Because of this, almost everyone has a different laptop model. The company doesn’t have too much revenue to spend, so they don’t order laptops until someone gets hired at the company. This leads to a few days of wait time from when someone starts to when they can actually work on a laptop.

The company doesn’t label their computers with anything, so if a computer is missing or stolen, there’s no way to audit it. There’s no inventory system to keep track of what’s currently in the fleet.

Once a computer is purchased, the HR person hands it to the new employee to set up. Software engineers that use Linux have to find a USB drive and add their preferred distribution to the laptop. Anytime someone needs something from HR -- whether it’s office related or tech related -- they email the HR representative directly.

When a new employee gets a machine, they’re given logins to use cloud services. They get a personal orientation with HR to make sure they can login. This requires the HR person to block off a few hours for every new employee. If an employee forgets the login to their machine, they have no way to retrieve a password and they have to reimagine their machine. Employees don’t have a strict password requirement to set for their computers.

The company currently has many of their services in the cloud, such as email, word processors, spreadsheet applications, etc. They also use the application, Slack, for instant communication.

**My Review**: 
```
Problems that Network Funtime Company has:
1. The HR always purchases the cheapest hardware for all the employees, because of this almost everyone has different laptop model.
Review:
This could result to a decrease of productivity in the entire organization, because different type of work needs different type of machine or specification to working properly.
Solutions:
First of all, we need to change the system where the HR has the absolute decision about what machine to buy. We can change it so the HR needs to communicate with the IT department and Finance department about what type of machine that they need to buy, so everyone in the organization can do their work smoothly and still in the range of the company’s budget. This can be done by making a tier-list of machine that they need to give to every department in the organization, so everyone in the organization can have a machine that matched what they need.
We can also make an agreement with certain vendors about the machine that we want to buy. So, maybe we can reduce the cost to buy all the machines that we need, while also make the entire organization has a uniform machine.

2. The company doesn’t have too much revenue to spend, so they don’t order laptops until someone gets hired at the company.
Review:
This leads to a few days of wait time from when someone starts to when they can actually work on a laptop.
Solutions:
For this problem we need to have some backup machine that we can give temporarily to the employee.

3. The company doesn’t label their computers with anything, there’s no inventory system to keep track of what’s currently in the fleet.
Review:
So, if a computer is missing or stolen, there’s no way to audit it.
Solutions:
We can need to make documentation about every machine that we give to the employee and make certain policies regarding ownership of that machine, like what happen when the employee left the company or the machine is stolen.

4. When a computer is purchased, the HR person hands it to the new employee to set up. So, software engineers that use linux have to find USB drive and add their preferred distribution to the laptop.
Review:
This could be hard for employees that doesn’t familiar with how to configure their machine.
Solutions:
First, we need to make certain policies about the machine configuration like what type of OS that they need to use, so this way everyone can have a uniform OS that matched their needs.
We can use certain configuration-management tools like puppet to pre-configure the machine and always making sure that every software that essentials is up to date.

5. Anytime someone needs something from HR whether it’s office related or tech related they email the HR representative directly.
Review:
This will slow down the productivity of the organization, because the HR can’t answer all their problems simultaneously 24/7
Solution:
We can make a ticketing system based on email with certain tags. So if some employees have a certain problem they need to email their problem and attached some tags along with it. With this their problem can be reviewed by every department that is related to their problem, and can help solving it too.

6. Every employee gets a personal orientation with HR to make sure they can login to the cloud. If the employee forgot their login password, they have no way to retrieve it.
Review:
This problem is consuming too much time.
Solutions:
We need to have a centralized management about employee account that we can monitor and access every time we need it. We can use tools like LADP or Active Directory to handle it.
```
<br>

## Scenario 2

You’re doing systems administration work for W.D. Widgets. Evaluate their current IT infrastructure needs and limitations, then provide at least five process improvements and rationale behind those improvements. Please write a 200-400 word process review for this consultation. Remember, there’s no right or wrong answer, but make sure to provide your reasoning.

**Sales Company**:

W.D. Widgets is a small company that sells widgets. They’re mostly made up of salespeople who work with lots of clients. You’ve taken over as the sole IT person for this company of 80-100 people.

When HR tells you to provision a machine for a new employee, you order the hardware directly from a business vendor. You keep one or two machines in stock, in case of emergency. The users receive a username that you generate for them. You then give them an orientation on how to login when they start. You currently manage all of your machines using Windows Active Directory. The company uses only Windows computers. When a new computer is provisioned, you have to install lots of sales-specific applications manually onto every machine. This takes a few hours of your time for each machine. When someone has an IT-related request, they email you directly to help them.

Almost all software is kept in-house, meaning that you’re responsible for the email server, local machine software, and instant messenger. None of the company’s services are kept on the cloud.

Customer data is stored on a single file server. When a new salesperson starts, you also map this file server onto their local machine, so that they can access it like a directory. Whoever creates a folder on this server owns that folder and everything in it. There are no backups to this critical customer data. If a user deletes something, it may be lost for everyone.

The company generates a lot of revenue and is rapidly growing. They’re expecting to hire hundreds of new employees in the next year or so, and you may not be able to scale your operations at the pace you’re working.

**My Review**:
```
Problem that W.D Widgets has:
1. When HR tells you to provision a machine for a new employee, you order the hardware directly from a business vendor.
Review:
It’s good, but it’s inefficient if we had to do it every day.
Solutions:
We can have an automated system that integrated with the company employee’s database, so every time there’s a new employee the system will order the machine the specific machine for us. But, of course before purchasing it the system need our permissions to do it.

2. The users receive a username that you generate for them. You then give them an orientation on how to login when they start.
Review:
Time consuming.
Solutions:
We can have a guidebook that list all the steps that they need to login to their machine instead of giving personal orientation every time.

3. When a new computer is provisioned, you have to install lots of sales-specific applications manually onto every machine. This takes a few hours of your time for each machine.
Review:
Time consuming.
Solutions:
We can use configuration-management tools like puppet to handle this problem, so every time there’s a new software that need to be installed, we can just change the configuration in our configuration-management tools.

4. When someone has an IT-related request, they email you directly to help them.
Review:
Time consuming.
Solutions:
We can make a guidebook about what they need to check if there’s a certain problem related to their machine. So if they encounter some problem that actually happen because of some minor thing, they can solve it immediately.
If the problem is out of their scope of ability, then we need to make certain SOP about how to email those problems to me. For example, they need to answer certain questions like “what type of error is it?”, “what steps did you follow?”, “what’s the expected result?”, and etc. So, I can troubleshoot it faster and only ask them a certain questions if I need it.

5. Almost all software is kept in-house, meaning that you’re responsible for the email server, local machine software, and instant messenger. None of the company’s services are kept on the cloud.
Review:
This could highly leads to human-error, because there are too much service to handle.
Solutions:
We really need to consider moving some services that isn’t really critical to the cloud service, like instant messenger. This way, I can really focus on maintaining services that essential to the company.

6. Customer data is stored on a single file server. When a new salesperson starts, you also map this file server onto their local machine, so that they can access it like a directory. Whoever creates a folder on this server owns that folder and everything in it. There are no backups to this critical customer data. If a user deletes something, it may be lost for everyone.
Review:
It’s really dangerous
Solutions:
We can need to have backup server that stores all of the company essential data. We can consider using cloud services to backup this data, so we don’t store all this data in one place. This way we can prevent data lost, because of catastrophic disasters that might happen. We can also use tool like Active Directory to manage distribution of our resource data to our employee. 
```

<br>

## Scenario 3

You’re doing systems administration work for Dewgood. Evaluate their current IT infrastructure needs and limitations, then provide at least five process improvements and rationale behind those improvements. Please write a 200-400 word process review for this consultation. Remember, there’s no right or wrong answer, but make sure to provide your reasoning.

**Non-profit Company**:

Dewgood is a small, local non-profit company of 50 employees. They hired you as the sole IT person in the company. The HR person tells you when they need a new computer for an employee. Currently, computers are purchased directly in a physical store on the day that an employee is hired. This is due to budget reasons, as they can’t keep extra stock in the store.

The company has a single server with multiple services on it, a file server, and email. They don’t currently have a messaging system in place. When a new employee is hired, you have to do an orientation with them for login. You’re also responsible for installing all the software they need on their machine, and mapping the file server to their computer. The computers are managed through Windows Active Directory. When an employee leaves, they’re currently not disabled in the directory service.

The company uses an open-source ticketing system to handle all internal requests as well as external non-profit requests. But the ticketing system is confusing and difficult to use, so lots of the employees reach out to you directly to figure out how to do things. In fact, so many things are difficult to find that employees typically ask around when they have a question.

There are nightly backups in place of the file server. You store this information on a disk backup and take it home with you everyday to keep it safe in case something happens onsite. There’s also a small company website that’s hosted on the single server at the company. This website is a single html page that explains the mission of the company and provides contact information. The website has gone down many times, and no one knows what to do when it happens.

**My Review**:
```
Problem that Dewgood has:
1. Currently, computers are purchased directly in a physical store on the day that an employee is hired. This is due to budget reasons, as they can’t keep extra stock in the store.
Review:
It matched their budget, but it decrease productivity
Solutions:
We can make an agreement with certain vendor about purchasing machines, so maybe we can reduce the cost and time that we need to find physical store to purchase it.
For the time being, we can consider using Virtual Machine that works in the cloud for the new employee as a temporary machine.

2. The company has a single server with multiple services on it, a file server, and email. They don’t currently have a messaging system in place.
Review:
These services can be moved to the cloud.
Solutions:
We can consider moving our services to the cloud, because cloud services cost exactly the amount of resources that we need. Because Dewgood is small organization, the cost of using cloud is maybe smaller than the cost of buying a new physical hardware to manage those services.

3. When a new employee is hired, you have to do an orientation with them for login. You’re also responsible for installing all the software they need on their machine, and mapping the file server to their computer. The computers are managed through Windows Active Directory. When an employee leaves, they’re currently not disabled in the directory service.
Review:
Time consuming.
Solution:
We can have guidebook about what they need to do to login and use their machine, instead of having a personal orientation every time there’s a new employee.
We can also have a script or an automated system which connect our employee database to our Active Directory to reduce human-error. So when an employee leaves, their account is automatically disabled.

4. The company uses an open-source ticketing system to handle all internal requests as well as external non-profit requests. But the ticketing system is confusing and difficult to use, so lots of the employees reach out to you directly to figure out how to do things. In fact, so many things are difficult to find that employees typically ask around when they have a question.
Review:
Time consuming
Solutions:
First of all, if that open-source ticketing system really hard to use, than we can consider to change it or we can modify it if we can.
We can include a guidebook or some pre-question in our ticketing system, that they need to answer and include in their message before send it to us. That can help us troubleshooting and respond their problem faster

5. There are nightly backups in place of the file server. You store this information on a disk backup and take it home with you every day to keep it safe in case something happen onsite. There’s also a small company website that’s hosted on the single server at the company. This website is a single html page that explains the mission of the company and provides contact information. The website has gone down many times, and no one knows what to do when it happens.
Review:
It’s dangerous
Solution:
We can consider backing up with cloud services if we can afford it instead of taking the disk every day.
For the company’s website the short-term solution, we can host it with virtual machine that run in the cloud or maybe some local machine that we have. As for the long-term solution, first we need to troubleshoot the problem to find it root cause. After that we can make post-mortems note that include when it happens, why it happens, what we do to fix it, and what we need to do to prevent this for happening again.
```
