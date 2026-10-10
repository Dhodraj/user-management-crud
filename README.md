# user-management-crud

Add, list, edit and delete users. React on the front, an Express API in the middle, MySQL at the back.

Built in August 2021.

https://user-images.githubusercontent.com/83802185/129373119-882e29ca-04cd-4c77-a959-25c57c7b7df0.mp4

## API

| Method | Path | What it does |
|---|---|---|
| POST | `/create` | adds a user |
| GET | `/details` | lists all users |
| PUT | `/updatefname`, `/updatelname`, `/updatemail` | changes one field |
| DELETE | `/delete/:id` | removes a user |

The API listens on port 3005. It connects to MySQL on localhost as `root` and uses a database named `crud` with a table named `data`.

## Run it

The repository has no `package.json` files, so install the packages by hand.

```bash
cd backend
npm install express mysql cors
node index.js

cd ../my-app
npm init -y
npm install react react-dom react-scripts react-router-dom axios formik @material-ui/core @material-ui/icons
npx react-scripts start
```
