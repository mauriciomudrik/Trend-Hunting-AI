# User Deletion

## 🇺🇸 English: What happens when deleting a user?

When requesting the deletion of a user through the administration panel, you have the following options available to manage the data tied to that account:

1. **Perform backup and send to the user's email**:
   - The system will compile all user data, as well as the data from projects where they are the sole owner, including collected posts, metrics, and keys.
   - A structured JSON file containing this information will be automatically attached and sent to the user's registered email address.

2. **Remove all related data (projects, posts, API configurations, and OAuth)** (Deep Wipe):
   - If this option is checked, not only will the user be removed, but the system will permanently wipe all projects where this user is the exclusive member.
   - This ensures the immediate termination of collections (posts), API keys (API Configurations), and active OAuth or scraping sessions registered under the user's account for those projects.
   - **Deletion Audit (Log)**: Whenever this deep wipe action is executed, the system's API will internally create a detailed text log file. This log will list each deleted project and describe each API or OAuth key removed, enabling compliance and confirming the deletion of sensitive digital assets.
