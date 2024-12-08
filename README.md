# TuneLink Server
Backend to [Tunelink](https://github.com/hannajiangg/TuneLink) built with MongoDB, Express.js, and Swagger UI for documentation.

## Set up instructions

1. Clone this repository to your work directory
2. Navigate into `tunelink-backend` (this repo) directory
3. Run `npm i`, this will install all required packages for the backend
4. Create a `.env` at root and copy contents of `.env.copy` into there, message on groupchat to get secrets, or remind ozel to email you, or download on provided drive link.
5. download .env from this url `https://drive.google.com/file/d/1CXZcNirtCNC43OU_aRnYcX-yG6y0CEGw/view?usp=sharing`.
5. Remind Ozel to give you access to mongodb, not required but it is helpful, for development purposes.
6. Navigate to `data/`
7. Unzip `test_data.zip`.
8. Remove contents of `test_audio` directory.
9. Go to `https://drive.google.com/drive/folders/1vvtAXnvMvA6ErBT0sbgSsn79shp8YUKL?usp=sharing` to download uncompressed audio files, place them in `test_audio` directory.
10. You can add more files if you want, but should be uncompressed.

You are ready to run the backend

## Run the server

1. After you have set up, run `npm start` to start the server
2. You can navigate to `localhost:3000/health` to check health status of the server

## Routes For Development, developers please read
- `localhost:3000/api-docs`
    - An interactive api documentation page that lists available routes

## Populating database
- Make sure you have the test_data, inside data directory
- Run `npm test -- tests/uploadRoutes.test.js` to run tests that will populate the database
