# TimeTrackerEx

A simple Visual Studio Code extension for tracking time spent on tasks and generating templates for status reporting.

## Features

### Time Tracking

TimeTrackerEx offers a straightforward way to track the time you spend on specific tasks:

- Start a timer with a single command
- End the timer with the same command to see how much time has elapsed
- Time markers are added directly to your document at the cursor position
- Duration is calculated and displayed automatically


### SR Template Generation

Quickly insert standardized status report templates with:

- Auto-populated date in YYYYMMDD format
- Username customization via settings
- Consistent format for status tracking



### Time Tracking

1. Position your cursor at the end of a task description
2. Run the command `TimeTrackerEx: Track Time` (via Command Palette or keyboard shortcut)
3. The start time marker will be added to your document
4. When you've completed the task, run the command again
5. The end time and duration will be added to your document

### Template Generation

1. Position your cursor where you want to insert the template
2. Run the command `TimeTrackerEx: Insert Template` (via Command Palette)
3. A template with the following structure will be inserted:

```
SRyyyymmddUserName:
  Was:
    -
  Next:
    -
  AIOB:
```

## Configuration

### User Name

Configure your username for template generation in VS Code settings:

1. Open Settings (File > Preferences > Settings)
2. Search for "TimeTrackerEx"
3. Set your username in the "timetrackerex.userName" field

## Commands

This extension provides the following commands:

- `timetrackerex.timeTracker`: Track time for a task
- `timetrackerex.insertTemplate`: Insert a status report template

### 0.0.1

- Initial release
- Time tracking functionality
- Template generation with date and username support