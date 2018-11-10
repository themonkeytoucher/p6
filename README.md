# p6
Individual_DE' crossover function takes 2 genomes and splits it randomly into two parts. So one part could have 3 chromosomes and the other half
could have 1000 chromosomes. The function then takes the first half of self's genome and the second half of other's genome and combines them 
together to make the first child. It them takes the second half of self's genome and the first half of other's genome and combines them to make
the second child. Finally, it takes the two childs and chucks them into the mutation function.

The Individual_DE mutation function takes in a genome. As long as the genome is not empty, there is a 1% chance of the genome mutating. If it does mutate then it will choose a random chromosome to mutate. Once it chooses one, the function will look at the type of block it is. The typing of 
the genome can be found in the genome's 2nd element. The typing of the genome will determine how it will mutate. Suppose we had a genome that was of the typing "3_coin" then the function will find the typing and the associated available mutations. That genome can either move in the x position or move in the y position. After it has mutated a genome, it will pop the old genome and insert the new genome back into it's original spot via heappush.