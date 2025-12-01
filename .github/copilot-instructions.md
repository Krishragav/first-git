# Copilot Instructions for first-git

## Project Overview

This is a simple learning repository for Git workflows featuring a basic Python calculator. The project demonstrates branching and feature development patterns.

**Current structure:**
- Main branch (main): Basic calculator with addition and subtraction operations
- Feature branch (feature/Multiplication): Extends calculator with multiplication operation
- Single Python file: `Calculator.py` - contains basic arithmetic operations

## Architecture & Components

**Calculator.py** - The main application module
- Simple print-based calculator demonstrating arithmetic operations
- Operations are executed immediately upon script execution
- Currently supports: Addition, Subtraction, Multiplication
- Pattern: Direct print statements for operation output
- Example: `print("Operation:", expression)`

## Development Workflow

### Git Workflow Pattern
This repository follows a **feature branch workflow**:
1. **main** branch: Stable, contains base functionality
2. **feature/** branches: Feature development branches for new operations
3. Current work: `feature/Multiplication` - adds multiplication support

### Commit Pattern
- Commits are versioned (e.g., "version1", "version2")
- Each commit typically adds a new operation to Calculator.py
- Commits track incremental feature additions

### Adding New Features
To add a new operation (e.g., division):
1. Branch from main: `git checkout -b feature/Division`
2. Add new print statement to Calculator.py
3. Commit with version increment: `git commit -m "version3"`
4. Maintain consistent formatting: `print("OperationName:", expression)`

## Key Patterns & Conventions

### Code Style (Calculator.py)
- Simple sequential operations without functions
- Each operation is a print statement on its own line
- Consistent format: `print("OperationName:", arithmetic_expression)`
- No error handling or input validation currently
- Direct inline calculations (no intermediate variables)

### Feature Addition Pattern
When extending functionality:
1. Add new print statement following existing format
2. Maintain alphabetical or logical operation order
3. Include descriptive operation name in output
4. Keep expressions simple and inline

## Testing & Execution

**Running the calculator:**
```powershell
python Calculator.py
```

**Expected output:**
```
Addition: 4
Subtraction: 2
Multiplication: 15
```

## Integration Points & Dependencies

- **Python version**: No specific version requirements observed
- **External dependencies**: None
- **Cross-component communication**: Single-file design, no inter-module dependencies
- **Git repository**: Remote tracking to origin (main and feature/Multiplication branches)

## Common Tasks for AI Agents

- **Adding operations**: Follow the print statement pattern; maintain consistent formatting
- **Commit messages**: Use version numbering approach (version1, version2, etc.)
- **Branch naming**: Use `feature/<OperationName>` convention for new operations
- **Testing changes**: Run `python Calculator.py` and verify output

## Notes for Future Work

- Consider refactoring to use functions if more operations are added
- Consider implementing division, modulo, or power operations following the feature branch pattern
- This is a learning repository; maintain simplicity for educational purposes
