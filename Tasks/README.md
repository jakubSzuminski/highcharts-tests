# Tasks for this Classroom

## Initial

1. Test two demos in the tests repository, by opening standard HTML file.
2. Change the assertion so it will check the number of points in the series instead of the number of series.
3. Write a new test, enable dataLabels and then check if dataLabels are visible on the graph.
4. Change series color, then write a new test, checking, if series color has changed correctly.
5. Change series type, then check if the series type has changed to your new type.

## QUnit

1. Write a test that will check some parameters in Highcharts and will pass with assert.equal but fail with assert.strictEqual
2. Write a test using assert.ok
3. Write a test with assertion that will break the code, then change the Qunit test so it will pass. Then edit it so it will fail, but not break the code.
4. Write tests for other Highcharts libraries (Maps / Stock / Gantt / Choosen module)
5. Write a QUnit module containing multiple tests, then write another one and disable it.
6. In the previous example, add the next module with test, then make the modules nested (grandparent -> parent -> child)

## Karma
1. Run tests through Karma for Highcharts library.
2. Write test that will fail, then run Karma again.
3. As a first test (alphabetically), create a test that will break Karma, then run it again. Then change it so it will fail instead of break.
3. Change location of testing files from test to "my-tests"
4. Add firefox as supported browser
5. Create callback function in example 6 from QUnit, so we will receive callbacks (beforeEach and afterEach) with info about the test we are "going to/from".
6. Change configuration so Karma will open chrome window on run
7. Change Karma configuration so it will not close after finishing last test.
8. Allow Karma to work with other Highcharts libraries (Maps / Stock / Gantt / Choosen module).

## Husky
1. Add Husky to your project, using `npm install husky -D`
2. Edit package.json > prepare script and run it once:
```
npm set-script prepare "husky install"
npm run prepare
```
3. Add a hook:
```
npx husky add .husky/pre-commit "npm test"
git add .husky/pre-commit
```
4. Make a commit
```
git commit -m "Keep calm and commit"
```

5. Check, if the Husky is working properly, then change the script so test will work on npm test-hc instead of npm test. 

6. If above works, make a commit again and check if Husky works, if not, make necessary adjustmennts.

# Pixelmatch

1. Add pixelmatch to your project, usign `npm install pixelmatch`
2. Create two images from the chart, moving one dataLabel couple of pixels off the second time.
3. Use pixelmatch to create an output of the difference image in test directory.