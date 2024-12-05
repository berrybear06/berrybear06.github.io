---
name: Polyfish (Polytopia AI)
ext-link: https://github.com/berrybear06/Tribes
project-order: 6
---
I'm working on an AI agent to play Polytopia. 
It's inspired by Google DeepMind's 
[AlphaStar](https://deepmind.google/discover/blog/alphastar-grandmaster-level-in-starcraft-ii-using-multi-agent-reinforcement-learning/) 
model to play StarCraft II, 
a similar game but played in real time and much more complicated. 
(And it's named after Stockfish for chess.) 
Technically, my current version plays 
[Tribes](https://cdn.aaai.org/ojs/7438/7438-52-10764-1-2-20200923.pdf), 
an open-source version of Polytopia, but 
I hope to adapt it to the real game after I figure out how to interface with it in code.

As of now, the parser to process game data is complete, 
along with the building blocks of the model architecture. 
After I complete the architecture itself, 
I'll train the model on the computer players developed in the Tribes research paper, 
and then try self or multi-agent reinforcement learning like DeepMind did. 

Fun fact: Tribes is written in Java and I'm using Python for my AI. 
I use a web socket for them to communicate. 
I think I may have to create a message protocol for model training and testing, but 
I've made protocols like that before.