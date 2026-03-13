# Stable Backup: v1.0 Client-Only Architecture

This is a backup of the stable client-only version of Liquid Glass Chat.

## Architecture
- **Pure client-side**: Swift native layer directly calls OpenAI API
- **No backend dependency**: All data stored locally via SwiftData
- **API Key**: User provides their own OpenAI API key, stored on device
- **Recovery**: Polling-based recovery using `store: true` + GET response

## Features
- Streaming chat with OpenAI Responses API
- Reasoning/thinking display with collapsible UI
- Tool calls: web search, code interpreter, file search
- File upload support
- Background recovery via polling
- Multiple conversations with local persistence

## Files
- `ios/` — All Swift source files (native chat module)
- `server/` — Server files (unused in this version)
- `app.config.ts` — Expo app configuration
- `todo.md` — Feature tracking
- `design.md` — UI design document
