# Pricing at Vocram Airways – Problem Summary

For the full problem statement, see Harvard Business Publishing Education:
- https://hbsp.harvard.edu/product/W13724-PDF-ENG
- https://hbsp.harvard.edu/product/W13725-PDF-ENG

This project explores the pricing challenges faced by an owner and pilot of a small floatplane charter business operating in Northern Ontario. With only three passenger seats available per flight and a growing mix of clientele, O’Rory must determine an optimal price to charge in order to maximize revenue without losing demand.

---

## Business Context
- Small floatplane charter service in Northern Ontario
- 3-passenger capacity
- Two flights per day (morning pickup, afternoon drop-off)
- First-come, first-served booking
- No cancellations or no-shows
- There are around 10-12 client calls that come in inquiring about prices before a departure


## Customer Mix
- 40% public-sector clients (e.g. researchers)
- 60% private clients (e.g. cottagers, professionals)
- Most bookings are for 1 seat

## Willingness to Pay
- Public clients: uniform distribution from $0–$100
- Private clients: uniform distribution from $0–$150
- Current price: $65 (same for both Public and Private)
- Customer type is unknown at booking

## Objective
- Maximize expected revenue
- Must choose a single price for both public and private customers
- Cannot observe client type in advance
- Limited to 3 seats per flight
- Is the current price of $65 the optimal price to maximize revenue?
---

## 🔄 Analytical Framework: Markov Chain

To model the booking process under uncertainty, O’Rory turns to a **Markov Chain model**:
- Each incoming call is a **random customer** with a **random willingness to pay**
- There are **10 seat states**, defined by different combinations of public/private bookings (e.g., 2 public clients + 0 private clients, or 2 public clients + 1 private client)
- A **transition probability matrix** shows the probability that one state (e.g., 2 public clients + 0 private clients) will transition to another state (e.g., 2 public clients + 1 private client) after a single call.
- Once all calls are processed or seats are filled, total revenue is calculated

This framework helps O’Rory estimate **expected revenue** for different pricing levels under uncertainty.

---

See the PowerPoint for a detailed explanation on how the solution is constructed. The code shows the solution being implemented.
