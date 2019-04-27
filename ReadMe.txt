
1. 将base64和jsEncrypt的js文件放到合适的地方方便引用（如:utils中）

2. 在需要编码的小程序页面js中引入上述两个文件
           const base64=require('../../utils/base64.js');
           const Encrypt=require('../../utils/jsEncrypt.js');
    具体使用：
        //rsa加密
        var PUBLIC_KEY=' ' //由后端提供
        var encrypt=new Encrypt();
        encrypt.setPublicKey(PUBLIC_KEY);
        password=encrypt.encrypt(password); //对password加密后再赋值给password
       
        //base64编码
        password=base64.encode(password)  //对已经加过密的password进行base64编码
   