# uDork - Google Hacking Tool
### New functional version: v.3.0

###### Author: M3n0sD0n4ld
###### Twitter: [@David_Uton](https://twitter.com/David_Uton)

# Description:

uDork é um script escrito em Bash Scripting que usa técnicas avançadas de pesquisa do Google para obter informações confidenciais em arquivos ou diretórios, encontrar dispositivos IoT, detectar versões de aplicativos da Web e assim por diante.

O uDork NÃO faz ataques contra nenhum servidor, ele usa apenas dorks predefinidos e/ou listas oficiais do exploit-db.com (Google Hacking Database:https://www.exploit-db.com/google-hacking-database).

# Download and install:
```
$ git clone https://github.com/m3n0sd0n4ld/uDork
$ cd uDork
$ chmod +x uDork.sh
- Open the file "uDork.sh" and write inside this line:
```
![Screenshot](https://github.com/m3n0sd0n4ld/uDork/blob/master/images/1.png)
```
$ ./uDork.sh -h
```

## Steps to obtain the cookie and configure the cookie
1. Login to facebook.com
2. Now we will access www.messenger.com (It is the Facebook messaging app) and click on the "Continue as..." button.
![Screenshot](https://github.com/m3n0sd0n4ld/uDork/blob/master/images/2.png)
3. Once we're in, all we have to do is get the two cookies we need to make uDork work.

### 3.1 - With firefox:
-- Right mouse button and click on "Inspect".
<br>
![Screenshot](https://github.com/m3n0sd0n4ld/uDork/blob/master/images/3.png)
<br>
-- Click on the "Network" tab and select any line that is in the domain "www.messenger.com".
<br>
-- Now click on the "Cookies" tab, copy and paste the cookies "c_user" and "xs" into the "uDork.sh" file.
<br>
![Screenshot](https://github.com/m3n0sd0n4ld/uDork/blob/master/images/4.png)
<br>
Thus: cookies="c_user=XXXXXX; xs=XXXXXX;"
<br>
<br>
![Screenshot](https://github.com/m3n0sd0n4ld/uDork/blob/master/images/1.png)
<br>

### 3.2 - With Google Chrome
-- Right mouse button and click on "Inspect".
<br>
![Screenshot](https://github.com/m3n0sd0n4ld/uDork/blob/master/images/5.png)
<br>
--  Click on the tab "Application", in the left column, look for the section "Cookies", copy and paste the cookies "c_user" and "xs" with their value to the file "uDork.sh".
<br>
![Screenshot](https://github.com/m3n0sd0n4ld/uDork/blob/master/images/6.png)
<br>
Thus: cookies="c_user=XXXXXX; xs=XXXXXX;"
<br>
![Screenshot](https://github.com/m3n0sd0n4ld/uDork/blob/master/images/1.png)
<br>

# Docker version:
## Acknowledgement
Twitter: [@interh4ck](https://twitter.com/interh4ck)
GitHub:(https://github.com/interhack86)
```
$ git clone https://github.com/m3n0sd0n4ld/uDork
$ cd uDork
$ docker build -t udork .
$ docker run --rm -it -e c_user=XXXXXXXXX -e xs=XXXXXXXXX udork -h
```

# Use:

## Menu
![Screenshot](https://github.com/m3n0sd0n4ld/uDork/blob/master/images/7.png)

## Example of searching pdf files
![Screenshot](https://github.com/m3n0sd0n4ld/uDork/blob/master/images/8.png)

## Example of a search for a list of default extensions.
![Screenshot](https://github.com/m3n0sd0n4ld/uDork/blob/master/images/12.png)
![Screenshot](https://github.com/m3n0sd0n4ld/uDork/blob/master/images/13.png)

## Example of searching routes with the word "password"
![Screenshot](https://github.com/m3n0sd0n4ld/uDork/blob/master/images/9.png)

## Dorks listing
![Screenshot](https://github.com/m3n0sd0n4ld/uDork/blob/master/images/10.png)

## Example of use Dorks Massive 
![Screenshot](https://github.com/m3n0sd0n4ld/uDork/blob/master/images/11.png)

## Example of use All Dorks Massive (Recommend for pentesting/audit) 
![Screenshot](https://github.com/m3n0sd0n4ld/uDork/blob/master/images/14.png)
![Screenshot](https://github.com/m3n0sd0n4ld/uDork/blob/master/images/15.png)


# Disclaimer
This tool requires session cookies from a Facebook account to work. I am NOT responsible for any problems with your account and/or computer.
