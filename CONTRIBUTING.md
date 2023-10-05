## Handle Issues, Branches and PRs
TODO

## Writing Good Commit Messages

### Structure

The commit message usually has a structure like this:

```
<type>(<scope>): <subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
```

1. **Type**: A word that categorizes the purpose of the commit (e.g., `feat`, `fix`, `chore`, `docs`, `style`, `rf`, `perf`, `test`, see below). 
2. **Scope**: An optional part that refers to the module or feature that is affected by the commit (e.g., `auth`, `dashboard`).
3. **Subject**: A brief description of the changes, starting with a verb in the present tense (e.g., `add`, `fix`).
4. **Body**: Detailed explanatory text, if necessary. Wrap it to about 72 characters or so.
5. **Footer**: Any associated issues, or breaking changes, etc.

Valid Types:
Specifies the type of commit. This could be one of the following:
  - `feat`: A new feature.
  - `fix`: A bug fix.
  - `chore`: Routine tasks or maintenance. Should not modify code. 
  - `doc`: Documentation changes.
  - `style`: Code style changes (e.g., formatting).
  - `rf`: Code refactoring. Previously `refactor` but it was shortened to `rf` only
  - `perf`: Performance improvements.
  - `test`: Adding or modifying tests

### Examples

1. **Simple Commit**  
    ``` 
    fix: correct minor typos in code
    ```

2. **Commit With Scope**
    ```
    feat(auth): add login via Google
    ```

3. **Commit with Body and Footer**
    ```
    rf(core): extract calculate method
    
    Move the calculate method from `main.js` to `utils.js` to eliminate code duplication.
    
    Closes #123
    ```

Variant 2. or 3. should preferred.
  
### Best Practices

1. Use the imperative mood ("add" not "added", "fix" not "fixed").
2. Limit the first line to 72 characters or fewer.
3. Capitalize the subject line.
4. Do not end the subject line with a period.
5. Use the body to explain "what" and "why" vs. "how".
6. Reference issues or pull requests liberally after the first line.
