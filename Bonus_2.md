# Bonus 2

This is an optional bonus question, so don't feel frustrated if you are not able
to finish it. For this question, you are required to use
[React](https://github.com/facebook/react) or
[Preact](https://github.com/developit/preact). We have to write a
`<StarWarsCharacters />` which will query the [Star War's
API](https://swapi.co/documentation#people) and get a list of Star Wars
characters, then it will display them as a list including their: 

### Requirements

* Query the `GET https://swapi.co/api/people/` endpoint.
* Once you get the data, each character should be displayed on a list.
* The following fields should be displayed: `name`, `birth_year`, `height`, and `mass`.

### Evaluation Criteria
* Should meet all the requirements
* Code structure
* Code quality
* React best practices
* Design is irrelevant, however feel free to add any CSS styling that you would
  like. We won't judge the styling.
* Because it is not in the list, it doesn't mean you can't get creative.
  Surprise us!
    
You don't have to setup `Webpack`
and/or `Babel` to transpile your JSX code. Feel free to use `babel-standalone`:

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width">
        <title>GumGum - Bonus 1</title>
        <script crossorigin src="https://unpkg.com/react@16/umd/react.development.js"></script>
        <script crossorigin src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
        <script src="https://unpkg.com/babel-standalone@6.26.0/babel.min.js"></script>
        <script type="text/babel">
            
            /* ----------------------------------- *
             *      WRITE YOUR JAVASCRIPT HERE
             * ----------------------------------- */
        
            class StarWarsCharacters extends React.Component {
                render() {
                    return (
                        <p>Star Wars - Characters List</p>
                    );
                }
            }
            
            ReactDOM.render(
                <StarWarsCharacters />,
                document.getElementById('root')
            );
        </script>
    </head>
    <body>
        <div id="root"></div>
    </body>
</html>
```

