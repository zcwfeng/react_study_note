![David|chuanwei.zhang](https://github.com/zcwfeng)
##React Hello World


###html 不用jxf

```
<div id="container">
<!-- This element's contents will be replaced with your component. -->
</div>
```

>对应的React

```
var Hello = React.createClass({
displayName: 'Hello',
render: function() {
return React.createElement("div", null, "Hello ", this.props.name);
}
});

ReactDOM.render(
React.createElement(Hello, {name: "World"}),
document.getElementById('container')
);

```

###HTML 带有JSF

```
<script src="https://facebook.github.io/react/js/jsfiddle-integration-babel.js"></script>
<div id="container">
<!-- This element's contents will be replaced with your component. -->
</div>
<script src="https://facebook.github.io/react/js/jsfiddle-integration-babel.js"></script>
<div id="container">
<!-- This element's contents will be replaced with your component. -->
</div>
```

>对应的REACT

```
var Hello = React.createClass({
render: function() {
return <div>Hello {this.props.name}</div>;
}
});

ReactDOM.render(
<Hello name="World" />,
document.getElementById('container')
);

```
