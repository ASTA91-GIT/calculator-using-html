# Web Calculator

A modern, responsive web-based calculator built with HTML, CSS, and JavaScript. This project demonstrates frontend web development skills including DOM manipulation, event handling, responsive design, and modern CSS techniques.

## 🧮 Calculator Overview

The Web Calculator provides a sleek, modern interface for performing basic arithmetic operations. It features a responsive design that works seamlessly on desktop, tablet, and mobile devices, with full keyboard support and smooth animations.

## ✨ Features

- **Modern Design**: Clean, professional interface with gradient backgrounds
- **Responsive Layout**: Works perfectly on all device sizes
- **Keyboard Support**: Full keyboard functionality for all operations
- **Visual Feedback**: Hover effects, animations, and smooth transitions
- **Error Handling**: Division by zero protection and input validation
- **Cross-Browser**: Compatible with all modern web browsers
- **Touch-Friendly**: Optimized for touch devices and mobile use
- **Real-time Display**: Live calculation display with proper formatting

## 🛠️ Technologies Used

- **HTML5**: Semantic markup and structure
- **CSS3**: Modern styling with Flexbox, Grid, and animations
- **JavaScript**: Interactive functionality and DOM manipulation
- **Font Awesome**: Icons for enhanced visual appeal
- **Responsive Design**: Mobile-first approach
- **Modern CSS**: Gradients, shadows, and transitions

## 🚀 How to Run

### Prerequisites
- Any modern web browser (Chrome, Firefox, Safari, Edge)
- No additional software installation required

### Running the Calculator

#### Method 1: Direct File Opening
1. **Navigate to the project directory**:
   ```
   PROJECTS/FRONT_END/projects/
   ```

2. **Open the file**:
   - Double-click `web_calculator.html`
   - Or drag and drop the file into your browser

#### Method 2: Local Server (Recommended)
1. **Using Python**:
   ```bash
   cd PROJECTS/FRONT_END/projects
   python -m http.server 8000
   ```
   Then open: `http://localhost:8000/web_calculator.html`

2. **Using Node.js**:
   ```bash
   cd PROJECTS/FRONT_END/projects
   npx serve .
   ```

3. **Using Live Server (VS Code Extension)**:
   - Right-click on `web_calculator.html`
   - Select "Open with Live Server"

## 🎯 How to Use

### Mouse/Touch Interface
1. **Click the calculator buttons** to input numbers and operations
2. **Use the 'C' button** to clear the display
3. **Use the '⌫' button** to delete the last character
4. **Press '=' or Enter** to calculate the result

### Keyboard Support
- **Numbers**: 0-9 keys
- **Operators**: +, -, *, / keys
- **Decimal**: . (period) key
- **Calculate**: Enter or = key
- **Clear**: Escape key
- **Delete**: Backspace key

## 📋 Code Structure

### HTML Structure
```html
<div class="calculator">
    <div class="title">Calculator</div>
    <div class="display" id="display">0</div>
    <div class="buttons">
        <!-- Calculator buttons -->
    </div>
</div>
```

### CSS Features
- **Grid Layout**: Responsive button grid
- **Flexbox**: Centered layout and alignment
- **CSS Variables**: Consistent color scheme
- **Media Queries**: Mobile responsiveness
- **Animations**: Smooth transitions and hover effects

### JavaScript Functions

#### Core Functions
- `updateDisplay()`: Updates the calculator display
- `appendToDisplay(value)`: Adds characters to display
- `clearDisplay()`: Resets calculator to initial state
- `deleteLast()`: Removes the last character
- `calculate()`: Performs the mathematical operation
- `handleOperator(op)`: Manages operator logic

#### Event Handling
- **Click Events**: Button interactions
- **Keyboard Events**: Full keyboard support
- **DOM Manipulation**: Dynamic display updates

## 🎨 Design Features

### Visual Design
- **Gradient Background**: Modern purple-blue gradient
- **Card Design**: Elevated calculator with shadows
- **Color-Coded Buttons**: Different colors for different button types
- **Smooth Animations**: Hover effects and transitions
- **Typography**: Clean, readable fonts

