# PXN Investments Email Templates

## Project Overview

Static HTML email templates for PXN Investments (a trading name of Praetura Ventures Limited). These are transactional/lifecycle emails for their investor portal.

## Templates

| File | Purpose | Template Variables |
|------|---------|-------------------|
| `email-welcome.html` | Post cooling-off account activation — sent after self-certified HNW/sophisticated investor completes 24hr cooling-off period, granting access to restricted fund documentation on the website | `{{logo_url}}`, `{{first_name}}`, `{{login_url}}`, `{{unsubscribe_url}}` |
| `email-forgot-password.html` | Password reset request | `{{logo_url}}`, `{{first_name}}`, `{{reset_url}}`, `{{unsubscribe_url}}` |
| `email-password-reset.html` | Password change confirmation | `{{logo_url}}`, `{{first_name}}`, `{{portal_url}}`, `{{unsubscribe_url}}` |
| `email-cooling-off.html` | 24-hour COBS 4.12A cooling-off period confirmation — sent immediately after self-certification as HNW/sophisticated investor | `{{logo_url}}`, `{{first_name}}`, `{{investor_category}}`, `{{registration_date}}`, `{{cooloff_end_date}}`, `{{portal_url}}`, `{{unsubscribe_url}}` |

## Design System

### Color Palette (Olive/Lime Green)
- **Background (outer):** `#2F3020` (dark olive)
- **Header/Footer:** `#12120D` (near-black)
- **Body:** `#F9F7EF` (warm off-white)
- **CTA buttons:** `#FBFEA7` (lime/yellow-green) with `#12120D` text
- **Feature cards:** `#fdffdc` (pale lime)
- **Body text:** `#12120d`
- **Muted text (footer/labels):** `#979864` (olive grey)
- **Link accent:** `#9EA06A` (muted olive)
- **Footer links:** `#FDFFDC` (cream)

### Typography
- **Font:** Inter (Google Fonts), fallback: `-apple-system, 'Segoe UI', Helvetica, Arial, sans-serif`
- **Headings:** 28px, weight 700, letter-spacing -0.48px
- **Body:** 16px, weight 400, line-height 1.4, letter-spacing -0.48px
- **Footer:** 14px, weight 400

### Layout
- **Max width:** 600px
- **Body padding:** 40px (24px on mobile)
- **Border radius:** 8px on container (top on header, bottom on footer), 6px on buttons
- **CTA padding:** 16px 32px

### Email Compatibility
- MSO/Outlook VML roundrect fallbacks for buttons
- `role="presentation"` on all layout tables
- Responsive `@media` queries at 600px breakpoint
- Apple disable message reformatting meta tag
- Preheader text pattern for inbox preview

## Conventions

- All templates share identical header, footer, and legal disclaimer blocks
- Template variables use `{{double_brace}}` syntax
- Sign-off is always "The PXN Investments Team"
- New templates must include the FCA regulatory disclaimer and investment risk warning
- Copyright: `2025 PXN Group`
- Legal entity: Praetura Ventures Limited (FRN 817345, Company No. 11439791)
