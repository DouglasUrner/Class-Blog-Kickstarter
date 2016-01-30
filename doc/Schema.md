* Post
  - ID
  - Author: user // Original creator
  - Body[]
  - Comments[]
  - Published: enum // {public, private, draft}

* Body
  - Revisions[]
  - Marks[]

* Revision
  - ID (link to Post or Comment)
  - Deleted: bool
  - Date: time
  - Title: string
  - Content (target of WYSIWYG editor)
  - Author: user  // Who made this change.

* Mark
  - ID (link to Post (or comment?))
  - User (who created the Like)
  - Date
  - Type: enum      // Flag, Like, Exemplar
  - SubType: enum   // Per Type (e.g., rude, not-constructive, off-topic)
  - Allowed: enum   // {yes, no, unchecked} allows control of Marks while
                    // maintaining history, I think we also need to track who
                    // decided to allow it.
