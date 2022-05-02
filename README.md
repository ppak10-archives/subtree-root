# subtree-root

## Getting Started
1. Clone this repository.

## Contributing to subtree
1. Create a new branch on this (`subtree-root`) repository for any changes.
2. You will need to push changes twice or more (Once to `subtree-root` and another to `subtree-child` and other subtrees)
    1. Commit and Push *All* Changes to `subtree-root` *First*.
    2. Push any subtree specific changes a new branch on a subtree (`subtree-child`) repository.
        - `git subtree --prefix=<folder_name> push <repository> <branch_name>`
        - `git subtree --prefix=subtree_child push https://github.com/ppak10/subtree-child.git enhancement/instructions`
          - This will push any changes under the `subtree_root/subtree_child` to the newly created `enhancement/instructions` branch in the `subtree_child` repository.

## Merging Changes
1. Aim to keep the branches between different repsitories in the same state.
    - (i.e. `subtree-root/subtree-child` == `subtree-child` for `main` branch.)
2. Merge changes in subtree child first, then merge changes in subtree root.
    - This should mitigate issues and merge conflicts between multiple developers.
    - Changes in `subtree-root/subtree-child` branch should be equal to `subtree-child` repo's `main` branch

## Possible Issues 
* Making changes directly to `main` branch in `subtree-child` repo would require a merge.
