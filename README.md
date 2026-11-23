# Ticket Cancellation Coupon Analysis

Do customers who use a coupon cancel their tickets more often? An analysis of 101,017 ticket bookings.

## Data
Travel-ticket booking data from Kaggle, as used in the notebook [Travel Ticket Cancellation Classification & EDA](https://www.kaggle.com/code/rayyaghausrahmat/travel-ticket-cancellation-classification-eda) (101,017 bookings, 22 columns). It is not included here because it has personal-identifier columns (hashed emails, mobile numbers and national codes). Download it and save it as `data/train_data.csv`.

## Method
Loaded and inspected the bookings, flagged each booking as having a coupon or not, and compared cancellation rates between the two groups with a grouped mean and a bar chart (pandas, Seaborn).

## Result
| Group | Cancellation rate |
|---|---|
| Coupon | 15.03% |
| No coupon | 15.17% |

Coupon holders cancel no more often than everyone else: a difference of about 0.14 percentage points. This is a null result, but a useful one: coupons do not appear to make people cancel more. The analysis is descriptive and does not include a significance test.

## Run it
```bash
pip install -r requirements.txt
jupyter notebook ticket_cancellation_coupon_analysis.ipynb
```
