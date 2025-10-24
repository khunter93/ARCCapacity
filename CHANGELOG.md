# Changelog

All notable changes to the ARC Call Capacity Dashboard will be documented in this file.

## [1.1] - 2025-10-24

### Added
- Mobile-responsive card layout for screens under 800px width
  - Cards show week, status, remaining capacity, and utilization
  - Cleaner, more compact view optimized for mobile devices
- Refresh button with minimalist icon design
  - Subtle hover effect (Gmail-style highlighting)
  - Spinning animation during data reload
  - Located in top right of card area
- Minimalist SVG icons for theme toggle
  - Sun and moon icons in black/white
  - Replaced emoji-based icons
  - Smooth hover scaling effect

### Changed
- Busy capacity threshold updated from 90% to 85%
  - Affects status indicators, color coding, and filters
- Theme toggle repositioned to header top right
- Timestamp relocated to footer (bottom left)
  - Format changed to: "Month Day, Year, Time" (e.g., "October 24, 2024, 3:45 PM")
  - Removed seconds from display
- Light theme set as default on first load
  - User preference still remembered via localStorage

### Removed
- Filters (Week, Status, Search) hidden on mobile devices
  - Provides cleaner, more focused mobile experience
- Capacity and Workload fields removed from mobile cards
  - Reduces information density for better mobile readability

## [1.0] - Initial Release

### Features
- Real-time capacity dashboard connected to Google Sheets
- Weekly capacity tracking with utilization metrics
- Light/dark theme toggle with localStorage persistence
- Status indicators (Healthy, Busy, Max Capacity)
- Color-coded progress bars and status dots
- KPI cards showing:
  - Total weeks
  - Total capacity
  - Total workload
  - Average utilization
- Filtering and search capabilities:
  - Week dropdown filter
  - Status filter
  - Text search for weeks
- Desktop table view with sortable columns
- Auto-refresh with JSONP and CSV fallback loading
- Responsive design with mobile breakpoint at 800px
