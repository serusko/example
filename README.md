# Example project

```bash
  /api # NestJs (backend) project folder
    # run on local PORT 3001 
    /dist # production build output - served by nginx on "/api.*" (locally on 3001 without prefix)
  /frontend # React (frontend) project folder
    # run on local PORT 3000
    /dist # production build output - served by nginx as root "/"
  /pgdata # Docker DB PostGres volume (can backup)
```

## TODO

- enable dev docker run (reuse env and run in dev mode)