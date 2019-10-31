# AutoCompete, a Programming Contest
AutoCompete is an monthly programming contest organized by Steve Geluso put on
by Flatiron School held in Seattle, WA. Teams of up to three people work
together competing to solve the most problems in 90 minutes. The problems come
from a problem packet custom created each month.  Teams can use whatever
programming language they want. The problems are designed for programs to read
from standard input and write to standard output. Check out the problems from
previous events!

## Previous Problem Sets
* [2019-07-25: Sum, How Many Anagrams?, Phone Screen, A Knights Tail, Prime Factorization, Determine File Type, Number Pyramid, Probably Spelled Correctly](./problem-sets/2019-07-25.md)
* [2019-06-13: dlroW olleH, N-ibonacci, Cipher, Tag, Minesweeper, Cave, Fuzz Bizz](./problem-sets/2019-06-13.md)

## Flatiron Seattle AutoCompete Rules
* Up to three people per team
* Only one computer per team
* Pen and paper will be provided
* Internet access is allowed (though probably mostly unuseful)
* No third party libraries (no gems, no pip, no npm, etc)
* You may solve problems in any order
* Rankings are ordered by the number of problems solved and time taken

## Sample Boiler Plate
All of the programs are required to read input from STDIN (standard input).
Each language has it's own way of accessing this input. Here are samples to
get you started. You can use this boilerplate to build the rest of your
programs around, or read from STDIN any other way you wish.

If you have a text file called `input` and a program called `foo` (in whatever
language) you can have the program read the file input by executing the
following in your bash terminal. The `cat` command prints the contents of
the `input` file and "pipes" the output as input for your program. Your program 
reads from STDIN and reacts to the input.

```
cat input | python foo.py
cat input | ruby foo.rb
cat input | node foo.js
```

Try this out to make sure your programs execute correctly!

**Python 3**
```py
import fileinput
for line in fileinput.input():
  print(line)
```

**Ruby**
```ruby
lines = ARGF.read.split("\n")
lines.each do |line|
  puts line
end
```

**JavaScript**
```js
const readline = require('readline');
const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout,
  terminal: false
});

const lines = []
rl.on('line', (line) => lines.push(line));
rl.on('close', (line) => execute(lines));

function execute(lines) {
  console.log(lines)
}
```

