# 🍅 BSCS Pomodoro Timer

A sleek, terminal-inspired **Pomodoro focus timer** with dark/light theme support, perfect for students grinding through Computer Science coursework.

![Timer Screenshot](https://img.shields.io/badge/Status-Active-green?style=flat-square)
![HTML/CSS/JS](https://img.shields.io/badge/Built%20With-HTML%2FCSS%2FJS-blue?style=flat-square)

## Features

✨ **Core Functionality**
- **Focus Mode**: 25-minute focused work sessions
- **Short Break**: 5-minute breaks between sessions
- **Long Break**: 15-minute breaks after 4 sessions
- **Custom Timer**: Set any duration from 1-90 minutes
- **Progress Bar**: Visual feedback with real-time progress tracking

🎨 **UI/UX**
- **Dark/Light Theme Toggle**: Eye-friendly dark mode (default) and light mode
- **Terminal Aesthetic**: Styled like a VS Code/terminal window with macOS window controls
- **Responsive Design**: Works on desktop and mobile devices
- **Real-time Updates**: Time display with MM:SS formatting

📊 **Tracking & Statistics**
- Session counter (completed focus sessions)
- Total focused time (in minutes)
- Breaks taken counter
- Live session information display

✅ **Task Management**
- Add daily CS tasks/assignments to your todo list
- Check off completed tasks
- Delete tasks with one click
- Persistent task UI within the session

## How to Use

1. **Clone the Repository**
   ```bash
   git clone https://github.com/KhielDecena/pomoduratimer.git
   cd pomoduratimer
   ```

2. **Open in Browser**
   - Simply open `index.html` in your web browser
   - No build process or dependencies required

3. **Start Focusing**
   - Click the **start()** button to begin a focus session
   - Select different modes (focus, break, long_break, custom)
   - Use **pause()** to pause and resume
   - Click **reset()** to restart the current session
   - Click **skip()** to jump to the next phase

4. **Add Tasks**
   - Type a task in the "tasks[] — today's CS grind" input field
   - Click **+ push()** or press Enter to add it
   - Check off tasks as you complete them
   - Delete tasks with the × button

## Theme Toggle

Click the theme button (☀️/🌙) in the top-right corner to switch between:
- **Dark Mode**: OLED-friendly dark theme (default)
- **Light Mode**: GitHub-inspired light theme

## File Structure

```
pomoduratimer/
├── index.html      # Main application file (HTML + CSS + JavaScript)
├── README.md       # Documentation (this file)
└── ...
```

## Technical Details

**Built With:**
- HTML5 for structure
- CSS3 for styling with CSS custom properties (variables)
- Vanilla JavaScript (no frameworks)

**Dependencies:**
- [Tabler Icons](https://tabler-icons.io/) - For UI icons
- [JetBrains Mono Font](https://fonts.google.com/specimen/JetBrains+Mono) - Terminal-style font

**Color Schemes:**
- Dark Theme: GitHub Dark color palette
- Light Theme: GitHub Light color palette

## Timer Logic

The Pomodoro technique breaks work into intervals:

```
Focus (25 min) → Break (5 min) → Focus (25 min) → ... → Long Break (15 min)
     ↓              ↓              ↓                      ↓
  Session 1    Break 1        Session 2         After 4 Sessions
```

### State Management
- **Idle**: Timer hasn't started yet
- **Running**: Timer is actively counting down
- **Paused**: Timer was running but is now paused
- **Break**: Currently in a break period

## Browser Support

Works on all modern browsers supporting:
- ES6 JavaScript
- CSS Grid & Flexbox
- CSS Custom Properties

## Customization

You can customize the default durations by editing the `MODES` object in `index.html`:

```javascript
const MODES={focus:25,short:5,long:15,custom:30};
```

- `focus`: Focus session duration (minutes)
- `short`: Short break duration (minutes)
- `long`: Long break duration (minutes)
- `custom`: Default custom timer value (minutes)

## Tips for Productivity

1. **Silence notifications** during focus sessions
2. **Put your phone away** to eliminate distractions
3. **Use the task list** to stay organized
4. **Track your sessions** to build consistent habits
5. **Take real breaks** — move around, hydrate, stretch

## Future Enhancements

Potential features for future versions:
- [ ] Sound notifications on timer completion
- [ ] Data persistence (localStorage for stats and tasks)
- [ ] Keyboard shortcuts (spacebar to start/pause, etc.)
- [ ] Session history and weekly stats
- [ ] Customizable session cycles

## License

This project is open source. Feel free to fork, modify, and use it!

## Support

For issues, suggestions, or contributions, please open an issue on [GitHub Issues](https://github.com/KhielDecena/pomoduratimer/issues).

---

**Stay focused. Stay productive. 🧑‍💻**

Built with ❤️ for BSCS students everywhere.
