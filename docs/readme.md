# new version update


https://github.com/css-modules/css-modules/pull/238

https://gist.github.com/xgqfrms-GitHub/16967b1b62afc156bae5162ca459be7e


# CSS Modules with React


https://github.com/css-modules/css-modules/blob/master/docs/css-modules-with-react.md

https://github.com/gajus/react-css-modules




## Demo.js

```js

import React from 'react';
import CSSModules from 'react-css-modules';

// import your css modules styles for the component
import styles from './Demo.css';

const Demo = (props) => {
    // 解构赋值
   const {route} = props;
   return (
        <div styleName='demo'>
            <button styleName='button blue'>press me</button>
        </div>
    )
};

export default CSSModules(Demo, styles, {allowMultiple: true});

``` 

## index.js

```jsx

import React from 'react';
import ReactDOM from 'react-dom';
import Demo from './components/Demo';

const App = (props) => {
    return (
        <main>
            <Demo />
        </main>
    )
};

ReactDOM.render(React.createElement(App), document.getElementById('root'));

```
















