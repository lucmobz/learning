# Learning Repository

## C++

* `std::shared_ptr` is an anti-pattern: https://ddanilov.me/shared-ptr-is-evil/
  * A nice post describing how `std::shared_ptr`s that express shared ownership can cause problems more often than not. Discusses the allocation of the data and reference counter when creating
    a `std::shared_ptr`, cyclic referencing problems, `std::weak_ptr` usage to break such cycles, and related problems to cases where deallocations of the blocks never happen

## Git/Github

* Cloning large repositories in a light way: https://github.blog/open-source/git/get-up-to-speed-with-partial-clone-and-shallow-clone/
  * Discusses how to use `git clone --depth=1 --no-single-branch -b <branch> <url>` and `git clone --filter=blob:none <url>` to clone large repository without getting all the files  
