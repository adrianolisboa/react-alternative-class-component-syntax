# react-alternative-class-component-syntax

[![Build Status](https://travis-ci.org/the-road-to-learn-react/react-alternative-class-component-syntax.svg?branch=master)](https://travis-ci.org/the-road-to-learn-react/react-alternative-class-component-syntax) [![Slack](https://slack-the-road-to-learn-react.wieruch.com/badge.svg)](https://slack-the-road-to-learn-react.wieruch.com/) [![Greenkeeper badge](https://badges.greenkeeper.io/the-road-to-learn-react/react-alternative-class-component-syntax.svg)](https://greenkeeper.io/)

React Class Components can be made much more concise using the *class field declarations*. You can initialize local state without using the constructor and declare class methods by using arrow functions without the extra need to bind them.

```
class Counter extends Component {
  state = { value: 0 };

  handleIncrement = () => {
    this.setState(prevState => ({
      value: prevState.value + 1
    }));
  };

  handleDecrement = () => {
    this.setState(prevState => ({
      value: prevState.value - 1
    }));
  };

  render() {
    return (
      <div>
        {this.state.value}

        <button onClick={this.handleIncrement}>+</button>
        <button onClick={this.handleDecrement}>-</button>
      </div>
    )
  }
}
```

## Installation

* `git clone git@github.com:the-road-to-learn-react/react-alternative-class-component-syntax.git`
* cd react-alternative-class-component-syntax-setup
* npm install
* npm start
* visit `http://localhost:8080`
