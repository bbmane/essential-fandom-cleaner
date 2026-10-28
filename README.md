# Essential Fandom Cleaner

I was tired of Fandom wikis wasting half of my screen on sidebars, widgets, Discord boxes and sign-in banners while I just wanted to *read the article*. This userstyle strips all of that away and gives the content the full width of the page, for a much cleaner and more focused reading experience.

Works best with ads blockers.

## What it does

- **Removes the right rail** (Discord widget, right-side Guide / Navigator, ads and other wiki-specific modules)
- **Removes the left global navigation** (Home, Explore, Saved, Progress, History, Utilities, Settings, More...)
- **Hides edit & save clutter**: the floating edit/save side tools, the page header actions, the `[edit]` links next to section headings and the wiki tools button group
- **Hides the community navigation bar and the footer**, and trims the top bar down to just the search field
- **Expands the main column to full width**, removes the leftover margin of the side navigation and the column gap left behind by the right rail
- Makes the wiki header background span the whole page width, so it doesn't look cropped

## Before / After

| Before                                      | After                                      |
| ------------------------------------------- | ------------------------------------------ |
| ![Before](https://i.imgur.com/vmmJ4rA.png) | ![After](https://i.imgur.com/d2jktJj.png) |

> [!WARNING]
> The style also hides the **Sign in / Create account** buttons and every **Edit** button. This script is made for normal users, not editors. If you need to log in or edit a page, just disable the style for a moment from the Stylus popup.

> [!NOTE]
> Fandom changes its markup every now and then. If something starts showing up again (or something you wanted disappears), a selector probably got renamed.

## Installation

1. Install a userstyle manager such as [Stylus](https://add0n.com/stylus.html).
2. [Click here to install the style](https://raw.githubusercontent.com/bbmane/essential-fandom-cleaner/main/main.user.css).
3. Visit any Fandom wiki page — the clutter will be gone automatically.

## Customization

Every rule is just a CSS selector in a single `display: none !important` list, so tweaking the style is easy. Remove a selector from the list to bring that element back:

| Selector | What it hides |
| -------- | ------------- |
| `.page__right-rail`, `.right-rail-wrapper`, `.right-rail-toggle`, `#WikiaRail` | Right sidebar and its toggle |
| `.global-explore-navigation` | Left global navigation (Home, Explore, Saved...) |
| `.page-side-tool.page-side-edit`, `.page-side-tool.page-side-save` | Floating edit / save buttons |
| `.page-header__actions`, `.wiki-tools.wds-button-group` | Page header actions and wiki tools |
| `.mw-editsection` | `[edit]` links next to section headings |
| `#community-navigation` and its children | Community navigation bar |
| `#global-top-navigation > div.global-top-navigation__action-wrapper` | Sign in / Create account buttons |
| `body > div.main-container > footer`, `#mw-data-after-content` | Footer and after-content data |

## Compatibility

- Works with any Fandom wiki on the modern (Fandom Design System) skin
- Tested with Stylus on Chromium-based browsers and Firefox

##

<sub>Star this repo if you like the project :)</sub>
