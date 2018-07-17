# hybbon-bootstrap-node
An initial bootstrap node for P2P network.


# How to run?


### 1. Clone a repository to build jars or use builds at bootstrap-builds/ folder.
```
git clone https://github.com/viogull/hybbon-bootstrap-node.git
```
### 2. Firstly, edit an config at bootstrap-builds/boot/settings.conf
    Specify port, domain and relay configurations.
```
Bootstrap.port = 4662 // port must be opened
Bootstrap.address = localhost //specify domain here
Bootstrap.enabled = true
AcceptData = true
NumPeers = 50
ExternalAddress = "" // specify IP address if domain exists
Relay
  {
    enabled = true // disable it 
    GCM {
      api-key = ""
      buffer-age-limit = 20
    }
  }
```
###  3. Then run script by command:
  ```
  sh run.sh
```
