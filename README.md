al-haram-store/
├─ README.md
├─ docker-compose.yml
├─ .env.example
├─ frontend/                # React / Next.js app
│  ├─ package.json
│  ├─ src/
│  └─ public/
├─ backend/                 # Node.js (Express/Nest) APIs
│  ├─ package.json
│  ├─ src/
│  ├─ migrations/
│  ├─ seeds/
│  └─ Dockerfile
├─ infra/                   # infra scripts: nginx, certbot, deploy scripts
│  ├─ nginx/
│  └─ docker/
├─ db/                      # optional - SQL files, init scripts
└─ tests/
   ├─ unit/
   └─ e2e/
