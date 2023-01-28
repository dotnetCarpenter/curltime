# curltime

## Example output

```
$ curltime example.com

Stats for https://example.com/
        http version:  2
     time_namelookup:  0.005929s
        time_connect:  0.164036s
     time_appconnect:  0.442980s
    time_pretransfer:  0.443290s
       time_redirect:  0.000000s (0 redirects)
  time_starttransfer:  0.564174s
                     ----------
          time_total:  0.564367s
```


## Usage

`curltime` is the codification of an excellent answer on SO: https://stackoverflow.com/a/22625150/205696

```
Usage: ./curltime [--url http://subdomain.example.com | example.com]

curltime version 0.2.0

If --url is not used, the last argument will be prefixed with "https://"
and postfixed with "/".

The output is controlled by
./curl-format.txt
See https://everything.curl.dev/usingcurl/verbose/writeout#available-write-out-variables
for available variables.

Parameters:

	-h, --help	display this help and exit
	-u, --url	write raw URL directly to cURL
```


## Installation

```sh
git clone git@github.com:dotnetCarpenter/curltime.git
cd curltime

# for bash
echo "\nexport PATH="$PWD:\$PATH"" >> ~/.bashrc
# OR
echo "\nexport PATH="$PWD:\$PATH"" >> ~/.profile

# for zsh
echo "\nexport PATH="$PWD:\$PATH"" >> ~/.zsh
#OR
echo "\nexport PATH="$PWD:\$PATH"" >> ~/.zprofile
```

> _Personally, I always you the profile file for my custom stuff._


## CC BY-SA 4.0 License

[Attribution-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-sa/4.0/)

Which is the same license used by [stackoverflow.com](https://stackoverflow.com/legal/terms-of-service/public#licensing).
