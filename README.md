[१३:३०, ५/९/२०२२] Puja Tirupati Neralwar: Lifecycle -2


import React from 'react'

import '../styles/App.css';


class App extends React.Component {

  handleClick(){
    this.setState({count: this.state.count+1})
  }
  constructor(props){
    super(props)
    this.state = {count:0}
    this.handleClick = this.handleClick.bind(this);

  }

  componentDidMount(){
    console.log('mounted')
  }
  
  render() {
    console.log('rendered')
    return (
      <div id="main">
          <div id="count">{this.state.count}</div>
          <button id="incr" onClick={this.handleClick}>Increment</button>
      </div>
    )
  }
}


export default App;
[१३:३०, ५/९/२०२२] Puja Tirupati Neralwar: //React life cycle 1

import React from 'react'

import '../styles/App.css';


class App extends React.Component {

  

  handleClick(){
    this.setState({count: this.state.count+1})
  }
  constructor(props){
    super(props)
    this.state = {count:0}
    this.handleClick = this.handleClick.bind(this);
  }

  render() {
    console.log("rendered")
    return (
      <div id="main">
          <div id="count">{this.state.count}</div>
          <button id="incr" onClick={this.handleClick}>Increment</button>
      </div>
    )
  }
}


export default App;
==============================================
<input type="number" min="1" max="9" id="wall_id">
   <input id="wall_color">
  <button id="apply" onclick="changeHandler()">Change</button>
  <button id="reset"onclick="resetHandler()">Reset</button> <br><br>
 
  <div id="1" value="1"></div>
   <div id="2" value="2"></div>
    <div id="3" value="3"></div>
   <div id="4" value="4"></div>
   <div id="5" value="5"></div>
   <div id="6" value="6"></div>
   <div id="7" value="7"></div>
   <div id="8" value="8"></div>
   <div id="9" value="9"></div>
   ===========================================================
   function changeHandler(){
    // document.querySelector("`#${colorid}`").style.background=`${color}`
    var divs=document.querySelectorAll("div")
    divs.forEach(function findTarget(div){
      if(div.getAttribute("id")==colorid){
        div.style.background=color

      }
      else{
        div.style.background="none"

      }
    })

  }
  function resetHandler(){
    var divs=document.querySelectorAll("div")

    divs.forEach(function findTarget(div){
      
        div.style.background="none"


    })
  }
  var coloridvalue=document.querySelector("#wall_id")
  var colorid
  var colorvalue=document.querySelector("#wall_color")
  var color
  colorvalue.addEventListener('input', updateValuecolour);
  coloridvalue.addEventListener('input', updateValueid);
  function updateValueid(e) {
    colorid= e.target.value;
  }
  function updateValuecolour(e) {
    color= e.target.value;
  }
  ===========================================================================
  div {
    width: 20px;
    height: 20px;
    border: 1px solid black;
    display: inline-block;
}
header {
    display: flex;
}
Asian paints ch ahe he
==========================================================================
function oddball_sum(array){
// write code here
// use console.log to display the output
 var count=0;
 for(var i=0;i<array.length;i++){
     if(array[i]%2===1){
         count+=array[i];
     }
 }
 console.log(count);

}
oddball sum
============================================================================
