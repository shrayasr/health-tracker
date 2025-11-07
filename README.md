# Health Tracker

> [!NOTE]
> This README and the project was vibe coded with Claude Code

A Progressive Web App (PWA) for tracking blood pressure and blood sugar levels. Built with vanilla JavaScript, Bootstrap 5, and Chart.js for a lightweight, responsive, and offline-capable experience.

## Features

- **Multi-Person Tracking**: Record health metrics for multiple people with autocomplete name suggestions
- **Dual Metric Support**: Track both blood pressure (systolic/diastolic/pulse) and sugar levels
- **Interactive Charts**: Visualize health trends over time with responsive line charts
- **Data Management**:
  - Edit existing records
  - Void/unvoid records without deletion (maintains data integrity)
  - Filter by metric type (BP or Sugar)
  - Adjustable record display limits (10, 20, 50, or 100 records)
- **Export Functionality**: Download all data as CSV for external analysis
- **Offline Support**: Works offline as a PWA with service worker caching
- **Responsive Design**: Mobile-friendly interface that works on all devices
- **Local Storage**: All data stored locally in your browser for privacy

## Demo

![Health Tracker Interface](_index.html)

## Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- No build tools or dependencies required

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/health-tracker.git
   cd health-tracker
   ```

2. Open `_index.html` in your web browser, or serve it with any local web server:
   ```bash
   # Using Python
   python -m http.server 8000

   # Using Node.js
   npx http-server
   ```

3. Install as a PWA (optional):
   - Open the app in your browser
   - Click the "Install" button in the address bar
   - The app will be available as a standalone application

## Usage

### Recording a Measurement

1. Enter the person's name (or select from previous entries)
2. Choose measurement type (Blood Pressure or Sugar Level)
3. Fill in the appropriate values:
   - **BP**: Systolic, Diastolic, and Pulse
   - **Sugar**: Sugar level in mg/dL
4. Date and time are auto-populated but can be adjusted
5. Add optional remarks
6. Click "Save Record"

### Viewing History

- **Charts**: Visual trends displayed at the top of the history section
- **Table**: Detailed records shown below charts
- **Filtering**: Use the dropdown to show only BP or Sugar records
- **Pagination**: Adjust how many records to display at once

### Managing Records

- **Edit**: Click "Edit" to modify a record
- **Void**: Mark a record as void (appears struck-through but remains in database)
- **Export**: Download all data as CSV file

## File Structure

```
health-tracker/
├── _index.html       # Main application file
├── manifest.json     # PWA manifest configuration
├── sw.js            # Service worker for offline support
├── icon-192.png     # PWA icon (192x192)
├── icon-512.png     # PWA icon (512x512)
├── LICENSE          # MIT License
└── README.md        # This file
```

## Technologies Used

- **HTML5**: Semantic markup
- **CSS3**: Custom styles with gradients
- **JavaScript (ES6+)**: Vanilla JS for application logic
- **Bootstrap 5.3.2**: Responsive UI components
- **Chart.js 4.4.0**: Data visualization
- **LocalStorage API**: Client-side data persistence
- **Service Workers**: PWA offline functionality

## Data Privacy

All health data is stored locally in your browser's localStorage. No data is sent to any server or third party. Your information stays on your device.

To backup your data, use the "Export CSV" feature regularly.

## Browser Compatibility

- Chrome/Edge: Full support
- Firefox: Full support
- Safari: Full support (iOS 11.3+)
- Opera: Full support

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

Shrayas Rajagopal

## Acknowledgments

- Bootstrap team for the excellent UI framework
- Chart.js team for the charting library
- The open-source community

## Future Enhancements

Potential features for future versions:
- Data import from CSV
- Medication tracking
- Reminder notifications
- Data sync across devices
- Additional health metrics (weight, temperature, etc.)
- Statistics and health insights
- Dark mode toggle
- Multiple language support

## Support

If you encounter any issues or have suggestions, please open an issue on GitHub.
