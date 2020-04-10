# opener
### Fetch many paths for many hosts 
#### Inspired by: https://github.com/tomnomnom/meg

## Install
* `$ sudo apt install python3`
* `$ sudo apt install python3-pip`
* `$ sudo pip3 install requests requests_toolbelt`

```
 ___             ___     
|   |___ ___ ___|_  |___ 
| | | . | -_|   |_  |  _|
|___|  _|___|_|_|___|_|  
    |_|                  

# Coded By : Khaled Nassar @knassar702

Options:
	-h,--help              | Show help message and exit
	-r,--allow-redirect    | Allow the main redirect
	-p,--path              | The Path (default /)
	-m,--method            | Http method (default GET)
	-n,--number            | Number of response (Ex : 200)
	-o,--output            | Name of results file
	--threads              | Max number of concurrent HTTP(s) requests (default 10)
	--timeout              | Seconds to wait before timeout connection (default 3)
Examples:
	$ cat live_domains.txt | python3 open3r 
	$ cat live_domains.txt | python3 open3r --threads=100 -p /robots.txt -m get
	$ cat live_domains.txt | python3 open3r --threads=100 -p /login -m post
	$ cat live_domains.txt | python3 open3r --timeout=50 -p /login -m get -n 200,302
	$ cat live_domains.txt | python3 open3r -p /phpinfo.php -o phpinfo_websites -n 200

```
