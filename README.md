# Edgenuity - Activities to Completion Calculator
A web-based calculator designed to help teachers plan and track their students' Edgenuity coursework across multiple classes. The calculator automatically accounts for weekends and school holidays to provide realistic daily activity targets.

## 🚀 Live Demo

Visit the calculator at: `https://juliebkhou.github.io/ActivitiesToCompletionCalculator/`

## ✨ Features

### Activity Tracking per Course
  - Quizzes (completed/total)
  - Tests (completed/total)
  - Exams (completed/total)
  - Essays/Assignments (completed/total)
  - Labs/Projects (completed/total)

### Multi-Course Support
- Support for up to 8 courses simultaneously
- Individual progress tracking for each course
- Automatic calculation of totals and remaining activities

### Smart Scheduling
- **Weekdays Only:** Calculations exclude weekends
- **Built-in School Holidays:**
  - October 6-10 (Fall Break)
  - November 24-28 (Thanksgiving Week)
  - December 22 - January 6 (Winter Break)
  - Lincoln's Birthday (February 12)
  - March 23 - April 3 (Spring Break)
  - All major US holidays

### 📈 Detailed Progress Reports
- Overall progress across all courses
- Individual course breakdowns with progress bars
- Daily activity targets for each course
- Visual progress tracking with percentages

## 🎯 How to Use

1. **Enter Student Information**
   - Add student name (optional)
   - Set target completion date

2. **Add Courses**
   - Click "Add Course" (up to 8 courses)
   - Enter course name
   - Fill in completed and total activities for each type

3. **View Results**
   - Get personalized daily targets
   - Track progress across all courses
   - See detailed breakdowns by activity type

## 🎨 Customization

### Modify School Holidays
Edit the `getSchoolHolidays()` function in the JavaScript section to add or remove specific holiday dates.

### Change Activity Types
Modify the `activityTypes` array to customize the types of activities tracked:
```javascript
const activityTypes = ['Quiz', 'Test', 'Exam', 'Essay/Assignment', 'Lab/Project'];
```

### Adjust Maximum Courses
Change the `maxCourses` variable to allow more or fewer courses:
```javascript
const maxCourses = 8; // Change this number
```

## 🧮 Calculation Logic

- **Workdays Only:** Only counts Monday through Friday
- **Holiday Exclusions:** Automatically excludes all programmed school holidays
- **Daily Targets:** Calculates `ceil(remaining_activities / available_workdays)`
- **Progress Tracking:** Shows completion percentage for each course and overall

## 📱 Responsive Design

The calculator is fully responsive and works on:
- Desktop computers
- Tablets
- Mobile phones

## 🔧 Technical Details

- **Built with:** HTML, CSS (Tailwind), and Vanilla JavaScript
- **No dependencies:** Runs entirely in the browser
- **No backend required:** Perfect for GitHub Pages hosting
- **Local storage:** Not used (calculations are session-based)

## 🤝 Contributing

Feel free to fork this repository and submit pull requests for improvements:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📄 License

This project is open source and available under the MIT License.

## 🆘 Support

If you encounter any issues:

1. Check that your target completion date is in the future
2. Ensure at least one course has activity totals entered
3. Verify your GitHub Pages is properly configured

---

*Built for students to better manage their Edgenuity coursework and stay on track with their academic goals.*
