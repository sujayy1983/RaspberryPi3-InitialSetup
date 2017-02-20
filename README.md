```
Description: Raspberry Pi3 quick setup

Author: Sujayyendhiren RS
```

```
 Step1: Basic edits to that ll get us started without much configuration
        (i) Edit hosts file as per your setup.
        (ii) Setup public private keypair and update ansible.cfg

 Step2: To setup OS image of our choice. The playbook is tested on MAC and this
lets us copy an OS image onto the SD card inserted into the MAC.

        Command:
          ansible-playbook -i hosts --tags jui rasp_os_deploy/deploy_os.yml 
                                or 
          ansible-playbook -i hosts --tags jlite rasp_os_deploy/deploy_os.yml 

 Step3: To clone practice code that gets you started with basic electronics.
          ansible-playbook -i hosts --tags init software_onpi/initial_setup.yml 

```
