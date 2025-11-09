# Algorithm Learning Repository Guidelines

## Project Structure & Module Organization
- `golang/`: Go language algorithm implementations, organized by algorithm types in subdirectories
- `python/`: Python algorithm implementations, organized by algorithm types in subdirectories
- `templates/`: Algorithm implementation templates, users complete code based on templates
- `solutions/`: Reference solutions and best practices
- `docs/`: Learning documentation and algorithm analysis
- Each language directory organized by algorithm categories: sorting, searching, graph theory, dynamic programming, etc. If the category doesn't have a directory, you need to create a new one

## Build, Test, and Development Commands
- **Go**: `cd golang && go run .` or `go build` to compile and run
- **Python**: `cd python && python main.py` or `python3 main.py` to run
- **Testing**: Run corresponding language test commands in each algorithm directory
- **Formatting**: Go uses `gofmt`, Python uses `black` or `autopep8`

## Coding Style & Naming Conventions
- **Go**: Use `gofmt` for formatting; functions and variables use camelCase; package names use lowercase
- **Python**: Follow PEP 8 standards; use snake_case naming; classes use CamelCase
- **General**: Variable names should be meaningful, avoid single-letter variables; add necessary comments


## Testing Guidelines
- **Go**: Use built-in testing package, test files end with `_test.go`
- **Python**: Use unittest or pytest framework, test files start with `test_`
- Each algorithm implementation should include corresponding test cases
- Tests should cover common edge cases and abnormal inputs

## Learning Path and Evaluation System
- **Learning Path**: Basic Algorithms → Data Structures → Advanced Algorithms → Comprehensive Applications
- **Template Mechanism**: Provide framework code for each algorithm, users fill in core logic
- **Evaluation Criteria**: Correctness, Efficiency, Readability, Test Coverage
- **Progress Tracking**: Provide personalized guidance based on user's chosen learning direction

## Algorithm Implementation Process
1. User selects algorithm type and specific problem
2. Provide algorithm template and requirements
3. User implements core algorithm logic
4. Run tests to verify correctness
5. Provide detailed code evaluation and optimization suggestions
6. Adjust learning path based on evaluation results

## Code Quality Standards
- **Correctness**: Algorithm logic is correct, handles edge cases
- **Efficiency**: Reasonable time and space complexity
- **Readability**: Code is clear with appropriate comments
- **Testing**: Includes complete test cases covering edge cases
- **Best Practices**: Follow language conventions, use appropriate data structures

## Output Language
- The user's native language is `Chinese`, you need to output according to local language habits
