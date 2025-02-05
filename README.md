# Disable NeuVector nvprotect
NeuVector 有一個名為 nvprotect 的內部保護機制，用來限制使用者對 NeuVector pod 的存取權限。

如果需要關閉，可以透過介面關閉，此處提供腳本，支援關閉 Controller、Scanner、Enforcer 的 nvprotect。

使用方法：
```
$ git clone https://github.com/cooloo9871/Disable-nvprotect.git
$ cd Disable-nvprotect
$ chmod +x disable-nvprotect.sh

# 關閉 nvprotect
# 關閉 enforcer 即可同時關閉 scanner 的 nvprotect
$ ./disable-nvprotect.sh off controller|enforcer

# 開啟 nvprotect
$ ./disable-nvprotect.sh on controller|enforcer
```
