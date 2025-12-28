# GHCND & GSOD Station Statistics Tool

A web-based application for searching, tracking, and analyzing climate data from Global Historical Climatology Network - Daily (GHCND) and Global Summary of the Day (GSOD) stations.

## Project Requirements
- **Data Access**: Fetch and analyze temperature data (TMIN, TAVG, TMAX) from NOAA.
- **Station Management**: Search and filter thousands of stations via local text files (`ghcnd-stations.txt`, `isd-history.txt`).
- **User Authentication**:
  - Multi-level access (Basic, Advanced, Admin).
  - Invitation-only signup system.
  - Special visitor access via codes.
- **Analytics**:
  - Detailed temperature statistics (Min, Max, Avg, Explosive Power).
  - Consecutive record tracking.
  - Comparison with custom thresholds.
- **Privacy & Tracking**: Record visitor information (location, device, OS) for admin review.
- **Internationalization**: Full support for multiple languages via `translations.json`.

## Project Structure
```text
/
├── app.py                # Main Flask application logic & API endpoints
├── translations.json     # Multi-language text mapping
├── requirements.txt      # Python dependencies
├── ghcnd-stations.txt    # GHCND station lookup data
├── isd-history.txt       # GSOD station lookup data
├── static/
│   ├── script.js         # Frontend logic, data visualization, and interactions
│   └── style.css          # UI styling (Vanilla CSS)
└── templates/            # HTML structural templates
    ├── index.html        # Main dashboard
    ├── date_details.html # Detailed view for specific dates/records
    ├── stats.html        # Visitor statistics (Admin only)
    ├── login.html        # Authentication pages
    └── ...               # User/Invitation management views
```
