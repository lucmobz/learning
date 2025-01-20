# Learning Repository

## C++
### Blogs
* `std::shared_ptr` is an anti-pattern: https://ddanilov.me/shared-ptr-is-evil/
  * A nice post describing how `std::shared_ptr`s that express shared ownership can cause problems more often than not. Discusses the allocation of the data and reference counter when creating a `std::shared_ptr`, cyclic referencing problems, `std::weak_ptr` usage to break such cycles, and related problems to cases where deallocations of the blocks never happen
