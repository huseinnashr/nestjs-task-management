# NestJS Task Management Rest API

## What's this

Course work for [nestjs-zero-to-hero](https://www.udemy.com/course/nestjs-zero-to-hero/) course. See it live: [The Rest API](http://nvdhunter-task-management-prod3.us-east-1.elasticbeanstalk.com/) & [Front End](http://nvdhunter-task-management-frontend.s3-website-us-east-1.amazonaws.com/)

## How To Run

### Prerequisites

1. Install the docker desktop
2. run `docker-compose up -d` to run postgresql server & pgadmin

### NPM Script's

```bash
# Running on dev env in watch mode
npm run start:dev

# Running on prod env
npm run start:prod
```

### Environment Variable

```bash
JWT_SECRET=YOUR_SECRET_STRING

# Synchronize db schema with typeorm model
TYPEORM_SYNC=BOOLEAN

# (Optional)
# Add this when deploying to Elastic Beanstalk
# This fixes permission issue when installing package [1]
NPM_CONFIG_UNSAFE_PERM=true
```

### Other Configuration

```bash
.env
/config/
```

## Links

[[1] Deploy nodejs with elastic beanstalk permission problem](https://stackoverflow.com/a/52628534/8556970)
