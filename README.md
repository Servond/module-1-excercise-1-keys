// 1
let strings = 'The QuIcK BrOwN FoX';
let splits = strings.split("");
for (let i = 0; i < splits.length; i++) {
    if (splits[i] === splits[i].toUpperCase()) {
        splits[i] = splits[i].toLowerCase();
    } else  {
        splits[i] = splits[i].toUpperCase();
    }
}
strings = splits.join("");
console.log(strings);

// 2
let int1 = 5;
let int2 = 10;

if (int1 == int2) {
    console.log('Numbers are the same')
} else if (int1 >= int2) {
    console.log(`${int1} is larger than ${int2}`)
} else {
    console.log(`${int2} is larger than ${int1}`)
}

// 3
let num1 = 11;
let num2 = 10;
let num3 = 10;

if (num1 <= num2 && num1 <= num3) {
    if (num2 <= num3) {
        console.log(`${num3}, ${num2}, ${num1}`)
    } else {
        console.log(`${num2}, ${num3}, ${num1}`)
    }
} else if (num2 <= num1 && num2 <= num3) {
    if (num1 <= num3) {
        console.log(`${num3}, ${num1}, ${num2}`)
    } else {
        console.log(`${num1}, ${num3}, ${num2}`)
    }
} else if (num3 <= num1 && num3 <= num2) {
    if (num1 <= num2) {
        console.log(`${num2}, ${num1}, ${num3}`)
    } else {
        console.log(`${num1}, ${num2}, ${num3}`)   
    }
}

// 4
let input = 0;
if (typeof input == 'string') {
    console.log(1)
} else if (typeof input == 'number') {
    console.log(2)
} else {
    console.log(3)
}




// 5
let sentence = 'An apple a day keeps the doctors away';
let splitSentence = sentence.split("");
for (let i = 0; i < splitSentence.length; i++) {
    if (splitSentence[i].toLowerCase() == 'a') {
        splitSentence[i] = '*'
    }
}
sentence = splitSentence.join("");
console.log(sentence);
