# 🐾 PawPoint Vet

A small website that connects vet clinics with pet owners online.

## Why I made this

Most vet clinics still get clients through phone calls and ads on notice boards. That only reaches so many people, which means fewer visits and less money per day. Also, a lot of pet health records live on paper cards that get lost.

So the idea is simple: put the clinic online. Owners can see services, book a visit, check their place in the queue, and look at their pet's health history from their phone. Clinics reach more people and keep cleaner records.

This is a front-end project, so it's only HTML and CSS. Nothing actually submits or saves. It's all static pages that show how the thing would look and work.

**Live site:** [https://noahmuthama.github.io/git_project/]

## Pages

| File | What it is |
|------|------------|
| `index.html` | Home page: hero, stats, popular services, how it works, vets, testimonials |
| `services.html` | Listing of 6 services as cards, with search and filters (visual only) |
| `service-detail.html` | Full detail for the General Check-up |
| `book.html` | Booking form in 3 sections, with one example error |
| `confirmation.html` | Success message and booking details |
| `dashboard.html` | Owner dashboard: active appointment, queue summary, history, empty state |
| `status.html` | Live queue status, with every status shown as an example |
| `staff.html` | Staff dashboard with a sidebar and a 12-row queue table |

## How to run it

No setup needed.

1. Download or clone the repo
2. Open `index.html` in your browser
3. Click around

Images live in an `images/` folder. If you see broken image icons, that's just because the photos haven't been added yet.


## Style guide

I kept the CSS cheap and simple on purpose. Every page has the same CSS pasted inside a `<style>` tag, so any page works on its own. All the colours are CSS variables at the top of the file.

### Colours

| Name | Hex | Used for |
|------|-----|----------|
| Primary | Forest green | Header, buttons, links |
| Primary dark | `#1b4332` | Button hover |
| Secondary | `#f4a300` | Accent, focus outline, call to action buttons |
| Background | `#faf8f3` | Page background |
| Text | `#222222` | Main text |
| Muted | `#666666` | Small and less important text |
| Success | `#d8f3dc` | Success messages, confirmed badge |
| Warning | `#fff3cd` | Warnings, waiting badge |
| Error | `#f8d7da` | Errors, cancelled badge |

### Typography

- Font: Arial, sans-serif
- Headings: h1 `1.8rem`, h2 `1.4rem`, h3 `1.1rem`, all bold
- Body text: `1rem`
- Small text: `0.85rem`, muted grey
- Big numbers (stats, queue): `2.2rem` bold

### Buttons

| Type | Look | 
|------|------|
| Primary | Green background, white text |
| Secondary / outline | White background, green border and text |
| Hover | Darker green |
| Focus | 3px amber outline |
| Disabled | Grey, `not-allowed` cursor |

Header and closing call to action buttons use the amber accent so they stand out.

### Cards

- 1px grey border
- 6px rounded corners
- 12px padding
- White background
- No shadow (keeping it cheap)

### Status badges

Every badge has text and a symbol, so colour is never the only clue.



## Responsive design

I used plain CSS media queries, not a framework.

- **Mobile (600px):** one column. The nav wraps so it fits the screen. The staff sidebar sits on top of the page.
- **Tablet (768px):** two column grids. The hero splits into text and image.
- **Desktop (1000px+):** three and four column grids. The staff page gets a sidebar next to the table.
- Wide tables sit inside a `.scroll` box so they scroll sideways instead of breaking the page.

## Accessibility

- Semantic HTML: `header`, `nav`, `main`, `section`, `article`, `aside`, `footer`, `form`, `fieldset`, `table`
- One `h1` per page and no skipped heading levels
- Every form input has a visible `<label>`
- The form error uses `aria-describedby` and text
- Images have real alt text
- Button and link text says what it does ("Book a Visit", not "Click here")
- Every interactive element has a visible focus outline

## Things to know

- The form does not submit. The "Confirm Appointment" button just links to the confirmation page.
- Search and filters on the services and staff pages are visual only.
- All names, numbers, prices (in KES) and contact details are made up.
- The clinic is fictional.

## What I'd add next

- A backend so bookings and records actually save
- Real login for owners and staff
- Printable or downloadable pet health records
- SMS reminders for appointments

## Credits

Built by Noah for 