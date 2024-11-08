VUE framework system has logical defects and vulnerabilities
Vulnerability description:
Vue.js is a progressive framework for building user interfaces A JavaScript framework used to build user interfaces. As one of the three dominant front-end frameworks (Vue, React, Angular), it is built on standard HTML, CSS, and JavaScript, and provides a declarative, component-based programming model to help you efficiently develop user interfaces.
The VUE framework system has a logical vulnerability that attackers can exploit to bypass system authentication and log in to any account.
It can be seen that the versions involved are both 2.6. x and 2.7. x
VUE official website:
![image](https://github.com/bluewuyan/11vue/blob/main/photo/1.png)
https://cn.vuejs.org/
Fofa syntax: JS page prompts for filtering VUE framework icons and VUE framework BODY attributes
(icon_hash="-1252041730" || icon_hash="1917028407") && body="Please enable it to continue"
2. Reproduce the process
Reproduce IP1: https://goatmanagementsystem.cn/#/login
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu1.png)
You can use the shortcut key: ctrl+u to view the page source code, 
and check the/js/chunk vendors. xxxxxx. js file to see the Vue framework version.
Use BURP to capture login packages, right-click on the burst and select the DO intercept option.
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu12.png)

![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu13.png)
Change the code to 200.
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu14.png)
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu15.png)
IP2：http://139.196.103.136/
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu21.png)
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu22.png)
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu23.png)

Capture the request packet and intercept the return packet to modify the code to 200.
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu24.png)
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu25.png)
IP3：http://110.42.244.253/
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu31.png)
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu32.png)
Capture the request packet and intercept the return packet to modify the code to 200.
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu33.png)
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu34.png)
IP4：http://101.37.13.227
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu41.png)
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu42.png)
Capture the request packet and intercept the return packet to modify the code to 200.
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu43.png)
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu44.png)
IP5:http://43.228.77.13:20002
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu51.png)
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu52.png)
We need to change both the code and state to 200 here.
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu53.png)
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu54.png)


IP6：http://47.103.199.200/
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu61.png)
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu62.png)
Capture the request packet and intercept the return packet to modify the code to 200.
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu63.png)
![image](https://github.com/bluewuyan/11vue/blob/main/photo/fu64.png)
