# Introduction to Julia

This Readme is intended to get you up and running with Julia. 

## Install Julia

* install Julia on your computer (two options, choose one)
	* Easy method:
		* Download from website [Julia Downloads](https://julialang.org/downloads/)
		* Choose the Julia version for your operating system
	* Optional method: 
		* If you use homebrew, you can use it to install Julia
		* `brew cask install julia`
* install the Julia notebook kernel "IJulia"
	* open "julia" REPL by typing "julia" in your terminal. this should start the Julia REPL and a "julia>" command prompt should appear.
	* Then, install IJulia for the jupyter notebook kernel:
		using Pkg
		Pkg.add("IJulia")
	* then exit by typing 
		exit()
* assuming you have Jupiter notebooks already installed, 
	* start a new new notebook server by typing (in your terminal, not in julia)
		jupyter notebook
	* then, create a new notebook with a julia kernel by creating a new notebook and picking "Julia" from the dropdown menu
* Then, install the "Plots" package by typing
	* using Pkg
	* Pkg.add("Plots")

## Julia Overview

### Julia Advantages

* easy to learn and to switch from other popular languages
	* direct interfaces with C libraries
	* syntax is similar to math equations
* quick to prototype new code
	* dynamic typing
	* REPL environment (enabled by JIT compilation)
* fast (in many ways)
	* compiled and faster than C for large numerical computations
	* ability to do fine-grained memory-management  enables native parallelization and optimization
* tighter integration with shells and system-processes than Python

### Julia Disadvantages
* TERRIBLE startup time for many common data exploration tasks due to JIT compilation -- plotting often takes >20s
* immature tools 
	* debugger introduced in Julia 1.3 is limited, most packages are still in alpha or beta stage of development and have bugs

### Julia Tutorials

[Julia - a concise tutorial](https://syl1.gitbook.io/julia-language-a-concise-tutorial/)

[Julia by example](https://juliabyexample.helpmanual.io/)

[Intro to Julia by UCI Datascience](http://ucidatascienceinitiative.github.io/IntroToJulia/)

[Julia Express PDF](http://bogumilkaminski.pl/files/julia_express.pdf)



