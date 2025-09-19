# Edgenuity - Activities to Completion Calculator
A web-based calculator designed to help LFLCS teachers plan and track their students' Edgenuity coursework across multiple classes. The calculator automatically accounts for weekends and school holidays to provide realistic daily activity targets.

## 🚀 Live Demo

Visit the calculator at: `https://juliebkhou.github.io/ActivitiesToCompletionCalculator/`

## ✨ Features

### Activity Tracking per Course
  - Quizzes (completed/total)
  - Tests (completed/total)
  - Exams (completed/total)
  - Essays/Assignments (completed/total)
  - Labs/Projects (completed/total)

### Course Calculations & Detaied Progress Reports
- Support for up to 15 courses
- Automatic calculation of totals and remaining activities
- Daily activity targets for each course and overall
- Visual progress bars to track each course and overall courses

### Save the Results as a PDF
- Button below the results to save the summaries
- First page contains the overall summary and summaries of up to 5 courses
- 6+ courses will spill onto the other pages

## 🎯 How to Use

1. **Enter Student Information**
   - Add student name (optional)
   - Set target completion date

2. **Add Courses**
   - Click "Add Course"
   - Enter course name
   - Fill in completed and total activities for each type

3. **View Results**
   - Get personalized daily targets
   - Track progress across all courses
   - See detailed breakdowns

4. **Save Results**
   - Save the overall summary
   - Save individual course summaries

## 🧮 Calculation Logic

- **Weekdays Only:** Calculations exclude weekends
- **Holiday Exclusions:** Automatically excludes all programmed school holidays and major US holidays
  - October 6-10 (Fall Break)
  - November 24-28 (Thanksgiving Week)
  - December 22 - January 6 (Winter Break)
  - March 23 - April 3 (Spring Break)
  - All major US holidays
- **Daily Targets:** Calculates `ceil(remaining_activities / available_workdays)`
- **Progress Tracking:** Shows completion percentage for each course and overall

## 🔧 Technical/ Customization Details

- **Cross-Platform:** Can work on computers, tablets, or phones
- **Built with:** HTML, CSS (Tailwind), and JavaScript
- **No dependencies:** Runs entirely in the browser
- **Local storage:** Not used (calculations are session-based)
- **Modify School Holidays:** Edit the `getSchoolHolidays()` function in the JavaScript section to add or remove specific holiday dates
- **Change Activity Types:** Modify the `activityTypes` array to customize the types of activities tracked:
```javascript
const activityTypes = ['Quiz', 'Test', 'Exam', 'Essay/Assignment', 'Lab/Project'];
```
- **Adjust Maximum Courses:** Change the `maxCourses` variable to allow more or fewer courses:
```javascript
const maxCourses = 15; // Change this number
```

## 🆘 Support

If you encounter any issues:

1. Check that your target completion date is in the future
2. Make sure at least one course has activity totals entered
3. Refresh the page (note: this deletes all the numbers entered)

---

*Developed by Julie Khou in collaboration with AI*
