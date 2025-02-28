# Learning Repository

## C++

* `std::shared_ptr` is an anti-pattern: https://ddanilov.me/shared-ptr-is-evil/
  * A nice post describing how `std::shared_ptr`s that express shared ownership can cause problems more often than not. Discusses the allocation of the data and reference counter when creating
    a `std::shared_ptr`, cyclic referencing problems, `std::weak_ptr` usage to break such cycles, and related problems to cases where deallocations of the blocks never happen

## Git/Github

* Cloning large repositories in a light way: https://github.blog/open-source/git/get-up-to-speed-with-partial-clone-and-shallow-clone/
  * Discusses how to use `git clone --depth=1 --no-single-branch -b <branch> <url>` and `git clone --filter=blob:none <url>` to clone large repository without getting all the files  

## GoogleTest and CMake

* Test C code with GoogleTest and CMake:
  * https://notes.eatonphil.com/unit-testing-c-code-with-gtest.html
    * Discusses a way to test C code with tests written in C++ with googletest  
  * https://github.com/cpp-for-yourself/lectures-and-homeworks/blob/main/lectures/googletest.md
    * Another similar approach with small differences 

## Visual Studio 2022 Debugger Pretty Printing

* Use `.natvis` files in CMake project root folders to allow for custom visualization of variables when debugging: https://learn.microsoft.com/en-us/visualstudio/debugger/create-custom-views-of-native-objects?view=vs-2022
