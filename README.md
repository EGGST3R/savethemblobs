# savethemblobs

A simple script to grab all SHSH blobs from Apple that it's currently signing to save them locally and on Cydia server.

And now also grabs blobs already cached on Cydia servers to save them locally.

Will automatically work with future firmwares!

## Dependencies

	Depends on Python 2.7 pip, and requests. 
	With pip installed, run:
		pip install requests
	

## Usage

	savethemblobs.py [-h] [--save-dir SAVE_DIR] [--overwrite]
	                 [--overwrite-apple] [--overwrite-cydia]
	                 [--no-submit-cydia] [--cydia-blobs]
	                 ecid device

	positional arguments:
	  ecid                 device ECID in int or hex (prefix hex with 0x)
	  device               device identifier/boardconfig (eg. iPhone3,1/n90ap)

	optional arguments:
	  -h, --help           show this help message and exit
	  --save-dir SAVE_DIR  local dir for saving blobs (default: ~/.shsh)
	  --overwrite          overwrite any existing blobs
	  --overwrite-apple    overwrite any existing blobs (only from Apple)
	  --overwrite-cydia    overwrite any existing blobs (only from Cydia)
	  --no-submit-cydia    don't submit blobs to Cydia server
	  --cydia-blobs        fetch blobs from Cydia server (32 bit devices only)


## License

savethemblobs is available under the MIT license. See the LICENSE file for more info.
