# Data Dictionary

## `data/bookings.csv`
| Column | Type | Description |
|---|---|---|
| booking_id | Character | Unique booking reference |
| booking_date | Date | Booking/session date |
| start_time | Character | Scheduled start hour in HH:MM format |
| facility_id | Character | Facility key linked to facilities.csv |
| sport | Character | Sport booked |
| duration_hours | Numeric | Reserved duration in hours |
| booking_status | Character | Completed, Cancelled or No-show |
| booking_channel | Character | Mobile App, Website or On-site |
| customer_type | Character | New or Regular |
| booking_fee | Numeric | Simulated booking fee in INR |
| cancellation_reason | Character | Reason for cancellation/no-show where recorded |

## `data/facilities.csv`
| Column | Type | Description |
|---|---|---|
| facility_id | Character | Unique facility key |
| facility_name | Character | Facility display name |
| area | Character | Simulated Kolkata area |
| primary_sport | Character | Main sport/facility category |
| bookable_units | Integer | Number of bookable courts/grounds |
| operating_hours_per_day | Integer | Assumed daily operating hours |
| hourly_rate | Numeric | Simulated hourly rate in INR |

## Data provenance
Both files are synthetic, created for this academic project using a fixed random seed. Names and locations are illustrative. They are not operational records from real facilities.
