## AstroBookings 
> Demo project for the course "From Vibe Coders to AI-Native Engineers".

A system comprising a **backend API** and a **frontend WebApp** designed for managing space travel bookings.
 
- Rockets have limited seat capacity and a specific operational range.
- Launches are scheduled by associating them with a rocket on a future date.
- Each launch sets a price per seat and a minimum required occupancy threshold.
- The lifecycle of a launch contemplates the sequential states: `scheduled` → `confirmed` → `successful`.
- A launch can transition to `suspended` due to low occupancy or `canceled` due to technical causes.
- Users (identified as operators or passengers) register using their email address and name.
- Operators manage the registry of rockets and launches, including handling cancellations and suspensions.
- Passengers can formalize personal bookings for launches with available seats.
- Payments and refunds (resulting from a suspension or cancellation) are processed through a mock transactional gateway.

---

> [!WARNING]
> AstroBookings is a fictional space travel company.
> The system is designed for demonstration and training purposes. 
> Not for production use; 
> No security is required at the initial stage.

---

Apart from the domain, the demo must also weave in transversal concerns and at least one structural refactoring and a one business modification.

- Logs / observability, centralized error handling, helper libraries.
- A significant implementation change — e.g. DTO→Value Object, centralized logging, result pattern.
- A one business modification — e.g. launch cancellation reason and fee. lauches scheduling with time restictions for the same rocket.

> [!NOTE]
> The demo plan must be independent of the technology. When I record or deliver it live, I will land it on a specific stack.