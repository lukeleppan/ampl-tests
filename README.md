# AMPL Testing Scripts

## Repository Structure

The test scripts should be placed along side the `src/` directory of the `AMPL` compiler.

Follow the directory structure below:
```
ampl/
    src/
        test{module}.c
        {requirements}.c
        {requirements}.h
        Makefile
    test/
        test.py
        tests/
            0.ampl
            ...
        {module}/
            0.out
            ...
    bin/
        test{module}
```

## Scripts

### Running Tests

The `test.py` script will run the tests, see:
```bash
python3 test.py --help
```
for more info.

### Saving tests to module directory

The `save_tests.sh` script saves the executed code to the module direcory, effectively overwriting the "expected out".


