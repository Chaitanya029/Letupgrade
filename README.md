# Letupgrade
// REACTjs basic back toggle 
import React, { useState } from 'react';

function App() {
  // Define a state variable to store the current color
  const [color, setColor] = useState('white');

  // Define a function to toggle the color between white and black
  function toggleColor() {
    if (color === 'white') {
      setColor('black');
    } else {
      setColor('white');
    }
  }

  // Return the JSX element that renders the web page with the current color and a button to toggle it
  return (
    <div style={{ backgroundColor: color, height: '100vh', display: 'flex', justifyContent: 'center', alignItems: 'center' }}>
      <button onClick={toggleColor}>Toggle Color</button>
    </div>
  );
}

export default App;
