# hassaanms-portfolio
A personal portfolio website built with HTML5 and CSS3 for INFR3120 (Web and Scripting Programming), Assignment 1, Fall 2026.

The site has four separate pages: Home, About Me, Projects, and Contact Me.

## Links
- Live Site: https://hassaanmuhammad-prog.github.io/hassaanms-portfolio/
- Repository link: https://github.com/hassaanmuhammad-prog/hassaanms-portfolio 

## File Structure
- `index.html` (Home page)
- `projects.html` (Projects page)
- `contact.html` (Contact page with validated form)
- `style.css` (Base stylesheet, mobile first)
- `tablet.css` (Styles for screens 768px and wider)
- `laptop.css` (Styles for screens 1024px and wider)
- `images/`, `videos/`, `documents/` (Media and documents)

## Pages

### Home (`index.html`)
- Welcome message and a short introduction, with a link to the Projects page
- Uses semantic tags: `header` (site name and navigation), `nav` (links to all four pages), `main` (page content), `section` (grouped content), and `footer` (contact email and copyright)
- The header and footer repeat on every page; only the `main` content changes
- Includes the viewport meta tag so the layout scales correctly on mobile devices
- Links to `style.css` for styling

### About Me (`about.html`)
_TODO_

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
_TODO: Results from W3C HTML validator, W3C CSS validator, W3C link checker, spell check, and WAVE accessibility test._

## External Code and Sources
_TODO: list any code from outside the lectures with the source and author. If none, state that all code is my own._

## Contact
- Email: [hassaan.muhammad@ontariotechu.net](mailto:hassaan.muhammad@ontariotechu.net)

