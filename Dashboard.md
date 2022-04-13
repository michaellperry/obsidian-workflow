## Open calls for speakers
```dataviewjs
let submitted =
  dv.pages('"Speaking/Speaker submission"')
    .file.outlinks;
let declined =
  dv.pages('"Speaking/Decline to submit"')
    .file.outlinks;
let callsForSpeaker =
  dv.pages('"Speaking/Call for speakers"');
let openCallsForSpeaker =
  callsForSpeaker
    .filter(c => !submitted.includes(c.file.link))
    .filter(c => !declined.includes(c.file.link));
dv.table(
  ["Event", "Deadline"],
  openCallsForSpeaker.map(c => [
    c.file.link,
    c.deadline
  ]).sort(a => a[1])
)
```
