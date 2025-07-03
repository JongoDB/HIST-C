# Contributing to HIST-C 🍯

First off, thanks for taking the time to contribute! ❤️

The following is a set of guidelines for contributing to HIST-C. These are mostly guidelines, not rules. Use your best judgment, and feel free to propose changes to this document in a pull request.

## 🚀 How Can I Contribute?

### 🐛 Reporting Bugs

Before creating bug reports, please check the issue list as you might find out that you don't need to create one. When you are creating a bug report, please include as many details as possible:

**Before Submitting A Bug Report:**
- Check the debugging guide
- Check the FAQs for common questions and problems
- Perform a cursory search to see if the issue has already been reported

**How Do I Submit A Bug Report?**
Bugs are tracked as GitHub issues. Create an issue and provide the following information:

- **Use a clear and descriptive title**
- **Describe the exact steps to reproduce the problem**
- **Provide specific examples** to demonstrate the steps
- **Describe the behavior you observed** and **explain which behavior you expected to see**
- **Include screenshots and animated GIFs** if they help explain the problem
- **Include details about your browser and operating system**

### 🌟 Suggesting Enhancements

Enhancement suggestions are tracked as GitHub issues. When creating an enhancement suggestion, please include:

- **Use a clear and descriptive title**
- **Provide a step-by-step description of the suggested enhancement**
- **Provide specific examples** to demonstrate the steps
- **Describe the current behavior** and **explain which behavior you expected to see**
- **Explain why this enhancement would be useful**

### 💻 Code Contributions

#### Local Development

HIST-C is a client-side application, so development is straightforward:

1. Fork the repo
2. Clone your fork locally
3. Open `index.html` in your browser
4. Make your changes
5. Test thoroughly
6. Submit a pull request

#### Pull Request Process

1. **Fork** the repository
2. **Create** a feature branch from `main`
3. **Make** your changes
4. **Test** your changes across different browsers
5. **Commit** your changes with descriptive commit messages
6. **Push** to your feature branch
7. **Submit** a pull request

### 🎯 What Should I Know Before I Get Started?

#### Code Structure

HIST-C is a single-file HTML application with embedded CSS and JavaScript:

```
index.html
├── HTML Structure
├── CSS Styles (embedded)
└── JavaScript Logic (embedded)
```

#### Key Components

- **File Upload Handler**: Manages drag-and-drop and file selection
- **File Processing Engine**: Handles compression and filtering
- **Output Generator**: Creates the final compressed format
- **UI Controller**: Manages user interactions and state

## 🎨 Style Guidelines

### JavaScript Style Guide

- Use camelCase for variable and function names
- Use meaningful variable names
- Add comments for complex logic
- Use modern ES6+ features where appropriate
- Keep functions focused and single-purpose

### CSS Style Guide

- Use meaningful class names
- Follow BEM methodology where applicable
- Use CSS custom properties for theming
- Ensure responsive design principles

### HTML Style Guide

- Use semantic HTML elements
- Ensure accessibility with proper ARIA labels
- Maintain proper indentation
- Use meaningful IDs and classes

## 🧪 Testing Guidelines

### Manual Testing Checklist

Before submitting a PR, please test:

- [ ] File upload (drag & drop and click)
- [ ] Different file types and extensions
- [ ] Large projects (100+ files)
- [ ] All compression options
- [ ] Download functionality
- [ ] Copy to clipboard
- [ ] Responsive design on different screen sizes
- [ ] Cross-browser compatibility (Chrome, Firefox, Safari, Edge)

### Test Cases to Consider

1. **Empty Projects**: Projects with no files
2. **Large Projects**: 500+ files, 10MB+ size
3. **Mixed Languages**: Projects with multiple programming languages
4. **Special Characters**: Files with unicode, spaces, special characters
5. **Edge Cases**: Very long file names, deeply nested folders

## 📝 Commit Message Guidelines

Use clear and meaningful commit messages:

```
feat: add support for Rust language syntax highlighting
fix: resolve issue with large file processing
docs: update README with new compression statistics
style: improve responsive design for mobile devices
refactor: optimize file filtering algorithm
test: add test cases for edge scenarios
```

## 🏷️ Issue and PR Labels

We use several labels to help organize issues and PRs:

### Type Labels
- `bug` - Something isn't working
- `enhancement` - New feature or request
- `documentation` - Improvements or additions to documentation
- `question` - Further information is requested

### Priority Labels
- `priority: high` - Critical issues that need immediate attention
- `priority: medium` - Important issues that should be addressed soon
- `priority: low` - Nice-to-have improvements

### Status Labels
- `help wanted` - Extra attention is needed
- `good first issue` - Good for newcomers
- `wontfix` - This will not be worked on

## 🌍 Language Support

Adding support for new programming languages involves:

1. **Comment Removal**: Add regex patterns for single-line and multi-line comments
2. **Debug Statement Removal**: Add patterns for common debug statements
3. **Minification Rules**: Add language-specific minification logic
4. **Testing**: Test with real-world projects in that language

Example for adding new language support:

```javascript
// In the removeComments function
if (['newlang', 'nl'].includes(ext)) {
    return content
        .replace(/--.*$/gm, '') // Single line comments
        .replace(/\/\*[\s\S]*?\*\//g, ''); // Block comments
}
```

## 🔍 Code Review Process

All submissions require review. We use GitHub pull requests for this purpose. Reviewers will look for:

- **Functionality**: Does the code work as intended?
- **Style**: Does the code follow our style guidelines?
- **Performance**: Is the code efficient?
- **Compatibility**: Does it work across different browsers?
- **Testing**: Has the change been properly tested?

## 🤝 Community Guidelines

### Be Respectful
- Use welcoming and inclusive language
- Be respectful of differing viewpoints and experiences
- Gracefully accept constructive criticism
- Focus on what is best for the community

### Be Collaborative
- Help others learn and grow
- Share knowledge and best practices
- Ask questions when you need help
- Offer help to others when you can

## 📞 Getting Help

If you need help contributing:

1. Check the README.md for basic information
2. Look through existing issues and PRs
3. Join our discussions on GitHub
4. Reach out to maintainers

## 🙏 Recognition

Contributors will be recognized in:
- README.md contributors section
- Release notes for significant contributions
- GitHub contributors page

Thank you for contributing to HIST-C! 🍯✨