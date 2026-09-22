# ContactFlow

React + Vite contact management workspace.

## Run
```bash
npm install
npm run dev
```

This version uses port 5173 with strictPort so it stays on the same browser origin as earlier ContactFlow versions. Stop any older Vite app using port 5173 before starting this one.

## Storage
Contacts are stored in IndexedDB without a fixed ContactFlow count limit. Existing `cf_contacts` localStorage data is merged into IndexedDB on startup instead of being deleted. Deletions are persisted by replacing the IndexedDB collection, preventing deleted contacts from reappearing.
