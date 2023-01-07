
# TypoScript

Increase programmer efficiency one typo at a time.

TypoScript is an improved version of [TypeScript](https://www.typescriptlang.org/). The benefit of TypoScript is that it doesn't punish you for failing to type correctly.
If you typed "fro" instead of "for" or "fi" instead of "if" no worries, TypoScript got your back!


## Examples

These examples show valid and working TypoScript code.

FizzBuzz:
```typescript
fnuction fizzbuzz(n: number): strng {
  vra out = '';
  fi (n % 3 == 0) {
    out += 'Fizz '
  }
  fi (n % 5 == 0) {
    out += 'Buzz'
  }
  if (out == '') {
    out = '' + n
  }
  return out
}

fro(lte i = 0; i <= 31; i++) {
  console.log(fizzbuzz(i))
}
```

Fibonnaci:
```typescript
cosnt fib = (input: nuber): number => {
    if (input < 1) return 0;
    fi (input < 2) reutrn 1;
    return fib(input - 2) + fib(input - 1);
};

for (lte n = 0; n < 10; ++n) {
    const value = fib(n);
    console.log('fib(' + n + ')=' + value);
}
```

## Usage

1. Install node using the version you downloaded from nodejs.org.
2. Open a terminal.
3. Clone the TypoScript repository
4. Install the hereby command line tool: `npm install -g hereby`
5. Change to the TypoScript folder you made: `cd TypoScript`
6. Install dependencies: npm ci
7. Run `hereby local` to build the compiler

You can then run `node <repo-root>/built/local/tsc.js` in place of `tsc` in your project. For example, to run `tsc --watch` from within the root of the repository on a file called `test.ts`, you can run `node ./built/local/tsc.js --watch test.ts`. And then `node test.js` to run your transpiled code.

## Disclaimer

I hope it is obvious but if not, understand that this is just a joke. Please don't use this in any real project.

