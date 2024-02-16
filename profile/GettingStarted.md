# Getting Started

The WheelSims project is a set of blocks distributed on different repositories, that can be shared among wheelchair simulators to accelerate the development of virtual reality in wheelchair training.

Since `git` is already complex for newcomers, having multiple repositories is yet more complex. For this reason, we recommend to use a good GUI to stay up to date and ease collaborative development. In these README files, we make use of [SourceTree](https://www.sourcetreeapp.com/), a free `git` client for Mac and Windows.


## Toplevel repositories

Only the repositories that start by `sim` are toplevel repositories and are meant to be cloned. The others are submodules. Currently, we have:

- `sim_generic_vr` : A generic Unity project that contains every Unity element available for the simulators. Use this repository to develop virtual reality material that is not related to one given simulator.
- `sim_irglm_vr` : The IRGLM simulator. It contains every submodules of `sim_generic_vr`, but will also contain other elements such as Matlab/Simulink stuff for the electromechanical components.
- Others to come.

## Cloning a repository

To clone a repository locally with all its submodule, choose `New` → `Clone from URL` and fill these informations (change to the repository name you want to clone):

![image](https://github.com/WheelSims/sim_generic_vr/assets/34967663/d9d2e243-29f7-4dea-994a-e5b46fa4fef7)

Once cloned, the project looks like this in SourceTree. Note submodules pane: double-clicking on a submodule launches a new repository window for this specific repository.

![Screen Shot 2024-02-16 at 09 50 35](https://github.com/WheelSims/.github/assets/34967663/d60469de-92e6-4135-8061-1caa2177867d)

## Opening in Unity

- Launch Unity Hub and open the Unity subfolder of your local clone.
