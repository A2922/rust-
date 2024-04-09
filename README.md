TASK 1 - Getting a list of installed browsers

This Rust code checks for installed browsers in specified directories and prints the list of installed browsers if any are found, or a message indicating none were found.

ON this line we have to specify our target location 
let program_files_dirs = vec![
        "C:\\Program Files\\Google\\Chrome\\Application",.
		OUTPUT - Chrome is installed
  
--------------------------------------------------------------------------------------------------------------------------------------------------------------------
  
  
TASK 2 -Getting/calculating sha256 hash of a file, provided file path as input string
 This Rust code calculates the SHA256 hash of a file located at E:\codeA\example.txt and prints the hash in hexadecimal format. It does this by reading the file in 
 chunks and updating a SHA256 hasher instance.

 In  cargo.toml we have used 
  sha2 = "0.10.8"
 
  ON this lines we have to specify our file whose sha256 we need
  let file_path = "E:\\codeA\\example.txt";
  output - SHA256 hash of E:\codeA\example.txt is: 677dfc059984ba8a108c51e96a1920c93532d2a30be5987c11fc42292a8c98cd

  ------------------------------------------------------------------------------------------------------------------------------------------------------------------

 TASK 3 - Getting mark of the web for a file, provided file path as input string
   This Rust code adds a "Mark of the Web" comment to the beginning of a file's content, which is used by Windows to mark files that are downloaded from the 
  internet. It reads the content of a file, adds the comment, and then writes the modified content back to the file.

  OUTPUT - Mark of the Web added successfully.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
TASK 4 - Reading the preferences of all profiles for Google Chrome. 

This Rust code reads Chrome user preferences for all profiles in a directory, parses them as JSON, and saves them in a TOML file.

In cargo.toml we have used
toml = "0.8.12" 
dirs = "5.0.1"
serde_json = "1.0"
OUTPUT - Preferences written to chrome_preferences.toml

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
TASK 5 - Getting list of current network connections without using netsh (high bar).

This Rust code uses the netstat2 crate to fetch and print detailed information about TCP and UDP sockets, including local and remote addresses, ports, and associated process IDs.

In cargo.toml we have used 
netstat2 = "0.9"
listeners = "0.2.0"
winapi = { version = "0.3", features = ["winsock2"] }

OUTPUT - TCP 127.0.2.2:53 -> 0.0.0.0:0 [4484] - LISTEN
TCP 127.0.2.3:53 -> 0.0.0.0:0 [4484] - LISTEN
TCP 172.16.0.2:49377 -> 2.18.40.153:443 [11444] - CLOSE_WAIT
TCP 172.16.0.2:49378 -> 2.18.40.153:443 [11444] - CLOSE_WAIT
TCP 172.16.0.2:49381 -> 2.18.40.144:443 [11444] - CLOSE_WAIT
TCP 172.16.0.2:49382 -> 2.18.40.144:443 [11444] - CLOSE_WAIT
TCP 172.16.0.2:49383 -> 2.18.40.144:443 [11444] - CLOSE_WAIT
TCP 172.16.0.2:49384 -> 2.18.40.144:443 [11444] - CLOSE_WAIT
TCP 172.16.0.2:49385 -> 2.18.40.144:443 [11444] - CLOSE_WAIT
TCP 172.16.0.2:49386 -> 2.18.40.144:443 [11444] - CLOSE_WAIT
TCP 172.16.0.2:49393 -> 136.143.191.144:443 [4400] - ESTABLISHED

TCP 127.0.0.1:49680 -> 127.0.0.1:49681 [6532] - ESTABLISHED
TCP 127.0.0.1:49681 -> 127.0.0.1:49680 [6532] - ESTABLISHED
TCP 127.0.0.1:49682 -> 127.0.0.1:49683 [6532] - ESTABLISHED
TCP 127.0.0.1:49683 -> 127.0.0.1:49682 [6532] - ESTABLISHED
TCP 0.0.0.0:49684 -> 0.0.0.0:0 [916] - LISTEN

TCP 172.16.0.2:49828 -> 34.120.231.152:443 [0] - TIME_WAIT
TCP 172.16.0.2:49829 -> 34.120.231.152:443 [0] - TIME_WAIT
TCP 172.16.0.2:49833 -> 13.107.5.93:443 [0] - TIME_WAIT
TCP 172.16.0.2:49834 -> 34.120.231.152:443 [0] - TIME_WAIT
TCP 172.16.0.2:49838 -> 18.161.111.8:443 [4400] - ESTABLISHED
TCP 172.16.0.2:49840 -> 3.160.196.8:443 [4400] - ESTABLISHED
TCP 172.16.0.2:49843 -> 3.160.196.8:443 [4400] - ESTABLISHED
TCP 172.16.0.2:49846 -> 18.161.111.127:443 [5964] - ESTABLISHED
TCP 172.16.0.2:49849 -> 104.18.37.228:443 [4400] - ESTABLISHED
TCP 172.16.0.2:49850 -> 18.204.113.19:443 [7352] - ESTABLISHED
TCP 172.16.0.2:49851 -> 104.18.37.228:443 [4400] - ESTABLISHED
TCP 172.16.0.2:49852 -> 18.204.113.19:443 [7352] - CLOSE_WAIT
TCP 172.16.0.2:49868 -> 34.120.231.152:443 [0] - TIME_WAIT
TCP 172.16.0.2:49869 -> 34.120.231.152:443 [0] - TIME_WAIT

UDP 172.16.0.2:138 -> *:* [4]
UDP 192.168.1.9:138 -> *:* [4]
UDP 172.16.0.2:1900 -> *:* [3248]
UDP 192.168.1.9:1900 -> *:* [3248]
UDP 0.0.0.0:3702 -> *:* [2976]
UDP 0.0.0.0:3702 -> *:* [7268]
UDP 0.0.0.0:3702 -> *:* [2976]
UDP 0.0.0.0:3702 -> *:* [7268]

------------------------------------------------------------------------------------------------------------------------------------------------------------------
TASK 6 - Getting/calculating sha512 hash of a file, provided file path as input string


 This Rust code calculates the SHA512 hash of a file located at E:\codeA\example.txt and prints the hash in hexadecimal format. It does this by reading the file in 
 chunks and updating a SHA256 hasher instance.

 In  cargo.toml we have used 
  sha2 = "0.10.8"
 
  ON this lines we have to specify our file whose sha256 we need
  let file_path = "E:\\codeA\\example.txt";

  OUTPUT - 
  SHA512 hash of E:\codeA\example.txt is: ea62e6a0c30c9750f79325ae78158967ef614a8b15489c4f6c8a4c187b7f6a7d2132aead3172d5a691bd4a92e9947568d123038a87a22748270e28bbc3bb8549

------------------------------------------------------------------------------------------------------------------------------------------------------------------
Task 7 - ⁠Performing WiFi scan and returning the results without using netsh (high bar)
This Rust code uses subprocesses to extract and display saved WiFi profiles and passwords on Windows.

In Cargo.toml we have used 
subprocess = "0.2"
regex = "1.6"
itertools = "0.12.1"
lazy_static = "1.4"

OUTPUT - Loading all WiFis saved on computer...
Loading passwords...

        1. 2922: "1111"
        2. 2922 2: "111001111"
        3. AndroidAP: "Ar15u123"     
        4. Aniket: "An1528t123"       
        5. Ankit: "98758746321"        
        6. Arvind Sharma: "1010101010"
        7. Arvind's Galaxy F23 5G: ""
        8. BAJA: "Baja@2023#"
        9. BOSE: "B159876324"









  
  
