# Turbo Challenge - Diego Salas

## Summary
This challenge was fun and frustrating at the same time. I enjoyed the constant eureka moments working with new tools and finding out about their capabilities. 

I had some learning experience with Django and had explored the Django Rest framework once so I felt more comfortable building the backend.

On the other hand, I had very little experience with React and none with Next Js/tailwind. I know typescript, javascript, html and css so I wasn't completely clueless but the frontend part was really hard.

The frustrating part was that I constantly found myself thinking "There must be a cleaner way to do this". Sometimes I digged deeper into it but other times I had to prioritize getting things done because of the time constraint.

I learned a lot during the challenge so I’m satisfied with my work. I completed most of the functional part, the section “Pending” has more detail on what I couldn’t do.


## Content
This repository contains two submodules that point to the backend and frontend repositories. 

The framework for backend was requested in the challenge constraints. I used SQLite to speed up the process of getting persistence working.

* Backend: Django REST framework localhost
* Database: SQLite - Django ORM

The framework for frontend was also requested. I decided to use tailwind although I’ve never used it because it was recommended in the next js documentation. I used Typescript because it is cleaner than javascript but because of the rush I feel I didn’t make good use of it.

* Frontend: NextJS + TypeScript + Tailwind

## AI Tools

I used Copilot integrated in Visual Studio Code with GPT 4o engine for code autocompletion and template generatin.

I used Google Gemini as an aditional tool to query about coding doubts and documentation material but also used google search engine for some especific querys and the frameworks and tools documentation websites.

## Pending

Features not implemented:

* Design improvement
* Auth service in backend
* Login with auth service
* Sing up with new user
* Create new user in backend
* API Security

Other tasks
* UX and performance tunning
* Code cleaning
* Front and backend README

## Task and time distribution

* 01/30 12:00 - Challenge received and confirmed.
* 01/30 15:40 - 01/30 16:30: Challenge started. Created log. Planning and analysis.
* 01/30 16:30 - 1/30 21:00 Created github repos for backend and frontend. Started frontend. First commit. Partial design.
* 01/31 11:00 - 01/31 13:45 Resumed design: Note editor and some other fixes. Finished design. Still needs work.
* 01/31 15:00 - 01/31 7:30 Started backend development. Setup django rest framework. Finished backend. Categories list and notes CRU available. Pending, return note count.
* 02/01 10:00 - 02/01 12:00 Started frontend/backend integration. Added category foreign key to notes in backend and extra data on endpoints (note count for categories, category name for notes). Added backend data to frontend dashboard.
* 02/01 15:00 - 02/01 19:30 Integrated note editor with backend. 
* 02/02 9:00 - 02/02 12:00 Testing and bug fixing. Preparing challenge material.

### Features listed

#### Backend: 
* Sign up
* Login
* Dashboard: List categories
* Dashboard: List notes
* Note editor: Note create/update


#### Frontend:
* Sign up form  
* Login form 
* Dashboard: Category list 
* Dashboard: header 
* Dashboard: Note list 
* Dashboard: Note
* Note editor: toolbar 
* Note editor: Note editor 

#### Data schema

##### Note:
	id (pk)
	title (str)
	body (str)
	updated (timestamp)
	created (timestamp)
	categoryId (int fk Category)

##### Category
	id (int)
	name (str)

##### User
    email (str)
    password (encrypted str)
	created (timestamp)
