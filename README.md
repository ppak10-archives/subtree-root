# subtree-root

## Getting Started
1. Clone this repository.

## Contributing to subtree
1. Create a new branch on this (`subtree-root`) repository for any changes.
2. Push any subtree related changes a new branch on a subtree (`subtree-child`) repository.
  - `git subtree --prefix=<folder_name> push <repository> <branch_name>`
  - `git subtree --prefix=subtree_child push https://github.com/ppak10/subtree-child.git enhancement/instructions`
    - This will push any changes under the `subtree_root/subtree_child` to the newly created `enhancement/instructions` branch in the `subtree_child` repository.