### Responsive Design
- **Mobile-First**: Optimized for small screens
- **Flexible Grid**: Adapts to different screen sizes
- **Touch Targets**: Adequate button sizes for touch devices
- **Viewport Meta**: Proper mobile scaling

## 🔧 Customization Options

### Easy Modifications

#### Change Color Scheme
```css
/* Modify CSS variables in the <style> section */
:root {
    --primary-color: #3498db;    /* Change main button color */
    --operator-color: #e74c3c;   /* Change operator button color */
    --equals-color: #27ae60;     /* Change equals button color */
    --clear-color: #f39c12;      /* Change clear button color */
}
```

#### Add New Operations
```javascript
// Add to the calculate() function
switch (operation) {
    case '+':
        result = previous + current;
        break;
    case '-':
        result = previous - current;
        break;
    case '*':
        result = previous * current;
        break;
    case '/':
        result = previous / current;
        break;
    case '^':  // Add power operation
        result = Math.pow(previous, current);
        break;
    case '√':  // Add square root
        result = Math.sqrt(previous);
        break;
}
```

#### Modify Display Format
```javascript
// Change number formatting in updateDisplay()
function updateDisplay() {
    // Format with commas for thousands
    const formatted = parseFloat(displayValue).toLocaleString();
    display.textContent = formatted;
}
```

## 🧪 Testing the Calculator

### Test Cases to Try

#### Basic Operations
1. **Addition**: 5 + 3 = 8
2. **Subtraction**: 10 - 4 = 6
3. **Multiplication**: 6 × 7 = 42
4. **Division**: 15 ÷ 3 = 5

#### Advanced Operations
1. **Chaining**: 5 + 3 × 2 (should follow order of operations)
2. **Decimals**: 3.14 + 2.86
3. **Large Numbers**: 999999 + 1
4. **Negative Results**: 5 - 10

#### Edge Cases
1. **Division by Zero**: 10 ÷ 0 (should show error)
2. **Multiple Decimals**: 3.14.15 (should prevent)
3. **Leading Zeros**: 00123 (should handle properly)
4. **Keyboard Input**: Test all keyboard shortcuts

#### Responsive Testing
1. **Desktop**: Full functionality
2. **Tablet**: Touch interactions
3. **Mobile**: Small screen layout
4. **Landscape/Portrait**: Orientation changes

### Sample Usage Session
```
1. Click '5' → Display shows: 5
2. Click '+' → Display shows: 5
3. Click '3' → Display shows: 3
4. Click '=' → Display shows: 8
5. Click '×' → Display shows: 8
6. Click '2' → Display shows: 2
7. Click '=' → Display shows: 16
8. Click 'C' → Display shows: 0
```

## 📚 Learning Objectives

This project helps you learn:
- **HTML5**: Semantic markup and structure
- **CSS3**: Modern styling techniques and responsive design
- **JavaScript**: DOM manipulation and event handling
- **Responsive Design**: Mobile-first development approach
- **User Experience**: Creating intuitive interfaces
- **Cross-Browser Compatibility**: Ensuring functionality across browsers
- **Modern Web Development**: Best practices and techniques

## 🔗 Related Links

- **Live Demo**: [Web Calculator](projects/web_calculator.html)
- **GitHub Repository**: [View Code](https://github.com/ASTA91-GIT/portfolio/blob/main/projects/web_calculator.html)
- **All Projects**: [Portfolio Projects](https://github.com/ASTA91-GIT/portfolio/tree/main/projects)
- **Main Portfolio**: [ASTA Portfolio](https://asta91-git.github.io/portfolio)

## 🤝 Contributing

Feel free to:
- Add scientific calculator functions
- Implement memory features (M+, M-, MR, MC)
- Add unit conversion capabilities
- Create different calculator themes
- Add calculation history
- Implement keyboard shortcuts
- Add sound effects for button clicks

## 📄 License

This project is part of the ASTA Portfolio and is available under the MIT License.

---

**Happy Calculating! 🧮**

*This project showcases modern web development skills while providing a practical and beautiful calculator application.*
