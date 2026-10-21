# NoteStack curriculum architecture

## Non-negotiable delivery rules
- Course listings are not course completion.
- Each published lesson needs original explanatory prose, a worked example, an instructional visual, a meaningful exercise, a topic-specific knowledge check, and a verifiable outcome.
- Unwritten lessons must be marked planned, never rendered as generated filler.
- Each course has its own syllabus, not six generic identical modules.
- Progress is tied to stable lesson IDs; avoid incompatible per-page storage keys.
- Deep links and navigation must work on GitHub Pages under /Note-stack/.
- Screenshots must be checked at 360px, 768px and desktop before declaring UI done.
- No copying All CS Notes source, artwork, branding or prose.

## Planned content schema
```json
{
  "course": {
    "id": "playwright",
    "title": "Playwright Testing",
    "category": "Web Development",
    "level": "Beginner to Advanced",
    "modules": [
      {
        "id": "foundations",
        "title": "Browser testing foundations",
        "lessons": [
          {
            "id": "first-browser-test",
            "title": "Write your first reliable browser test",
            "status": "published",
            "objectives": [],
            "sections": [],
            "exercise": {},
            "quiz": [],
            "reviewed": false
          }
        ]
      }
    ]
  }
}
```

## Release gates
1. Build lesson engine and migrate both existing authored Playwright lessons without breaking links.
2. Publish coherent Playwright syllabus with topic-specific modules and lesson IDs.
3. Implement progress migration from current legacy localStorage keys.
4. Validate semantic HTML, route navigation, quiz scoring, persistence and mobile layout.
5. Complete each course's authored content and run a quality review before marking published.
6. Verify deployed GitHub Pages site, not just successful GitHub commits.

## Truthful current status
36 course outlines; two authored Playwright lessons, currently separate HTML pages. Remaining content is incomplete. This file is a technical contract, not a completion certificate.
