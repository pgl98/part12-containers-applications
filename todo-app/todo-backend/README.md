# Express application

Install dependencies with `npm install`

Run with `npm start`

Or in development mode with `npm run dev`

# Visit counter

When running the server, visit http://localhost:3000 to see visit counter, or give environment variable `PORT` to change the port.

# MongoDB

The application has /todos crud which requires a MongoDB. Pass connection url with env `MONGO_URL`

# Redis

Pass connection url with env `REDIS_URL`

# Notes

1. Had to change the image in the docker-compose.dev.yml file from 'mongo' to 'mongo:4.4.9-focal' since the former led to the following error:
    WARNING: MongoDB 5.0+ requires a CPU with AVX support, and your current system does not appear to have that!
      see https://www.mongodb.com/community/forums/t/mongodb-5-0-cpu-intel-g4650-compatibility/116610/2
      see also https://github.com/docker-library/mongo/issues/485#issuecomment-891991814
      
   It turns out I don't have a CPU with AVX support.
