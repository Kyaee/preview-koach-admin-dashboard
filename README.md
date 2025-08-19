# preview-koach-admin-dashboard

<!--
Use the following template to describe your PR. Feel free to remove any unused portions!
-->

## Status: :construction: In development
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

<!--
- [ ] Tests
- [ ] Documentation
-->

## Screenshots 
**Initial UI** `/admin/coach`
<img width="1850" height="937" alt="Screenshot 2025-08-01 022400" src="https://github.com/user-attachments/assets/78bce642-4033-434b-9d0a-e78d7c461851" />

**On Hover of Status Pill: Changes display based on application status**
<img width="1849" height="939" alt="Screenshot 2025-08-01 022431" src="https://github.com/user-attachments/assets/47b7c346-e02c-4fc9-90e7-c9547349429a" />

### A/B Testing of Status Guide Component
> Reused existing styles from global components & both are mobile responsive.
> Carousel was pushed :33 but lemme know if I should push the Table instead of the Carousel

1. Carousel<img width="1846" height="870" alt="Screenshot 2025-08-01 022538" src="https://github.com/user-attachments/assets/52af434f-809c-4e25-beba-efa5440b837d" />
2. Table<img width="1844" height="938" alt="Screenshot 2025-08-01 022816" src="https://github.com/user-attachments/assets/80ae96c1-96aa-4fc3-99f6-f61c082666fc" />



### Update and Confirm Coach Application
**Initial Dialog Update component**<br/>
Behavior: Opens a dialog when clicking an applicant
<img width="1847" height="907" alt="Screenshot 2025-08-05 193130" src="https://github.com/user-attachments/assets/ecdada79-73ff-4772-860c-fc332870ac1e" />

**Initial Confirm Changes Component - Dialog Confirm Component**<br/>
Behavior: After clicking `Confirmed Changes`, display another modal to confirm changes<br/>
State: **Inputting the Confirmed Text Input**<br/>
<img width="1846" height="908" alt="Screenshot 2025-08-05 193350" src="https://github.com/user-attachments/assets/9f98532d-549d-43ea-8d55-95ef3e9c3b1e" />


State: **If the Coach Application Status is ABANDONED or REJECTED**
<img width="1848" height="907" alt="Screenshot 2025-08-05 193508" src="https://github.com/user-attachments/assets/1c57ddb3-97c1-4955-9a42-a4e9bcf4d67c" />

State: **If Admin wants to restore all status option, they proceed with Restore Mode**
<img width="1848" height="908" alt="Screenshot 2025-08-05 193546" src="https://github.com/user-attachments/assets/1e560d8d-8d5c-4f8c-a0b7-3c1a56c84724" />

**By clicking it, they can select other options**
<img width="1847" height="906" alt="Screenshot 2025-08-05 193614" src="https://github.com/user-attachments/assets/3b25f3f6-225b-49dc-81b1-7374f835306b" />



<!--
Mac OS Screenshots: ctrl + shift + cmd + 3 (entire screen) or 4 (selection of screen), then paste in editor
Mac OS GIFs: Try using Kap
Linux/Windows: Ctrl + Alt + PrintScreen (of a window) or Ctrl + Shift + PrintScreen (selection of screen), then paste in editor
-->
