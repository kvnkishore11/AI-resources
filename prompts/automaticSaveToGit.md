PROMPT WITHIN CONTEXT WINDOW

Generate a comprehensive Git commit message for the changes I've made and provide appropriate code comments following these guidelines:

1. FORMAT FOR COMMIT MESSAGE:
   - Title: <type>: <concise summary>
   - Body: Detailed explanation with bullet points
   - Footer: References to issues/PRs (if applicable)

2. TYPES:
   - feat: A new feature
   - fix: A bug fix
   - docs: Documentation changes
   - style: Code style changes (formatting, missing semi-colons, etc)
   - refactor: Code changes that neither fix bugs nor add features
   - perf: Performance improvements
   - test: Adding or fixing tests
   - chore: Changes to build process, dependencies, etc
   - revert: Reverting a previous commit

3. TITLE GUIDELINES:
   - Use imperative mood ("Add" not "Added")
   - Keep under 50 characters
   - No period at the end
   - Be specific and descriptive

4. BODY GUIDELINES:
   - Explain WHAT was changed and WHY (not HOW)
   - Use bullet points with hyphens for multiple points
   - Wrap text at 72 characters
   - Include context and motivation for changes
   - Mention any significant dependencies

5. CODE COMMENT GUIDELINES:
   - Add comments for each significant change in the code
   - Format: // [<type>] <explanation and rationale>
   - Example: // [fix] Removed unused variable to prevent memory leaks
   - For multi-line changes, use block comments with the same format
   - Ensure comments explain both WHAT was changed and WHY
   - Comments should align with descriptions in the commit message
   - Place comments directly above the changed code when possible

6. EXAMPLES OF ALIGNED COMMIT MESSAGES AND CODE COMMENTS:
   - Commit: fix: resolve unused variable warnings
     Code comment: // [fix] Removed unused imports to eliminate console warnings and improve performance

   - Commit: refactor: simplify user authentication flow
     Code comment: /* [refactor] Simplified authentication logic
      * Reduced nested conditionals for better readability
      * Improved error handling with specific error messages
      */

Remember to focus on the purpose and impact of the changes, not just listing the files modified. The code comments should provide context for future developers (including yourself) about why specific changes were made.