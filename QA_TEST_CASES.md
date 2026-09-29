# Mobile QA Research Test Cases

## TC-01 — Create Note

Given the Notes app is open
And no note titled "Sage Test" exists

When the user creates a note with:
- Title: Sage Test
- Description: Testing mobile QA agent

Then a note titled "Sage Test" should appear in the notes list.


## TC-02 — Edit Note

Given a note titled "Sage Test" exists

When the user edits the note
And changes its title to "Sage Updated"

Then a note titled "Sage Updated" should appear in the notes list.


## TC-03 — Delete Note

Given a note titled "Sage Updated" exists

When the user deletes the note

Then "Sage Updated" should no longer appear in the notes list.


## TC-04 — Persistence

Given a note titled "Sage Test" has been created

When the application is terminated and launched again

Then "Sage Test" should still appear in the notes list.