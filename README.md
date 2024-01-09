import inquirer from "inquirer";

const answer:{
    sentence: string
} = await inquirer.prompt([
    {
        name: "sentence",
        type: "input",
        message: "Enter Your Sentence To Count The Words :"
    }
])

const Words = answer.sentence.trim().split(" ") 
console.log(`Your Sentence Word Count Is ${Words.length}`)
