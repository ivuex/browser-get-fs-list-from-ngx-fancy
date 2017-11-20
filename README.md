# browser-get-fs-list-from-ngx-fancy

## What can this demo do? 
- Times ago, send files and directories list info to client, at least require a ohter script,
	such as nodejs, java, php, python ...
- In this way, we can make browser get the list,
 which contains the file and directories in special absolute path; 

## what are the advantages?
- Other script require some memery using, many team like ours team cannot work without nginx;
- Most of Other language is a little inefficient than nginx;

## How does this idea work?
- copy fancy-index.conf and index.conf to your nginx virtaul host configuire directory,
  which usually is /etc/nginx/conf.d/;
- Make sure your nginx main configure file (usually is /etc/nginx.conf) include above two configure file, 
- Run code in shell, like below:
```
 cd /your/nginx/virtual/host/directory;
 nginx -t; //检查配置文件语法
 sudo service nginx reload; // or sudo service nginx restart;
```
- If some error output to you, you can read Notice section in this readme document;
- If still not work for you, you can check it and fix it, via checking, thinking, baidu, google ...
- Of cause, You can send mail to me: ivuex@yahoo.com,
- and you can enhance this demo, and push requests to me, If you want.

## Notice:

  > Suppose that your are going to make browser client get the files and directories list infomation of ${yourDir};
  > ${yourDir} must be absolute path in nginx configure.
  >
  > Make sure the index dcocument (followed in next line,
   after index directive.) cannot be resolve directly in ${yourDir};
  


	
	
