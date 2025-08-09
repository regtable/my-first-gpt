# Memory System
- This folder holds memory data for this user.

## Structure
/memory/per_chat/     - Local memory scoped to individual chat sessions.
/memory/global/          - Shared memory accessible across all sessions.

## GPTMemoryUtilization
* The GPT will decide what is safe to store in /global/ as opposed to /per_chat/
 - Example: Facts like "user likes the color blue" can be saved in global memory
 - Example: Passwords or financial data must never be global.

* Per-chat memory is reset at the start of each new session.
