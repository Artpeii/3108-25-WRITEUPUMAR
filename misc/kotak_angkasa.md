# Kotak Angkasa

<img width="623" height="704" alt="image" src="https://github.com/user-attachments/assets/3470011e-5a8a-4ad1-80a8-6c0cf4930c63" />

Click the link

<img width="1080" height="487" alt="image" src="https://github.com/user-attachments/assets/df2cab77-c586-4303-abfd-e86f44440c8f" />

Solve the Rubik's Cube and copy the flag
Flag: 3108{Sh31kh_MuZ4ph4r_5p4c3_73219} 

### Takeaways:
- I realise by reading others' write-ups, you can modify the JavaScript of the cube to the solved state.
- Nonetheless, solving the puzzle was fun xD
- This is the code btw: <br>
  *note: the code isn't from me okay* <br>
`const cube = { 
front:  Array(9).fill("green"), 
back:   
Array(9).fill("blue"), 
left:   
Array(9).fill("orange"), 
right:  Array(9).fill("red"), 
top:    
Array(9).fill("white"), 
bottom: Array(9).fill("yellow") 
}; 
socket.emit("cubeState", cube);`






