text
# ParkPulse — Requirements and MoSCoW

## Product objective
Help shoppers find suitable parking, manage their parking session,
redeem shopping benefits and collect loyalty rewards.

## Prototype boundaries
- Fictional parking facilities and availability data
- Simulated payments
- Hypothetical retail partner offers
- No guaranteed reservations
- No real barrier control or charging integration

## Requirements

| ID | Requirement | Priority | Acceptance criterion | Status |
|---|---|---|---|---|
| REQ-01 | Users can select a shopping destination. | Must | The selected destination is displayed as the active search destination. | Planned |
| REQ-02 | The app displays parking facilities matching the destination. | Must | Only facilities assigned to the selected destination are displayed. | Planned |
| REQ-03 | Users can view tariffs, opening hours and entry height. | Must | The detail view matches the stored facility data. | Planned |
| REQ-04 | Simulated availability is clearly labelled. | Must | Every availability display includes a demo notice. | Planned |
| REQ-05 | Users can start and end a parking session. | Must | Ending a session records the end time and displays the calculated fee. | Planned |
| REQ-06 | Users can redeem a valid shopping discount code. | Must | A EUR 2 code reduces a EUR 6 parking fee to EUR 4. | Planned |
| REQ-07 | Users can complete a simulated payment. | Must | A successful simulation displays a payment confirmation. | Planned |
| REQ-08 | Parking, charging and discounts are displayed separately. | Must | The checkout shows each applicable cost component. | Planned |
| REQ-09 | Users can filter for EV charging facilities. | Should | Only facilities with the selected charging characteristics are displayed. | Planned |
| REQ-10 | Users can save their parking level and bay. | Should | Saved details remain available during the session. | Planned |
| REQ-11 | Users can view previous parking sessions. | Should | Completed sessions appear in the history. | Planned |
| REQ-12 | Users can scan a discount QR code. | Could | A supported demo QR code fills in the discount code. | Planned |
| REQ-13 | Users can filter by carsharing provider and parking purpose. | Could | Results distinguish allowed, prohibited and unknown suitability. | Planned |
| REQ-14 | Each eligible paid session earns exactly one stamp. | Must | Reloading payment confirmation creates no additional stamp. | Planned |
| REQ-15 | Six stamps unlock one free-parking voucher. | Must | The sixth eligible session issues exactly one voucher and resets the stamp counter. | Planned |
| REQ-16 | Users can view their stamp balance and vouchers. | Must | The rewards view reflects the recorded transactions. | Planned |
| REQ-17 | Failed payments do not consume a voucher. | Must | The voucher remains available after a failed payment. | Planned |

## Proposed reward rules
- One completed eligible paid parking session earns one stamp.
- Six stamps unlock one free-parking voucher.
- The proposed voucher covers parking charges up to EUR 10.
- Charging costs are excluded.
- Only one discount or voucher can be used per session.
- Reward sessions do not earn another stamp.
- The final amount cannot be negative.

## Won't have in this version
- Real payments
- Live occupancy feeds
- Guaranteed reservations
- Automatic number-plate recognition
- Barrier control
- Real charging control
- Ending carsharing rentals
