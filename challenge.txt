function removeDupe(inpArr) {
  let outArr = [];
  console.log(`input is: ${inpArr}`)

  inpArr.forEach(function(characters) {
    if (outArr.includes(character)) {
      return
    }
    else {
      outArr.push(character)
    }
  });

  return outArr
}

let response = removeDupe([1,2,"dog",2,3,"dog"])

console.log(`output is: ${response}`)



-----------------------------------------

const removeDupe = arr => arr.filter((character,index) => arr.indexOf(character) === index);


let inp = [1,2,"dog",2,3,"dog"]
console.log(`input is: ${inp}`)

let response = removeDupe(inp)

console.log(`output is: ${response}`)

------------------------------------------
outArr = []

const fakeForLoop = (counter, inp) => {
  if (counter >= inp.length){
    return
  } else {
    if (outArr.includes(inp[counter])) {
      return fakeForLoop(counter + 1);
    } else {
      outArr.push(inp[counter])
    }
  }
  return outArr
} 

let inp = [1,2,"dog",2,3,"dog"]
console.log(`input is: ${inp}`)

let response = fakeForLoop(0, inp)
console.log(`output is: ${response}`)