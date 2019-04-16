# Sagemath-Rotor-Graph
Rotor Graph library for Sagemath

## How to use

### If using the Sagemath git repository

#### 1 - Install Sagemath
In order to use the library, you must first install Sagemath from its source code and build it.
All instructions to do so can be found here: http://doc.sagemath.org/html/en/installation/source.html

#### 2 - Create a local branch

This part is optional. You can use the Rotor Graph library on any branch you want but make sure not to push the files on the Sagemath repo.

Once Sagemath is installed, create a local branch in the Sagemath git repository using

```
$ git branch sagemath_rotor_graph
```

Checkout that branch

```
$ git checkout sagemath_rotor_graph
```

#### 3 - Adding the Rotor Graph library as a submodule

The point is to keep this branch local to not pollute Sagemath.
On this branch you can create a git submodule (https://git-scm.com/docs/git-submodule) to this repo.
Assuming your Sagemath repository is in the `sage` directory:

```
sage $ git submodule add https://github.com/XanX3601/Sagemath-Rotor-Graph.git src/sage/rotors
```

This will create a `rotors` directory inside the Sagemath sources that contains the Rotor Graph library.
The changes should be ready to be committed (view with `git status`).

You can rebuild Sagemath using

```
sage $ ./sage -br
```

You can now use the library and update its branch by merging the master into it when you feel like it.

### If you have downloaded Sagemath source code

Assuming your Sagemath code is in the `sage` directory

```
sage $ cd src/sage
sage/src/sage $ git clone https://github.com/XanX3601/Sagemath-Rotor-Graph.git rotors
```

This will add the Rotor Graph library

You can rebuild Sagemath using

```
sage $ ./sage -br
```

You can now use the library.
