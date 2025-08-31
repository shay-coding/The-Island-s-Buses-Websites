place route json files here

JSON Format Changes

The old JSON (first example) contained full timetable data alongside the route information. It included:
- A length field under the route object.
- A departures array for each direction, listing every departure time throughout the day.

The new JSON (second example) is designed for the updated tracking system. It removes unnecessary fields and keeps the structure lighter and easier to process. Key differences are:
- The length field has been removed.
- The departures arrays are no longer included.
- Stop lists for each direction remain the same, so the core route structure is unchanged.

In short:
Old format = full timetable (route metadata + stops + departure times).
New format = leaner (just route info and stops) for live tracking purposes.
