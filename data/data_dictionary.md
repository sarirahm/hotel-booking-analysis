# Data Dictionary

## Dataset Overview

This dataset contains hotel booking records from both Resort Hotels and City Hotels. It includes information about booking details, customer demographics, reservation history, accommodation preferences, and booking outcomes. The dataset is used to analyze booking behavior, identify factors associated with reservation cancellations, understand customer characteristics, and support business decision-making in the hospitality industry.

## Data Dictionary

| Variable | Data Type | Definition |
|----------|-----------|------------|
| **hotel** | Categorical | Type of hotel where the reservation was made (H1 = Resort Hotel, H2 = City Hotel). |
| **is_canceled** | Binary | Indicates whether the reservation was canceled (1) or not canceled (0). |
| **lead_time** | Numerical | Number of days between the booking date and the guest's arrival date. |
| **arrival_date_year** | Numerical | Year of the guest's arrival date. |
| **arrival_date_month** | Categorical | Month of the guest's scheduled arrival. |
| **arrival_date_week_number** | Numerical | Week number of the year corresponding to the guest's arrival date. |
| **arrival_date_day_of_month** | Numerical | Day of the month on which the guest is scheduled to arrive. |
| **stays_in_weekend_nights** | Numerical | Number of weekend nights (Saturday and Sunday) included in the reservation. |
| **stays_in_week_nights** | Numerical | Number of weekday nights (Monday to Friday) included in the reservation. |
| **adults** | Numerical | Number of adult guests included in the reservation. |
| **children** | Numerical | Number of child guests included in the reservation. |
| **babies** | Numerical | Number of infant guests included in the reservation. |
| **meal** | Categorical | Meal package selected for the reservation (e.g., BB, HB, FB, or no meal package). |
| **country** | Categorical | Guest's country of origin represented using ISO country codes. |
| **market_segment** | Categorical | Market segment through which the reservation was made (e.g., Direct, Corporate, Travel Agent, Tour Operator). |
| **distribution_channel** | Categorical | Distribution channel used to complete the reservation (e.g., Direct, Travel Agent, Tour Operator). |
| **is_repeated_guest** | Binary | Indicates whether the guest has previously stayed at the hotel (1) or is a first-time guest (0). |
| **previous_cancellations** | Numerical | Number of previous reservations canceled by the guest before the current booking. |
| **previous_bookings_not_canceled** | Numerical | Number of previous reservations successfully completed without cancellation. |
| **reserved_room_type** | Categorical | Code representing the room type originally reserved by the guest. |
| **assigned_room_type** | Categorical | Code representing the room type assigned to the guest upon check-in. |
| **booking_changes** | Numerical | Number of modifications made to the reservation before check-in or cancellation. |
| **deposit_type** | Categorical | Type of deposit used to guarantee the reservation (No Deposit, Non Refund, or Refundable). |
| **agent** | Numerical | Unique identifier of the travel agency responsible for the reservation. |
| **company** | Numerical | Unique identifier of the company or organization responsible for the reservation or payment. |
| **days_in_waiting_list** | Numerical | Number of days the reservation remained on the waiting list before being confirmed. |
| **customer_type** | Categorical | Customer classification based on the booking type (Contract, Group, Transient, or Transient-Party). |
| **adr** | Numerical | Average Daily Rate (ADR), calculated as the average lodging revenue earned per occupied room per night. |
| **required_car_parking_spaces** | Numerical | Number of parking spaces requested by the guest. |
| **total_of_special_requests** | Numerical | Total number of special requests made by the guest, such as room preferences or additional amenities. |
| **reservation_status** | Categorical | Final status of the reservation (Check-Out, Canceled, or No-Show). |
| **reservation_status_date** | Date | Date on which the reservation status was last updated. |

## Data Types

| Data Type | Description |
|-----------|-------------|
| **Categorical** | Variables containing labels or categories. |
| **Numerical** | Variables containing quantitative values that can be measured or calculated. |
| **Binary** | Variables containing only two possible values (0 and 1). |
| **Date** | Variables representing calendar dates. |

## Notes

- The dataset contains reservations from two hotel types: **Resort Hotel (H1)** and **City Hotel (H2)**.
- Some variables, such as **agent**, **company**, **reserved_room_type**, and **assigned_room_type**, are anonymized using identifiers or codes to protect privacy.
- Missing values may exist in several variables (e.g., `agent`, `company`, `children`, and `country`) and should be handled appropriately during data cleaning.
- The target variable for predictive or exploratory analysis is **`is_canceled`**, which indicates whether a reservation was canceled.