# ParkPulse — Use Cases

## UC-01: Find suitable parking

### Primary actor
Driver

### Goal
Select a suitable parking facility near a shopping destination.

### Preconditions
- The app contains fictional facility data.
- The user can select a destination.

### Main flow
1. The user selects a destination.
2. The app displays matching parking facilities.
3. The user optionally applies filters.
4. The app updates the results.
5. The user selects a facility.
6. The app displays its tariffs, opening hours and restrictions.

### Alternative flows
- No matching facilities: show a message and allow filter changes.
- Unknown availability: display "Unknown", not "Available".
- Simulated availability: display a clear demo notice.

### Result
The user has selected a facility.
No parking space has been reserved.

### Related requirements
REQ-01, REQ-02, REQ-03, REQ-04, REQ-09


## UC-02: Pay, redeem a benefit and earn rewards

### Primary actor
Driver

### Goal
Complete a parking session, apply an eligible benefit and pay.

### Preconditions
- A parking session has started.
- A tariff is assigned to the session.
- Demo discount codes and reward rules are configured.

### Main flow
1. The user ends the parking session.
2. The app calculates the parking fee.
3. The app displays parking and optional charging costs separately.
4. The user optionally chooses one discount or voucher.
5. The app validates the selected benefit.
6. The app displays the final amount.
7. The user starts the simulated payment.
8. The app confirms successful payment.
9. If the session qualifies, the app credits exactly one stamp.
10. If the stamp count reaches six, the app issues one voucher
    and resets the stamp counter.
11. The app displays the receipt and updated reward balance.

### Alternative flows
- Invalid or used discount: show a message and allow another choice.
- Failed payment: preserve the voucher and allow retry.
- Repeated confirmation: do not duplicate payment or reward records.
- Free-parking reward session: do not award another stamp.

### Result
The session has a recorded payment result.
Any reward changes are recorded exactly once.

### Related requirements
REQ-05, REQ-06, REQ-07, REQ-08,
REQ-14, REQ-15, REQ-16, REQ-17
