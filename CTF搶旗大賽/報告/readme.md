## 本學期報告
- [期中報告:使用pycrypto實作現代密碼學(30%)](#期中報告)
- [平時報告:使用openssl實作現代密碼學(30%)](#平時報告)
- [期末報告:現代密碼學之破密分析實測(0%)](#期末報告)


## 期中報告

- 標題:使用pycrypto實作現代密碼學

- 現代密碼學
  - 非對稱式(公開)金鑰系統加解密: 
    - RSA
    - ELGAMAL
    - ECC
  - 對稱式金鑰系統加解密
    - DES
    - 3DES
    - AES 
  - Hash
    - MD5
    - SHA,.... 
- python現代密碼模組:
  - Python Cryptography Toolkit (pycrypto)
  - PyCryptodome
  - cryptography 
- python現代密碼模組:pycrypto
  - 模組架構
    - Crypto.Hash: Hash Functions
    - Crypto.Cipher: Encryption Algorithm
    - Crypto.Protocol: Various Protocols
    - Crypto.PublicKey: Public-Key Algorithms
    - Crypto.Util: Odds and Ends
      - Crypto.Util.number 
- pycrypto現代密碼模實作
  - 非對稱式(公開)金鑰系統加解密實作
    - RSA
    - ELGAMAL
    - ECC 
  - 對稱式金鑰系統加解密實作
    - DES
    - 3DES
    - AES
  - Hash實作
    - MD5
    - SHA1
    - SHA2
    - SHA512

## 平時報告

- 標題:使用openssl實作現代密碼學

- 現代密碼學
  - 非對稱式(公開)金鑰系統加解密: 
    - RSA
    - ELGAMAL
    - ECC
  - 對稱式金鑰系統加解密
    - DES
    - 3DES
    - AES 
  - Hash
    - MD5
    - SHA,.... 
- openssl現代密碼模組:
  - openssl
  - 使用模式
    - 將openssl當作指令執行
    - 使用c++呼叫 openssl ==> 高手才用 C語言：Windows C/C++ 加密解密實戰(朱晨冰、李建英)
  - https
    - nmap nse 測支援https ssl1-3(嚴重錯誤)  TLS1.1-1.2(錯誤) TLS1.3
  - openssl CVE 
    - https://hub.docker.com/r/hmlio/vaas-cve-2014-0160/ 
  - openssl原始碼分析 
- python現代密碼模組:openssl
  - 非對稱式(公開)金鑰系統加解密實作
  - 對稱式金鑰系統加解密實作
  - Hash實作

### openssl
- OpenSSL是一個開放原始碼的軟體函式庫套件
- 兩大類型用法: (1)使用命令列來加解密  (2)使用c/c++來呼叫openssl函示庫
- 應用程式可以使用這個套件來進行安全通訊，避免竊聽，同時確認另一端連線者的身分。
- http + SSL/TLS(openssl) = HTTPs ==> 這個套件廣泛被應用在網際網路的網頁伺服器上。


## 期末報告

-標題:現代密碼學之破密分析實測

- 破密分析常用工具
  - 質因數分解:
    - http://factordb.com/
  - libnum 套件 
  - mod-inverse 計算
    - sympy
    - gmpy2

- 非對稱式(公開)金鑰系統之破密分析: RSA,
  - 小n的攻擊
  - 孿生子的攻擊
  -  

- 對稱式金鑰系統之破密分析

- Hash之破密分析
