# preview-koach-admin-dashboard

<!--
Use the following template to describe your PR. Feel free to remove any unused portions!
-->

## Status: :construction: In development
❗ For testers, run `yarn install --frozen-lockfile`. I added a new package `react-papaparse`
<!--
Copy-paste one of the following three lines outside this comment

:rocket: Ready
:no_entry_sign: Do not merge
-->

## Description

PR that includes the following features:
1. **Add UI helpers that provides context to application statuses:**
    - Display description about a coach application once a status label is hovered
    - Implement a help icon or text element located above the coach application table. When clicking, will implement a modal that displays a comprehensive "Coach Application Guide" table, outlining each status's meaning and associated admin actions.
2. **Additional Confirmation for Admin Status Changes:**
    - Show an additional confirmation dialog, when an admin changes a coach's application status
    - Text indicating that "This action cannot be undone. The application cannot be reverted to a previous status after saving."
    - Hide previous statuses upon admin change, preventing reversion of status.
3. **Export filtered table data as `.CSV` file** 
<!--
A few sentences describing the overall goals of the pull request's commits.
-->

## Todos
- [x] UI helpers for coach application statuses
- [x] Create storybook for UI helpers?
- [x] Confirmation for Admin Status Changes
- [x] Export filtered table as CSV
- [ ] Fix stories deployment issue

<!--
- [ ] Tests
- [ ] Documentation
-->

## Screenshots
Initial UI `/admin/coach`
<img width="1850" height="937" alt="image" src="https://github.com/user-attachments/assets/36ad1e05-cad5-487c-b928-de9b9f42bae3" />

On Hover of Status Pill: Changes display based on application status
<img width="1849" height="939" alt="image" src="https://github.com/user-attachments/assets/d52bebfa-18cc-4fdb-8b97-e3932252cfe8" />

A/B Testing of Status Guide Component
> Reused existing styles from global components & both are mobile responsive.
> Carousel was pushed :33 but lemme know if I should push the Table instead of the Carousel

1. Carousel<img width="1846" height="870" alt="image" src="https://github.com/user-attachments/assets/6f3bb09b-f5d2-4ad4-b1c2-6c52739bce52" />
2. Table<img width="1844" height="938" alt="image" src="https://github.com/user-attachments/assets/75cdd2cd-a6fe-4ccd-a701-99240e7be1b6" />


<!--
Mac OS Screenshots: ctrl + shift + cmd + 3 (entire screen) or 4 (selection of screen), then paste in editor
Mac OS GIFs: Try using Kap
Linux/Windows: Ctrl + Alt + PrintScreen (of a window) or Ctrl + Shift + PrintScreen (selection of screen), then paste in editor
-->
