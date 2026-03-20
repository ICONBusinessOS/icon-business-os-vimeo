# ICON BusinessOS — Vimeo Integration

> Operations intelligence for Vimeo. Monitor video library health, engagement trends, and content pipeline from within the ICON BusinessOS platform.

## Features

- **Video Operations Score**: library health, engagement trends, storage utilization
- **Engagement Intelligence**: play rate, finish rate, comment velocity, like trends
- **Content Pipeline**: upload velocity, draft/published ratio, scheduled releases
- **Distribution Health**: embed stats, domain distribution, privacy compliance audit

## Vimeo API Endpoints Used

| Endpoint | Signal |
|----------|--------|
| `GET /me` | Account health, storage quota, plan tier |
| `GET /me/videos` | Video inventory, upload velocity |
| `GET /videos/{id}/stats` | Play count, finish rate, engagement |
| `GET /me/albums` | Collection/showcase organization |
| `GET /me/projects` | Project-based content pipeline |
| `GET /videos/{id}/privacy/domains` | Distribution/embed audit |

## Setup

1. Create app at https://developer.vimeo.com/apps
2. Auth: OAuth 2.0 Authorization Code Grant
3. Scopes: `public`, `private`, `video_files`, `stats`
4. Redirect URI: `https://os.theicon.ai/api/oauth/vimeo/callback`
5. Connect via ICON BusinessOS dashboard

## Requirements
- Vimeo account (Basic through Enterprise)
- OAuth 2.0 app registered with Vimeo

## License
MIT
