# pygitloc

A package to calculate lines of code from a GitHub repository link.

## Installation

To install the package, use:

```bash
pip install pygitloc==0.5
```

## Usage

To calculate the lines of code from a GitHub repository, run:

```bash
pygitloc <github-link>
```

Replace `<github-link>` with the URL of the GitHub repository you want to analyze. For example:

```bash
pygitloc https://github.com/yourusername/your-repo
```

## Requirements

This package relies on the following dependencies:

- [GitPython](https://pypi.org/project/GitPython/)
- [PyGithub](https://pypi.org/project/PyGithub/)

## How It Works

1. The `pygitloc` command clones the specified GitHub repository to a temporary directory.
2. Finally, it calculates and outputs the results and cleans up the temporary directory.

## Example

```bash
$ pygitloc https://github.com/torvalds/linux
Cloned https://github.com/torvalds/linux to temp_repo
     1973 text files.
     1953 unique files.
      1824 files ignored.

github.com/shubhamshnd/cloc v 1.88  T=18.00 s (61.6 files/s, 5762.4 lines/s)
-------------------------------------------------------------------------------
Language                     files          blank        comment           code
-------------------------------------------------------------------------------
C                             1180         252635         329417        2046599
Assembly                       159          16646          27585         108099
C/C++ Header                   270          57480         152239          96316
...
-------------------------------------------------------------------------------

# Clean up
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request on GitHub.


## Acknowledgments

- [GitPython](https://github.com/gitpython-developers/GitPython)
- [PyGithub](https://github.com/PyGithub/PyGithub)

## Contact

For any questions or issues, please contact [shubhamshindesunil@gmail.com](mailto:shubhamshindesunil@gmail.com).
[My Linkedin](https://www.linkedin.com/in/shubham-shnd/)

