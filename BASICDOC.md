# Documenting codebase changes

This is a space where I'll be documenting design decisions and the overall structure of the project, to make it a bit easier for other people to get to know (and hopefully give feedback on) my work.

In the first instance, the aim of this repository is to efficiently generate simulations over a 2D mesh of the self-organisatio behaviour of a continuous field of both ECM and cell density. A separate project may attempt to model the behaviour of individual cells, but this is of less importance as we'll be implicitly decentring cell movement to more closely mirror tissue behaviour in a non-embryonic setting (such as soft tissue distraction).

The primary theoretical aspects of the model are very well introduced in the paper "Mechanical aspects of mesenchymal morphogenesis" by Oster et al., and I'll be trying to progressively implement the more complex aspects of the model as I go. In an attempt to minimise developmental overhead, I will start by offloading all of the visualisation and graphing to python, so I can focus more on the mathematical/OOP considerations (as opposed to trying to grapple with OpenGL).

Because I have a decent amount of experience with reaction-diffusion, I'll implement a Crank-Nicolson Gray-Scott to begin with because I've done it in python.

There is no linear algebra in the C++ standard library?? Horrifying - have wrangled with Conan for about an hour now, and I think understand a bit more about CMake, have opted for Eigen because apparently its very performant according to a rando on stackexchange.


