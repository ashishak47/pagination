## Simple react pagination component.

## Usage Exmaple
```javascript

function App() {
  let total = 173, perPage = 10;

  let [current, setCurrent] = React.useState(1);
  const onPageChanged = (page) =>{
    console.log("## page clicked " + page);
    setCurrent(page);
  } 
  
  return (
    <>
      <Pagination
        onPageChanged={onPageChanged}
        current={current}
        total={total}
        perPage={perPage}

      />
    </>
  );
}
```

### Props

<table class="table table-bordered table-striped">
    <thead>
    <tr>
        <th style="width: 100px;">name</th>
        <th style="width: 50px;">type</th>
        <th style="width: 50px;">default</th>
        <th>description</th>
    </tr>
    </thead>
    <tbody>
        <tr>
          <td>onPageChanged</td>
          <td>PropTypes.func.isRequired</td>
          <td></td>
          <td>callback for page change</td>
        </tr>
        <tr>
          <td>perPage</td>
          <td>PropTypes.number.isRequired</td>
          <td></td>
          <td>items to be shown on per page(to calculate total pages)</td>
        </tr>
        <tr>
          <td>total</td>
          <td>PropTypes.number.isRequired</td>
          <td></td>
          <td>total number of results(to calculate total pages)</td>
        </tr>
        <tr>
          <td>current</td>
          <td>PropTypes.number.isRequired</td>
          <td></td>
          <td>current page of pagination</td>
        </tr>
        <tr>
          <td>range</td>
          <td>PropTypes.number</td>
          <td>2</td>
          <td>Range for pagination. Number of pagination items to be shown before and after current page</td>
        </tr>
    </tbody>
</table>

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br>
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.<br>
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.<br>
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br>
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (Webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: https://facebook.github.io/create-react-app/docs/code-splitting

### Analyzing the Bundle Size

This section has moved here: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

### Making a Progressive Web App

This section has moved here: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

### Advanced Configuration

This section has moved here: https://facebook.github.io/create-react-app/docs/advanced-configuration

### Deployment

This section has moved here: https://facebook.github.io/create-react-app/docs/deployment

### `npm run build` fails to minify

This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify
