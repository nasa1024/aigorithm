# Algorithm Learning Repository Usage Guide

## Project Structure
- `golang/`: Go language algorithm implementations, organized by algorithm types in subdirectories
- `python/`: Python language algorithm implementations, organized by algorithm types in subdirectories
- `javascript/` or `typescript/`: JS/TS algorithm implementations by categories
- `java/`: Java algorithm implementations by categories
- `cpp/`: C++ algorithm implementations by categories
- `rust/`: Rust algorithm implementations by categories
- `csharp/`: C# (.NET) algorithm implementations by categories
- `templates/`: Algorithm implementation templates, users complete code based on templates
- `solutions/`: Reference solutions and best practices
- `docs/`: Learning documentation and algorithm analysis
- Each language directory organized by algorithm categories: sorting, searching, graph theory, dynamic programming, etc.

## Usage Method
**One Problem at a Time**: Users select and complete one algorithm problem at a time, then notify the assistant for evaluation

## Build and Test Commands
- **Go**: `cd golang && go run .` or `go build`
- **Python**: `cd python && python main.py` or `python3 main.py`
- **JavaScript/TypeScript**: `cd javascript && npm test` (or `node main.js`); TS via `ts-node` or build with `tsc`
- **Java**: Maven `mvn -q test` (run via `mvn -q exec:java`) or Gradle `./gradlew test run` in `java/`
- **C++**: Simple build `g++ -std=c++17 -O2 main.cpp -o main && ./main`; or CMake `mkdir build && cd build && cmake .. && cmake --build . && ctest`
- **Rust**: `cd rust && cargo run` / `cargo test`
- **C# (.NET)**: `cd csharp && dotnet run` / `dotnet test`
- **Testing**: Run corresponding language test commands in each algorithm directory
- **Formatting**: Go `gofmt`; Python `black`/`autopep8`; JS/TS `prettier` + `eslint`; Java `google-java-format` or Spotless; C++ `clang-format`; Rust `rustfmt` + `clippy`; C# `dotnet format`

## Coding Standards
- **Go**: Use `gofmt` for formatting; functions and variables use camelCase; package names use lowercase
- **Python**: Follow PEP 8 standards; use snake_case naming; classes use CamelCase
- **JavaScript/TypeScript**: camelCase for variables/functions, PascalCase for classes/types; lint with ESLint
- **Java**: Packages lowercase; Classes PascalCase; methods/variables camelCase; constants UPPER_SNAKE_CASE
- **C++**: Prefer consistent style; recommend Google C++ Style (Types PascalCase, functions lowerCamelCase, constants kPrefix)
- **Rust**: snake_case for functions/variables; PascalCase for types/traits; use `rustfmt`
- **C#**: PascalCase for types/methods; camelCase for locals/fields; namespaces PascalCase
- **General**: Variable names should be meaningful, avoid single-letter variables; add necessary comments

## Testing Standards
- **Go**: Use built-in testing package, test files end with `_test.go`
- **Python**: Use unittest or pytest framework, test files start with `test_`
- **JavaScript/TypeScript**: Use Jest/Mocha/Vitest; tests `*.test.ts|js` under `__tests__/` or alongside sources
- **Java**: Use JUnit; test classes end with `*Test.java`
- **C++**: Use GoogleTest or Catch2; test files end with `_test.cpp`
- **Rust**: Use built-in `cargo test`; integration tests under `tests/`, unit tests with `#[cfg(test)]`
- **C#**: Use xUnit/NUnit/MSTest; test projects named `*Tests`
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
