# cli-python
This is a sample CLI tools

Here is the sample code: 

```
import argparse
welcome = "Practicing CLI"
parser = argparse.ArgumentParser(description=welcome)
parser.add_argument('--domain', '-d', required=True, help='please add your domain name')
parser.add_argument('--ofile', '-o', help='define output file to save results of stdout. i.e. "output.txt"')
parser.add_argument('--lines', '-l', help='number of lines of output to print to the console"', type=int)
args = parser.parse_args()

domain = args.domain
ofile = args.ofile
lines = args.lines

print('domain: ', domain)
print('output file: ', ofile)
print('lines: ', lines)
```
