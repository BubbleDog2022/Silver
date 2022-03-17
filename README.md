Original App Design Project - README Template
===

# GoldHelper

## Table of Contents
1. [Overview](#Overview)
1. [Product Spec](#Product-Spec)
1. [Wireframes](#Wireframes)
2. [Schema](#Schema)

## Overview
### Description
Remind students of their pass times and empty spots of desired classes and provide them with the past feedbacks about a class. Could be used for course rushing or decision making during pass times.

### App Evaluation
[Evaluation of your app across the following attributes]
- **Category:** Education
- **Mobile:** This app is developed for mobile only
- **Story:** Help students to rush into demnanded classes. Students can see the past feedbacks of a class before making decisions. 
- **Market:** Any UCSB undergraduate could use this app.
- **Habit:** This app could be used as the user's pass time is approaching
- **Scope:** This app is primarily based on gold. It has the potential to combine some of the functions of Gauchospace and other ucsb websites, and thus has a wider scope. 

## Product Spec

### 1. User Stories (Required and Optional)

**Required Must-have Stories**

* User logs in to access registeration data for further actions
* User sets an alarm to inform the pass time
* Real-time tracking of empty spots
* User views the past feedbacks about a class

**Optional Nice-to-have Stories**

* Show a list of hot electives based on past data
* hightlight 8 am classes

### 2. Screen Archetypes

* Login
   * User logs in with their UCSB Id and password
* Home
   * User can see a welcome message
* Tracking page 
   * User can see the courses in track
* Settings
   * User can set whether to inform him or her when the pass time comes
* Course search
   * Type course number to search a course
* Course info.
   * Display the ratings of the professor
   * Allow the user to keep track of the empty spots

### 3. Navigation

**Tab Navigation** (Tab to Screen)

* Home
* Tracking
* Settings
* Course search

**Flow Navigation** (Screen to Screen)

* Forced Log-in -> Authentification -> Home
* Course search -> Course info.

## Wireframes
[Add picture of your hand sketched wireframes in this section]
<img src="wireframes.png" width=600>

### [BONUS] Digital Wireframes & Mockups

### [BONUS] Interactive Prototype

## Schema 

### Models
#### Student

   | Property      | Type     | Description |
   | ------------- | -------- | ------------|
   | studentId      | int   | unique id for the student |
   | name        | String | full name of the student |
   | courses         | pointers     | courses in track |
   
#### Course

    | Property    | Type   | Description | 
    | ----------- | ------ | ----------- | 
    | courseId    | int    | unique id for the course |
    | name        | String | name of the course |
    | instructor  | String | instructor of the course |
    | rate | float | rate of the course |
    | description | text | official description of the course |
    | comments | pointers | comments from previous iteration of the course |
### Networking
