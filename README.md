# bukkenoh_manual_setup

__THIS IS FOR BUKKENOH TEAM ONLY!__<br>

__https://bukkenoh.backlog.com/git/SITE__

__REQUIREMENTS:__<br>
__- This is for proto ver 4__<br>
proto4.bukken1-web.xyz

1. PHP 8.1.x || 8.2.6
2. Node 8.16.0 || 8.15.0
3. Composer 2.x.x || 2.5.8

__- This is for proto ver 3__<br>
proto3.bukken1-web.xyz
1. PHP 7.4.x || 7.4.10

__- This is for proto ver 2__<br>
proto2.bukken1-web.xyz<br>
firstwith.jp
1. PHP 7.2.x || 7.2.19

__- This is for proto ver 1__<br>
proto.bukken1-web.xyz

__WHEN STARTING CODING__<br> 
1. Open the "Git Bash" and input __`cd c:laragon/www`__
2. Inside the "www" input __`git clone https://bukkenoh.backlog.com/git/SITE/proto4.bukken1-web.xyz.git`__
3. Go to the root folder of the project<br> ![image info](./setup_root_folder.jpg)
4. Copy and paste the ".htaccess" file<br>
5. Go to the "laravel" folder of the project<br> ![image info](./img_setup_bukkenoh_env.jpg)
6. Copy and paste the ".env" file<br>
7. Open the "Visual Studio Code" and make sure you're in your branch
8. Edit the ".env" file and save all the file edited
```diff

// default
- USER_ID = 43
- STORE_ID = 124

+ ROOT_URL = http://local.proto4.bukken1-web.xyz/

// can be found in the project wiki
+ USER_ID = 43
+ STORE_ID = 88

```
9. Go to your terminal and make sure you're in the root and in your branch<br>
10. Input __`cd laravel`__ and install composer __`composer install`__<br>
11. Create a new terminal and in you root input this __`cd src`__ and install yarn __`install yarn`__<br>
12. Inside the src folder input __`yarn watch`__
13. You're almost there! Make sure you start the laragon and go to your local, example "http://proto4.bukken1-web.xyz.test/"<br>
14. "Empty Cache and Hard Reload" your local after you load this "http://proto4.bukken1-web.xyz.test/cmd/makecache"<br>
15. The '0' will display

## NOTES!!!
This is for the older prototype.<br>
Requirements:
1. PHP 7.2.Xv || v7.2.19
2. Node 8.16.0 || v8.15.0
3. Composer 1.9.X || v1.9.3

__OLDEST PROTOTYPE__<br>
if it's still not working after "/cmd/makecache"<br>
go to "ArrayInput.php" this can be found here<br>
![image info](./img_setup_bukkenoh_arrayinput.jpg)
```diff

// default
- } elseif ('-' === $key[0]) {

// add this
+ } elseif (0 === strpos($key, '-')) {

```

__OTHERS!__<br>
__`yarn watch --project sp`__ oldest prototype when there's sp folder<br>
__`yarn build`__ or __`yarn rebuild`__<br>
__`yarn iconfont`__

__OUTSIDE NOTES HERE!__<br>
JP: https://github.com/hiloki/flocss<br>
EN: https://github.com/hiloki/flocss/blob/master/README_eng.md<br>
https://bukkenking.notepm.jp/



