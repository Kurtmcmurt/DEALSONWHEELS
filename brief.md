Create a Web UI using Vue.js, with the following features:

- Display all vehicles the hire company has as returned from the all-vehicles REST service.

- Filter these vehicles to just those available for hire on a given day (defaulting to today), by
querying the available-vehicles REST service.

- A mechanism where the user can select a specific vehicle with a start and end date and then
call the hire-cost-calculation REST service, with the result displayed.

- The ability for the user to then proceed to make that booking/reservation, for a particular
customer, via the booking REST service.


You will need to stub/mock the REST endpoints to simulate the back-end services, and that your UI
implementation can call in place of a real running back-end. Returned data can be hard-coded; these
stubs are not expected to actually perform the business logic that the real back-end would execute.
The UI should consider usability, provide validation and user feedback where appropriate.

A vehicle has a number of attributes:
- Registration number
- Category of vehicle:
  - Small car
  - Estate car
  - Van
- Make
- Model
- Fuel type
  - Petrol
  - Diesel
- Price per day – this is based on the category of vehicle, and can be assumed to be
unchanging:
  - Small car - £25 / day
  - Estate car - £35 / day