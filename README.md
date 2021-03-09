# Communicating-Ford-Bike-Data-Findings-
by Mina Atef

Dataset:

Ford GoBike is a regional public bicycle sharing system in the San Francisco Bay Area, California. Beginning operation in August 2013 as Bay Area Bike Share, the Ford GoBike system currently has over 2,600 bicycles in 262 stations across San Francisco, East Bay and San Jose. On June 28, 2017, the system officially launched as Ford GoBike in a partnership with Ford Motor Company.

Ford GoBike consists of a fleet of specially designed and locked into a network of docking stations throughout the city. The bikes can be unlocked from one station and returned to any other station in the system, making them ideal for one-way trips. The bikes are available for use 24 hours/day, 7 days/week, 365 days/year and riders have access to all bikes in the network when they become a member or purchase a pass.

Data wrangling process:

Drop unwanted columns['start_time', 'end_time', 'start_station_latitude', 'start_station_longitude', 'end_station_latitude', 'end_station_longitude', 'bike_id']
Change start_time and end_time to datetime format
Drop missing values
Drop abnormal member_birth_year values
Change duration_sec from seconds to Minutes
Change member_birth_year to member_age that contains the age values instead of birth year

Summary of Findings:

There are a lot more subscriber usage than customers.
User-wise, there are male riders more than female, and most members are subscribers compared to casual riders. Also most riders are around 25 to 40 years old.
Most rides are short and lasts up to 30 minutes, though there were some very long outliers like 24 hour rides.

Key Insights for Presentation:

Subscribers use the service for work that's why most trips were on work days (Mon-Fri) and especially during rush hours (when going to work in the morning and return home in the afternoon), whereas customers tend to ride for fun in the afternoon or early evenings over weekends. Subscriber users are slightly older than customer users who tend to take longer rides.
