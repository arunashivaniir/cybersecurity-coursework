# Algorithm for file updates in Python

## Project description

This project automates the process of updating an IP allow list stored in `allow_list.txt`. A Python script reads the file, removes IP addresses listed in a `remove_list`, and saves the updated list back to the file. This ensures efficient and accurate access control management.

## Open the file that contains the allow list

import\_file \= "allow\_list.txt"  
with open(import\_file, "r") as file:  
    ip\_addresses \= file.read()

**Explanation**:

* `import_file = "allow_list.txt"`: Assigns the filename to a variable.

* `with open(..., "r") as file`: Opens the file in **read mode** (`"r"`) using a `with` statement, which ensures the file is automatically closed after use.

* `file`: Temporary variable to interact with the open file inside the block.

## Read the file contents

ip\_addresses \= file.read()

**Explanation**:

* `.read()` reads the entire content of the file as a single string and assigns it to `ip_addresses`.

## Convert the string into a list

ip\_addresses \= ip\_addresses.split()

### **Explanation :**

* `.split()` is a **string method** that splits a string into a **list of words or tokens**, using **whitespace as the default separator**.

## Iterate through the remove list

for ip in remove\_list:

**Explanation**:

* The `for` loop is used to go through each IP address in `remove_list`.

* `ip` is the loop variable that holds the current IP address in each iteration

## Remove IP addresses that are on the remove list

    if ip in ip\_addresses:  
        ip\_addresses.remove(ip)

**Explanation**:

* `if ip in ip_addresses:` checks if the current IP is in the list read from the file.

* `.remove(ip)` removes that IP address from the list if it exists.

## Update the file with the revised list of IP addresses 

ip\_addresses \= " ".join(ip\_addresses)  
with open(import\_file, "w") as file:  
    file.write(ip\_addresses)

**Explanation**:

* `" ".join(ip_addresses)` converts the updated list back to a single string separated by spaces.

* `open(..., "w")` opens the file in write mode, which replaces the old content with the updated string

## Summary

* Opened the file containing the allow list.

* Read and convert the IP addresses to a list for easier manipulation.

* Iterated through a list of disallowed IPs and removed them.

* Saved the cleaned list back into the file.

* Used functions and file operations to automate allow list updates.

