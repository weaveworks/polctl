# Testing Policies

## test_policies

The `test_policies` binary will go over a polices directory structure and run all the tests. If a policy does not have test cases it will be ignored.

### How to run

The availble command are: 

```bash
NAME:
   policies test - Test policy policy code

USAGE:
   test_policies [global options] command [command options] [arguments...]

VERSION:
   0.0.1

COMMANDS:
   help, h  Shows a list of commands or help for one command

GLOBAL OPTIONS:
   --root-dir value       Root directory containing all policy directories
   --policy-path value    path to policy dir
   --help, -h             show help (default: false)
   --version, -v          print the version (default: false)
```

To run against a single policy:

```bash
./test_policies --policy-path <policy-path>
```

To run against multiple policies:

```bash
./test_policies --root-dir <root-dir>
```
