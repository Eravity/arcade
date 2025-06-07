/code-coach/
│
├── /src/
│   ├── /api/             # (optional) Express routes, if needed later
│   ├── /scripts/         # Entry points (task checkers, generators, etc.)
│   │   └── checkTasks.ts
│   ├── /core/            # Core logic modules
│   │   ├── taskManager.ts       # Logic for reading/parsing .md tasks
│   │   ├── aiService.ts         # OpenAI/GPT interactions
│   │   ├── dbService.ts         # JSON DB operations (xp, rewards, etc)
│   │   └── markdownService.ts   # Read/write .md files
│   ├── /types/           # TypeScript interfaces and types
│   │   └── Task.ts
│   └── config.ts         # Centralized config (paths, API keys)
│
├── /data/                # Persistent app data (your vault and db)
│   ├── /vault/           # Folder watched by Obsidian
│   └── db.json           # XP, tasks, rewards, status etc.
│
├── /scripts/             # Optional: command-line wrappers
│   └── run-checker.sh
│
├── .env                  # API keys, local config
├── package.json
├── tsconfig.json
└── README.md
