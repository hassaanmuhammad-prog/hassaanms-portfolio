# hassaanms-portfolio
100928683
Hassaan Muhammad

A personal portfolio website built with HTML5 and CSS3 for INFR3120 (Web and Scripting Programming), Assignment 1, Fall 2026.

The site has four separate pages: Home, About Me, Projects, and Contact Me.

## Links
- Live Site: https://hassaanmuhammad-prog.github.io/hassaanms-portfolio/
- Repository link: https://github.com/hassaanmuhammad-prog/hassaanms-portfolio 

## File Structure
- `index.html` (Home page)
- `about.html` (About Me page with photo and intro video)
- `projects.html` (Projects page)
- `contact.html` (Contact page with validated form)
- `style.css` (Base stylesheet, mobile first)
- `tablet.css` (Styles for screens 768px and wider)
- `laptop.css` (Styles for screens 1024px and wider)
- `images/` (Profile photo and video poster)
- `videos/` (Introduction video)
- `documents/` (Documents)
- `README.md` (This file)

## Pages

### Home (`index.html`)
- Welcome message and a short introduction, with a link to the Projects page
- Uses semantic tags: `header` (site name and navigation), `nav` (links to all four pages), `main` (page content), `section` (grouped content), and `footer` (contact email and copyright)
- The header and footer repeat on every page; only the `main` content changes
- Includes the viewport meta tag so the layout scales correctly on mobile devices
- Links to `style.css` for styling

### About Me (`about.html`)
- My own photo and a short introduction in a `section` with its own `h2` heading
- A second `section` with an embedded introduction video (about 60 seconds) using the HTML5 `video` element
- The video has the `controls` attribute so visitors can play, pause and change the volume, and a `poster` image that shows before it plays
- The photo and video are scaled with CSS so they shrink on small screens


### Projects (`projects.html`)
- Four projects, each in its own `article` with a heading and a short description
- A `section` with its own `h2` heading groups the projects, and each project title is an `h3`
- Project cards have a sage background, and sit two per row on tablet and wider screens

### Contact Me (`contact.html`)
- Form with name, email, cell number, comments, and a submit button
- Validation uses HTML5 attributes: `required`, `type="email"` for the email, a `pattern` for the phone number (format 905-555-1234), and `minlength` and `maxlength` for text fields
- No server is connected, so the form demonstrates the layout and validation only

## Responsive Design (Viewports)
The site uses fluid sizing (percentages, rem units and max-width) plus three stylesheets that load by screen width. No flexbox is used anywhere.

|  View  |      Width     |   CSS file   | Reason                                                                                 |
|--------|--------------- |--------------|----------------------------------------------------------------------------------------|
| Mobile |  under 768px   | `style.css`  | Base styles, written mobile first so small screens get a simple single column layout   |
| Tablet |  768px and up  | `tablet.css` | 768px is the width of a portrait tablet; project cards sit two per row                 |
| Laptop |  1024px and up | `laptop.css` | 1024px is a common small laptop width; wider content column, larger text and nav links |

## Gradients
- Linear gradient: the header on every page, running left to right from `#0E331B` to `#285438` (`style.css`).
- Angled linear gradient: the footer on every page, at 135 degrees from `#285438` to `#0E331B` (`style.css`).

## Colour Scheme
Using a monochromatic green scheme created with Adobe Color. Text uses neutral black or white for readability.
- https://color.adobe.com/create/color-wheel?color-palette=ADEEC5%2CA2BAAB%2C5B876B%2C285438%2C0E331B&color-palette-name=My+Color+Theme

|    Colour  |     HEX  |                  Used for                     |
|------------|----------|-----------------------------------------------|
| Mint       | `#ADEEC5`| Page background                               |
| Sage Grey  | `#A2BAAB`| Cards and form background                     |
| Mid Green  | `#5B876B`| Borders and Dividers                          |
| Forest     | `#285438`| Navigation background, gradient colour        |
| Dark Green | `#0E331B`| Header and footer background, gradient colour |

## Testing and Validation
- **W3C HTML validator:** pages validated with no errors or warnings. TODO: confirm `about.html` too.
- **W3C CSS validator:** `style.css`, `tablet.css` and `laptop.css` validated with no errors.
- **W3C link checker:** TODO: run on the live site and record the result.
- **Spell check:** TODO: run the Code Spell Checker extension in VS Code and record the result.
- **WAVE accessibility:** no errors and no contrast errors. One alert ("possible heading") on the site name in the header. It is intentionally a paragraph, because each page has a single `h1` inside `main`. TODO: confirm `about.html` too.

## External Code and Sources
Parts of the HTML and CSS in this project (including the contact form, the tablet and laptop stylesheets, and some styling rules) were written with help from Claude, an AI assistant by Anthropic, and then adapted by me. I reviewed this code and can explain how it works. No code was copied from other websites. The colour palette was made with Adobe Color.

## Contact
- Email: [hassaan.muhammad@ontariotechu.net](mailto:hassaan.muhammad@ontariotechu.net)
