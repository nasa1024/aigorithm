# Algorithm Learning Repository Usage Guide

## Project Structure
- `golang/`: Go language algorithm implementations, organized by algorithm types in subdirectories
- `python/`: Python language algorithm implementations, organized by algorithm types in subdirectories
- `templates/`: Algorithm implementation templates, users complete code based on templates
- `solutions/`: Reference solutions and best practices
- `docs/`: Learning documentation and algorithm analysis
- Each language directory organized by algorithm categories: sorting, searching, graph theory, dynamic programming, etc.

## Usage Method
**One Problem at a Time**: Users select and complete one algorithm problem at a time, then notify the assistant for evaluation

## Build and Test Commands
- **Go**: `cd golang && go run .` or `go build`
- **Python**: `cd python && python main.py` or `python3 main.py`
- **Testing**: Run corresponding language test commands in each algorithm directory
- **Formatting**: Go uses `gofmt`, Python uses `black` or `autopep8`

## Coding Standards
- **Go**: Use `gofmt` for formatting; functions and variables use camelCase; package names use lowercase
- **Python**: Follow PEP 8 standards; use snake_case naming; classes use CamelCase
- **General**: Variable names should be meaningful, avoid single-letter variables; add necessary comments

## Testing Standards
- **Go**: Use built-in testing package, test files end with `_test.go`
- **Python**: Use unittest or pytest framework, test files start with `test_`
- Each algorithm implementation should include corresponding test cases
- Tests should cover common edge cases and abnormal inputs

## Learning Path (From Simple to Difficult)
1. **Basic Algorithms**: Sorting, searching, mathematical calculations
2. **Data Structures**: Arrays, linked lists, stacks, queues, hash tables
3. **Intermediate Algorithms**: Recursion, divide and conquer, greedy algorithms
4. **Advanced Algorithms**: Dynamic programming, graph theory, tree structures
5. **Comprehensive Applications**: Complex problem solving

## Problem Difficulty Levels
- **Easy**: Basic concepts and implementation
- **Medium**: Requires certain algorithmic thinking
- **Hard**: Complex algorithm design and optimization

## Learning Process
1. User selects algorithm type and specific problem (one at a time)
2. Provide algorithm template and requirements
3. User implements core algorithm logic
4. User notifies assistant after completing code
5. Assistant generates detailed `doc.md` evaluation document
6. Provide optimization suggestions based on evaluation results

## Evaluation Criteria
- **Correctness**: Algorithm logic is correct, handles edge cases
- **Efficiency**: Reasonable time and space complexity
- **Readability**: Code is clear with appropriate comments
- **Testing**: Includes complete test cases covering edge cases
- **Best Practices**: Follow language conventions, use appropriate data structures

## Output Language
- User's native language is Chinese, output should follow Chinese language habits