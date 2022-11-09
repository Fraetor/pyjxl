# pyJXL

A python JPEG XL decoder. It is currently *very* incomplete.

## Installation

I am aiming to make this decoder as portable as possible. As such it will
ideally have minimal dependencies outside of the standard library. I will use
NumPy, as image data maps nicely to a 2D array and it will give us the speed
necessary for any per pixel processing. I may also use a dependency for PNG
output, if I don't write one myself.

### Requirements

- Recent [Python 3](https://www.python.org/) (developed with 3.11, but may work with some older versions)
- [NumPy](https://numpy.org/) Can be installed with `pip install numpy`.

### Development Requirements

- [PyTest](https://docs.pytest.org/)

## Usage

We are a long way away from it, but this is how I intend the decoder to work
from the command line:

```sh
python3 pyjxl.py input_file.jxl [output_file.png]
```

## Roadmap/To Do

- [ ] Decide on internal representation of image data (NumPy array?)
- [ ] Define external interfaces by decoding PPM image.
- [ ] Decode JPEG images.
- [ ] PNG output of decoded images.
- [ ] Start on JPEG XL support.

<!-- ## Contributing

State if you are open to contributions and what your requirements are for
accepting them.

For people who want to make changes to your project, it's helpful to have some
documentation on how to get started. Perhaps there is a script that they should
run or some environment variables that they need to set. Make these steps
explicit. These instructions could also be useful to your future self.

You can also document commands to lint the code or run tests. These steps help
to ensure high code quality and reduce the likelihood that the changes
inadvertently break something. Having instructions for running tests is
especially helpful if it requires external setup, such as starting a Selenium
server for testing in a browser. -->

<!-- ## Acknowledgements

Show your appreciation to those who have contributed to the project. -->

## Licence

This software is available under the [MIT Licence](LICENCE).