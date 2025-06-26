# Database Playground

## Planning

### Objective

* Design and build a rich, flexible database schema as the core of the system.
* Practice, learn, revise, and experiment with database modeling, normalization, and querying.
* Explore and apply SDLC principles to a solo backend-focused project.

### Success Criteria (Done When)

* A well-structured, normalized database schema is created to support various domains.
* Random data can be generated and consistently inserted into the schema for testing.
* Core queries and data relationships (e.g., ownership, timelines, associations) work as intended.
* Example use cases (e.g., simulation, chat, media tracking) can be tested against the database without errors.

### Goal

Develop a general-purpose database that can support multiple real-life-inspired use cases, and use those applications to test and explore the database. This includes:
* A robust database schema with comprehensive domain coverage.
* Auto-generated test data to simulate real-world usage.
* Applications or simulations (optional and incremental) that:
  * Utilize the data (e.g., simulate life events via auto-sugoroku)
  * Interact with various domains (e.g., chat, media tracking)
  * Help evaluate and validate schema quality

### Scope

This system will cover the following domains:
* Personal information and identity
* Employment
* Property and real estate
* Finance and banking
* Media collections and metadata
* Communication (chat/messages)

### Constraints

This is a backend-focused project. Therefore:
* UI/UX is not a priority (CLI, SQL scripts, or minimal interfaces are sufficient).
* Data accuracy and realism are not required; randomly generated or synthetic data is acceptable.
* Implementation of simulations or user-facing systems is optional and meant to support testing, not be feature-complete.

## Requirement

# Statements

"Create a database with detailed information of multiple"

Data needed:
* Personal information and identity
  * ID
  * name
    * first, middle, last, and aliases (multiple)
  * gender
  * born and passed date
  * nationalities (multiple)
  * qualifications (including educations, licences, and certifications), with start and end date, result, and comments about the student
    * ID
    * name of the qualification
    * type
    * issuer
    * description
  * achievements (with ID, name, type, achived date, and description)
  * races
  * religions
  * spouses (multiple)
  * past spouses
  * childrens
    * father
    * mother
  * events (with name, type, start and end date, and description)
  * occupations (with employer, salary, role, department, company, and working locations)
  * past occupations (with start and end date)
  * bank accounts
  * properties owned (buildings)
  * lands owned
  * vehicles owned
  * media and series collections
  * mobile phone numbers
  * e-mail
  * permanent address (property)
  * description
* Employment
  * role
  * department
    * roles
  * company
    * ID
    * name
    * domains
    * departments
* Property and real estate
* Finance and banking
* Media collections and metadata
* Communication (chat/messages)

* person information
  * ID
  * name
    * firstname
    * lastname
    * middlename
    * aliases
  * gender
  * born date
  * passed date
  * nationalities
  * qualifications (including educations, licences, and certificates)
    * ID
    * qualification
    * start date
    * end date
    * result
    * comment
  * achievements
    * ID
    * achievement
    * description
    * achieved date
  * races
  * religions
  * childrens
  * description
  * events
  * occupations
    * employers
    * salary
    * role
      * description
    * department    
      * description
    * company
    * working locations
  * past occupations (same as occupation, except for past)
    * start date
    * end date
  * bank accounts
  * media and series collections
  * mobile phone numbers
  * e-mail
  * permanent address (property)
* race
  * ID
  * name
  * description
* religion
  * ID
  * name
  * description
* property
  * ID
  * name
  * type
  * location
  * address
  * owners
  * events
  * description
* location
  * ID
  * name
  * coordinate
    * latitude
    * longitude
  * state
  * country
  * postcode
  * owners
  * events
  * description
* vehicle
  * ID
  * name
  * type
  * owners
  * events
  * description
* company
  * ID
  * name
  * industries
  * departments
  * events
  * descritions
* qualification issuer
  * ID
  * name
  * type
  * company
  * events
  * description
* bank
  * ID
  * name
  * company
  * events
  * description
* bank account
  * ID
  * owners
  * balance
  * bank
  * events
* bank transactions
  * ID
  * from person
  * to person
  * amount
  * description
  * date
* media
  * ID
  * name
  * media category, can be of these categories:
    * video: animes, cartoons, movies, TV-series, shorts, etc.
    * audio: podcasts, musics, songs, ani-songs, etc.
    * reading: comics, mangas, light-novels, novels, magazines, etc.
  * type
    * anime, ani-songs, manga, etc.
  * content
  * creators
  * tags
  * description
* series
  * ID
  * name
  * medias
  * description
* qualification
  * ID
  * name
  * type
  * issued by
  * description
* event
  * ID
  * name
  * type
  * start date
  * end date
  * description
* conversation
  * ID
  * name
  * description
  * created on
  * created by
  * members
  * chats
* chat
  * from
  * to
  * date sent
  * text content
  * media
* achievement
  * ID
  * name
  * type
  * description

## Design

## Coding

## Testing

## Deployment

## Maintenance
