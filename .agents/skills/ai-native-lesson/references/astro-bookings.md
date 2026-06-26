## AstroBookings 
 
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
 
> [!WARNING]
> AstroBookings is a fictional space travel company.
> The system is designed for demonstration and training purposes. 
> Not for production use; 
> No security is required at the initial stage.

---

Además del dominio  debemos incluir funcionalidades transversales (logs y observability, gestión de errores centralizada, librerías de ayuda...) y al menos un refactoring structural (un cambio importante en la implementación a mitad de curso, por ejemplo paso de dto a value object, uso de log centralizado, result pattern o similares )
El plan de la demo en el curso tiene que ser independiente de la tecnología. Cuando lo grabe o lo imparta en directo lo aterrizaré en un stack concreto. Pero, a priori, debe ser agnóstico del lenguaje/framework.