### Project Proposal: Exploratory Data Analysis of NYC Subway Stations and Entertainment Events at Madison Square Garden 

*Matteo Fortier*
16/06/21

**Framing Question:** What is the relationship between entertainment events hosted at Madison Square Garden and the foot traffic of surrounding subway stations in 2019?

Further exploratory questions include: What stations are least/most affected (if a relationship exists) by entertainment events? What are the times least/most affected? What is the distance range of effects?

**Purpose and Need:** COVID-19 restrictions are easing, and entertainment events are returning to normal frequencies and capacities. However, the virus may persist for a while longer, and people may still be fearful of gathering in large crowds, especially in poorly ventilated tight places such as a subway. It is valuable to analyse the relationship between entertainment events and the traffic of subways so that those who prefer to avoid large crowds can evaluate whether taking the subway at a station where an event is taking place is appropriate. This especially benefits high-risk individuals where crowds are a crucial consideration. This can also benefit event organisers who want to suggest alternative journeys to customers to maximise sales.

**Data Description:**

The following datasets will be used:

- MTA Turnstile Data - Used to measure the foot traffic of stations at a given day at a given 4 hour interval. Obtained via http://web.mta.info/developers/turnstile.html. 
- Past Concerts Archive for MSG - Used to obtain dates of when previous concerts were hosted at MSG. Obtained via https://www.concertarchives.org/venues/madison-square-garden--4?page=1&year=2019#concert-table

2019 data for the above datasets will be used with the assumption that 2019 is a more accurate representation of typical concert and travel behaviours. 

Initial events to be explored:

| Artist         | Tour                              | Date            |
| -------------- | --------------------------------- | --------------- |
| Elton John     | Farewell Yellow Brick Road (tour) | March 5 2019    |
| Fleetwood Mac  | An Evening with Fleetwood Mac     | March 11 2019   |
| Ariana Grande  | Sweetener World Tour              | June 18 2019    |
| Jonas Brothers | Happiness Begins Tour             | August 30 2019  |
| Cher           | He We Go Again Tour               | December 4 2019 |

MTA Data Surrounding the above dates will be explored.

The unit of analysis for this project will be the foot traffic (calculated via entries and exits) of a given station for a given day for a given 4 hour interval. This unit of analysis will potentially allow for a relationship to be observed when a concert is held at MSG. '34 St - Penn Station' will be a particular station to analyse. 

The station, date, time, entries and exits features of the MTA dataset are expected to be used. 

**Tools:**

- Ingesting the raw data into a SQLite database via the Quick Setup (Manual method may be used if required)
- Querying from the SQLite database into Python via SQLAlchemy and SQLite queries
- Database cleaning and aggregation via either SQLAlchemy or Pandas
- Exploratory data analysis via Pandas
- Findings will be visualised via matplotlib library (alternatively seaborn library)

**MVP Goal:**

A potential minimum viable product for the project:

A line graph comparison of foot traffic at '34 St - Penn Station' station on a typical day without a concert versus a day with a concert.

