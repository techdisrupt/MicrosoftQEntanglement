# Introduction to Quantum Programming with Microsoft

If you ever wondered how to use Microsoft Products in creating quantum algorithms, here is a very minimal example piece of code based on a Microsoft example. However the reason the code exists here in this repo is that there appears to be quite a few issues in the community of getting this code to run and work correctly.

Also you can think of this repo as another way to jump start your entry into using Quantum Tools from Microst, if you cannot be bothered to follow the step by step example and you simply want to get some base code running. If you want to see more explanation of the routines and code, you can work through the example [here](https://docs.microsoft.com/en-us/quantum/quantum-writeaquantumprogram?view=qsharp-preview&tabs=tabid-vs2017)

# What you need for this example

1. VScode (Microsoft Visual Studio Code) (This is a fantastic Microsoft Editor). [Get MS Visual Studio Code](https://code.visualstudio.com/download)

2. This repo.
3. Some basic knowledge of coding.
4. Some elementary understanding of Quantum Coding or Quantum Information.

# The code in the repo

1. Bell.qs (Base code that creates creates the Qubits, Bell States and performs operations on the Qubits)
2. Driver.qs (The entry point, this is where we run the multiple simulations)
3. Bell.csproj (The XML C# project file)

# Installing and running

1. Get the cold.
2. Open the folder in VScode.
3. Go to the terminal tab, and type: `dotnet run`

# Expected output

You should see something like this:

```
Init:Zero 0s=499  1s=501  agree=1000
Init:One  0s=521  1s=479  agree=1000
Press any key to continue...
```

## Quantum Statistics

This is for a thousand runs, essentially the code is measuring the output of a Qubit after being placed into an initial state and then being operated upon with a Hadamard Transformation (H) and then we measure the number of 0's and 1's or |0> or |1>. This by it's very nature is probabalistic so you will likely see a very different number of 0s and 1s, but you should not deviate too far from 500 each, or a 50%-50% split.

## Quantum Entanglement

Applying the Hadamard and CNOT to a pair of Qubits, we create an entangled state. This means that if we measure the first Qubit and the second, we will expect 100% agreement. As you can see from the output this is the case as we have generated the Bell state: |00> + |11>. Be don't know whether we get |00> or |11> but we do always have either 00 or 11 and hence always agree. 





















