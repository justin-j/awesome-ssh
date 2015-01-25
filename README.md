# awesome-ssh
Simple ssh setup for Mac and AWS

### setup ssh folder and server info in your home directory
create an .ssh folder if you don’t have it already
open terminal
```
cd ~
mkdir .ssh
```
create your config file
```
vi ~/.ssh/config
```
the three vi commands you will use are insert mode “i”, exit insert mode “esc”, and write quit “:wq”
insert your configuration (replace everything in brackets)
```
Host <alias for connecting>
User <username on the server>
HostName <host or public dns>
IdentityFile <path to your pem file>
```
### connect through ssh to your server
in terminal
```
ssh <Host>
```
