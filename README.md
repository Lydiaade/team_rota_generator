# Team Rota Generation

## Context

This project has been created since it has become a chore to generate the team rota for the Sunday services.
It would be much easier if this could be generated by simply updating individual unavailability and then the code
outputs the rota for a specific time period.

## Requirements for rota generation (in order of prioritisation)

- [x] Can specify dates for generation between certain time periods
- [x] Exports csv file of rota with dates and individuals working
- [x] No-one does the same role back to back
- [x] Can exclude dates specified by individuals
- [ ] Equal working shifts - equal number total (if one can only work certain shifts reduced shifts)
  - [x] Count 2 of every position, if someone has done a role more than twice they are required a break from that role until all others have reached 2 then all is reset. This only applies if the individual can do all roles
  - [x] Give breaks after 3 shifts back to back
- [x] Extract dates for rota generation
- [x] Set date in the example format -> `Sunday 15th January 2023`

### Nice to Haves

- [x] Move team members to a csv file
- [x] Have people that work only certain roles e.g. Person X only on camera duty
- [x] Can exclude months for individual - if they go to uni
- [ ] Limit the rota generation to 3 months, confirm if user wants to proceed and generate for extended period
- [ ] Pull out roles and generate template csv file based on roles
- [ ] Export as a pdf file -> pretty pdf
- [ ] Avoid overwriting previous rota generated -> currently same file name is used
- [ ] Use of spare individual in case of emergency e.g. Person R emergency worker
- [ ] Configure special services if there are and assign additional role
- [ ] Generate positions based on number of equipment
- [ ] Use of probability to allocate members to shifts
- [ ] Consider previous rota and generate dates with the same rules
- [x] Only add dates of unavailability if after date.now()
- [ ] Add instructional guide of how to use system
- [ ] Send icalendar invites to members to ensure awareness of shifts

### Identified bugs
- The 3 weeks and then time off given does not work currently individuals are being given 4 week back to back shifts

### Big Goals
- Send out calendar invite with details of shift to member emails with respective shifts

### Practices to implement
- Test driven development, testing all lines of code
- Test coverage on the project
- Improved architecture of classes
