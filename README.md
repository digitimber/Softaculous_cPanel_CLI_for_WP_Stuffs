Created a little bash script to assist with command line interaction of deplying development sites within my cPanel /w Softaculous environment


Distributed as-is, no warranty, no guarantee, might make your dog run away and your milk sour

Usage: Create a .pw file in your user home directory with the following info:
```
CPW='cpanel_user_password'
WPPW='some_random_password_for_wp_admin_user'
```


Run:
```
./softcli
```
Output:
```
Please use ./softcli install <subdomain> to create the new site or
Please use ./softcli remove <inst_id> to remove an existing site or
Please use ./softcli otlogin <inst_id> to create a one time login for a site or
Please use ./softcli stage <inst_id> <subdomain> to create a staging site from an existing id on a new subdomain or
Please use ./softcli makelive <inst_id> to push a copy of staging to the live site it was created from or
Please use ./softcli list to list existing installations
```
