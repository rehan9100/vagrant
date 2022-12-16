Be sure that you are in the same directory as the Vagrantfile when running these commands!

## Creating a VM

```console
$ vagrant init        
$ vagrant init <boxpath>
$ vagrant init bento/ubuntu-20.04
```

## Starting a VM

```console
$ vagrant up      
$ vagrant resume           
$ vagrant provision           
$ vagrant reload              
$ vagrant reload --provision
```

## Getting into a VM
```console
$ vagrant ssh 
$ vagrant ssh <boxname>
```

## Stopping a VM
```
$ vagrant halt    
$ vagrant suspend
```

## Cleaning Up a VM
```console
$ vagrant destroy   
$ vagrant destroy -f
```

## Boxes
```console
$ vagrant box list        
$ vagrant box add <name> <url>
$ vagrant box outdated
$ vagrant box remove <name>
$ vagrant package
```
## Saving Progress
```console
$vagrant snapshot save [options] [vm-name] <name>`
```

## Tips
```console
$ vagrant -v                    
$ vagrant status                
$ vagrant global-status         
$ vagrant global-status --prune 
$ vagrant provision --debug  
$ vagrant push    
$ vagrant up --provision | tee provision.log
```
## Notes
- If you are using VVV, you can enable xdebug by running `vagrant ssh` and then `xdebug_on` from the virtual machine's CLI.
