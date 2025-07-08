# Star Rating Component - Machine Coding Exercise

A simple, interactive star rating component built with vanilla HTML, CSS, and JavaScript. This project demonstrates fundamental web development concepts including DOM manipulation, event handling, and responsive design.

## 🌟 Features

- **Interactive Rating**: Click on stars to set a rating (1-5 stars)
- **Visual Feedback**: Stars fill with gold color when hovered or selected
- **Real-time Display**: Shows the current rating number in the header
- **Hover Effects**: Stars preview rating on hover with smooth transitions
- **Persistent Selection**: Rating persists after mouse leaves the component
- **Responsive Design**: Clean, centered layout that works on different screen sizes

## 🚀 Demo

The star rating component includes:
- 5 clickable star icons
- Hover effects with star size animation
- Real-time rating display
- Smooth color transitions (gray to gold)

## 📁 Project Structure

```
machineCoding1/
├── example1.html          # Main HTML file with complete implementation
└── README.md             # Project documentation
```

## 🛠️ Technologies Used

- **HTML5**: Semantic markup and structure
- **CSS3**: Styling, flexbox layout, and hover effects
- **JavaScript (ES6+)**: DOM manipulation and event handling
- **Font Awesome**: Star icons (CDN)

## 💻 How to Run

1. Clone or download this repository
2. Open `example1.html` in any modern web browser
3. No additional setup or dependencies required!

```bash
# If you have a local server (optional)
# Navigate to project directory and run:
python -m http.server 8000
# Then visit: http://localhost:8000/example1.html
```

## 🔧 Implementation Details

### Key JavaScript Concepts Demonstrated

1. **Event Delegation**: Single event listener on parent container
2. **DOM Manipulation**: Dynamic class management for visual states
3. **Event Types**: 
   - `click` - For rating selection
   - `mouseover` - For hover preview
   - `mouseleave` - For reverting to selected state

### CSS Techniques Used

1. **Flexbox Layout**: Centering and star arrangement
2. **CSS Transitions**: Smooth hover animations
3. **Font Icon Integration**: Font Awesome stars
4. **Hover Effects**: Size and color changes

### Core Functionality

```javascript
// Star selection logic
function handleStarSelection(currentIdx) {
    starsRef.forEach((star, idx) => {
        if(idx < currentIdx) {
            selectStar(star.querySelector('i'));
        } else {
            deSelectStar(star.querySelector('i'));
        }
    })
}
```

## 🎯 Learning Objectives

This exercise covers:

- **DOM Traversal**: Query selectors and element manipulation
- **Event Handling**: Multiple event types and event delegation
- **State Management**: Tracking selected vs. hovered states
- **CSS Animations**: Hover effects and transitions
- **User Experience**: Intuitive interaction patterns

## 🔄 Possible Enhancements

- [ ] Add half-star ratings (0.5, 1.5, 2.5, etc.)
- [ ] Include rating labels ("Poor", "Good", "Excellent")
- [ ] Add local storage to persist ratings
- [ ] Create multiple rating components on one page
- [ ] Add keyboard navigation support
- [ ] Implement custom star colors/themes
- [ ] Add rating submission and display features

## 🐛 Known Issues

- Rating resets when page is refreshed (no persistence)
- Only supports integer ratings (1-5)

## 📚 Concepts Practiced

### JavaScript
- Event listeners and event delegation
- DOM element selection and manipulation
- CSS class management
- Data attributes usage
- Function organization and reusability

### CSS
- Flexbox layout system
- Pseudo-classes (`:hover`)
- Font icon integration
- Responsive design principles
- Animation and transitions

### HTML
- Semantic structure
- Data attributes
- External CDN integration
- Accessibility considerations

## 🎨 Styling Details

- **Colors**: Gold (#gold) for selected stars, gray (#817f7f) for unselected
- **Layout**: Centered container using flexbox
- **Animations**: Size increase on hover (24px → 28px)
- **Spacing**: 5px gap between stars

## 🔗 External Dependencies

- [Font Awesome 6.7.2](https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.2/css/all.min.css) - For star icons

## 📝 Code Quality

- Clean, readable code structure
- Consistent naming conventions
- Separation of concerns (HTML/CSS/JS)
- Event-driven architecture
- Reusable functions

---

**Note**: This is a machine coding exercise focused on demonstrating core web development skills without external frameworks or libraries (except Font Awesome for icons).

## 👨‍💻 Author

Created as part of machine coding practice exercises.

---

*Happy Coding! 🚀*