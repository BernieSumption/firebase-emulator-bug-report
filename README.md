## To reproduce bug

```
cd functions
npm i
npm run serve
```

Then visit: http://localhost:4000/logs
And in another tab, visit: http://localhost:5001/firebase-emulator-bug-repro/us-central1/helloWorld

The log message written by the helloWorld function causes the log UI to crash because it contains an empty array. Empty objects have the same effect.