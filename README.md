# Calendar in Vanilla Javascript, then transformed in react app

Using snowpack for bundling the app

npm install
npm start

## Javascript

http://localhost:8080/vanilla

vanilla.html
vanillaScript.js
vanillaStyle.css

## React version

http://localhost:8080/

index.html
style.css
src/index.jsx
Sub-folders containing react components created from the vanilla version
- src/App : the Higher components that wrapped the other ones
- src/CalendaerHeader
- src/Day
- src/DeleteEventModal
- src/NewEventModal
- src/hooks/useDate.js : reduce the size of src/App: the code inside useDate.js is actually the useEffect section of the App.js, creating this javascript hook simplify the src/App implementation and makes it more clear

Note: using snowpack dev mode (npm start = snowpack dev): the index.html must reference the compiled version of jsx, that is src/index.js, instead of src/index.jsx
