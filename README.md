# pay

This script is for easily executing the curl command mainly targeted the Payment Gateways. 

### Environment
| Subject  | Object |
| ------------- | ------------- |
| OS  | Mac, Linux  |


### Usage

First you need to set up your host:
 
```
cd config
cp config.sample config
vim config
```

```
domain=https://moomin.com # this part should not end 
                          # with slash or something.
skey=skey_aaaaa_bbbb
```

Then install the **pay** script:

```
$ ./installer
```

For help menu:

```
$ pay -h
```

First you need to add a new manual
```
$ pay -n
```

They ask for the API so you should opt the target API.


Then **enlist** manuals:

```
pay -l
```

For playing manuals (actually executing **curl** command: 

```
$ pay -p
```

This can allow the script to interactively let you select the manual and execute it.

If you do not want to be bothered by manual selection interactive process, this can be skipped by:

```
pay -p [category] [manual] [optional:y]
```
If **y** is put directly as argument, there are no confirmation before the execution of curl command so there actually is no interactive part at all.

For the deletion of manual, you can type this way:

```
$ pay -d
```



### Contact
For any bug reports or any other contacts, please notice me directly:

email:    **tobasojyo@gmail.com**

twitter:  **@keisuganodev**