GLITCHWAYVE — DASHBOARD REDESIGN

FILES
- index.html: page structure and external library references
- style.css: screenshot-inspired layout, responsive behavior, and building themes
- script.js: existing app logic with the updated desktop navigation and home dashboard

INSTALLATION
1. Make a backup of your current index.html, style.css, and script.js.
2. Extract this ZIP file.
3. Replace the three existing files in your Glitchwayve project with these versions.
4. Open index.html through your usual local server or hosting setup.

DESIGN CHANGES
- Desktop navigation is now a horizontal rounded navigation bar.
- The home page uses four summary cards, a quick-access strip, and a two-column recent-activity/detail panel.
- The recent-activity list is populated from the signed-in student's existing requests, appointments, room bookings, and equipment-borrowing records.
- Clicking an activity item updates the detail panel.
- The dashboard now opens in dark mode with charcoal surfaces and high-contrast text.
- Interweave uses gold neon accents; Glitch Tower uses violet/purple neon accents.
- Panels and cards glow subtly in the active building color when hovered or focused.
- The redundant search icon was removed from the top bar; Find a service and Quick access Search remain available.
- The layout adapts to tablet and mobile screens; the mobile bottom navigation is retained.

IMPORTANT
- Your Supabase URL and publishable key remain in script.js as in your supplied file.
- Keep Row Level Security enabled and make sure the table policies are configured for student-owned records.
- The redesign does not create demo activity records. Summary counts and activity details come from the logged-in student's Supabase records.
- I also corrected the existing services query filter from .eq("is_active, true") to .eq("is_active", true), so the active-services filter passes the column and value separately.
