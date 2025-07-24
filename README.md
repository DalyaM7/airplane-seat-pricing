# Pricing at Vocram Airways – Problem Summary

This project explores the pricing challenges faced by an owner and pilot of a small floatplane charter business operating in Northern Ontario. With only three passenger seats available per flight and a growing mix of clientele, O’Rory must determine an optimal price to charge in order to maximize revenue without losing demand.

---

## Business Context
- Small floatplane charter service in Northern Ontario
- 3-passenger capacity
- Two flights per day (morning pickup, afternoon drop-off)
- First-come, first-served booking
- No cancellations or no-shows


## Customer Mix
- 40% public-sector clients (e.g. researchers)
- 60% private clients (e.g. cottagers, professionals)
- Most bookings are for 1 seat

## Willingness to Pay
- Public: uniform distribution from $0–$100
- Private: uniform distribution from $0–$150
- Current price: $65 (same for both Public and Private)
- Customer type is unknown at booking

## Objective
- Maximize expected revenue
- Must choose a single price for both public and private customers
- Cannot observe client type in advance
- Limited to 3 seats per flight
---

## 🔄 Analytical Framework: Markov Chain

To model the booking process under uncertainty, O’Rory turns to a **Markov Chain model**:
- Each incoming call is a **random customer** with a **random willingness to pay**
- There are **10 seat states**, defined by different combinations of public/private bookings
- A **transition probability matrix** is used to simulate how each call affects the booking state
- Once all calls are processed or seats are filled, total revenue is calculated

This framework helps O’Rory estimate **expected revenue** for different pricing levels under uncertainty.

---

