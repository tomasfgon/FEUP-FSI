# LogBook10

## SEED Labs – XSS Lab

### Task 1

To post a malicious message to display an alert window when opening a specific
profile page, we ran the following HTML script:

![Task 1](images/seedlabs-web/task1-1.PNG)

On the edit profile page, we start by finding the user ID (GUID), so we can
choose whose profile we want to target on our script. The script can be
injected on the "About Me" section of the edit profile page.

As a result, whenever an user opens this profile page, the following alert
window will pop-up.

![Task 1 Result](images/seedlabs-web/task1-2.PNG)

### Task 2

To post a malicious message to display cookies, the logic is the same. We
simply need to change our script so that, instead of returning an alert
windows, it prints the cookies.

![Task 2](images/seedlabs-web/task2-1.PNG)

As a result, whenever an user opens this profile page, the current user's
cookies will be displayed.

![Task 2 Result](images/seedlabs-web/task2-2.PNG)

### Task 3

To steal cookies from the victim’s machine, we changed the script again. This
time a get request is sent to an address we control, containing said cookies

1. Injecting malicious script:

![Task 3](images/seedlabs-web/task3-1.PNG)

2. Setting up netcat listener:

![Task 3](images/seedlabs-web/task3-2.PNG)

3. Accessing Samy's profile with the malicious code:

![Task 3](images/seedlabs-web/task3-3.PNG)

4. Request received with cookies:

![Task 3](images/seedlabs-web/task3-4.PNG)

### Task 4

To become the victim’s friend we need to know the format of the add friend request.
The network tab on the browser's developer tools gives us that information.

![Task 4](images/seedlabs-web/task4-1.PNG)

1. Injecting add friend script that uses the visitor's cookies:

![Task 4](images/seedlabs-web/task4-2.PNG)

2. Alice's profile before visiting Samy's profile:

![Task 4](images/seedlabs-web/task4-3.PNG)

3. Alice's visiting Samy's profile (we can see in the developer tools a request
   has been sent):

![Task 4](images/seedlabs-web/alice_visit_samy_profile.png)

4. Alice's profile after visiting Samy's profile:

![Task 4](images/seedlabs-web/task4-4.PNG)
