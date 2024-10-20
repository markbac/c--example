# Windows To-Do App
A simple Windows To-Do application built using Windows Forms in C#.

## Features
- Add, edit, and delete tasks.
- "New", "Open", "Save", and "Exit" options in the File menu.
- Task persistence via local file storage.

## Project Structure

The project structure is as follows:

```
/WindowsTodoApp
├── .github/              # GitHub Actions workflows
├── docs/                 # Documentation files
├── src/                  # Main application source files
│   ├── MainForm.cs       # The main form (UI) code-behind
│   ├── MainForm.Designer.cs # The form designer code
├── LICENSE               # License file
├── README.md             # Project readme file
```

## GitHub Actions Workflow

This project includes a GitHub Actions workflow that builds and releases the application when a tag with the pattern `v*.*.*` is pushed to the repository. The workflow does the following:
- Restores dependencies
- Builds the application
- Publishes the application as a release artifact on GitHub

### How to trigger the build:
1. Create a tag that follows the pattern `v*.*.*` (e.g., `v1.0.0`) and push it to GitHub.
   ```
   git tag v1.0.0
   git push origin v1.0.0
   ```

2. The GitHub Action will automatically build and release the application.

## Installation
To run the app:
1. Open the solution in Visual Studio.
2. Build the project.
3. Run the executable created in the `bin` folder.

## Usage
- Open the app and create a new task list.
- Add tasks to the list using the 'Add' button.
- Save your task list to a `.txt` file for future use.

## Contributing
Feel free to submit pull requests for additional features or bug fixes.

## License
MIT License. See LICENSE file for details.
