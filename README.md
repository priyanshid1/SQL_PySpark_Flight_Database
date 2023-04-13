# SQL_PySpark_Flight_Database

On a relational flights database, enter multiple SQL queries. The Bureau of Transportation Statistics provided the data for this database, which spans the years 2005 through 2015. 

There are four tables in the database:

• Flights (fid, year, month_id, day_of_month, day_of_week_id, carrier_id, flight_num, origin_city, origin_state, dest_city, dest_state, departure_delay, taxi_out, arrival_delay, canceled, actual_time, distance)
• Carriers (cid, name)
• Months (mid, month)
• Weekdays (did, day_of_week)

In addition, however, you should impose the following constraints:
• The primary key of the FLIGHTS table is fid.
• The primary keys for the other tables are cid, mid, and did respectively.
• Flights.carrier_id references Carrier.cid
• Flights.month_id references Months.mid
• Flights.day_of_week_id references Weekdays.did
