
1. ��base64��jsEncrypt��js�ļ��ŵ����ʵĵط��������ã���:utils�У�

2. ����Ҫ�����С����ҳ��js���������������ļ�
           const base64=require('../../utils/base64.js');
           const Encrypt=require('../../utils/jsEncrypt.js');
    ����ʹ�ã�
        //rsa����
        var PUBLIC_KEY=' ' //�ɺ���ṩ
        var encrypt=new Encrypt();
        encrypt.setPublicKey(PUBLIC_KEY);
        password=encrypt.encrypt(password); //��password���ܺ��ٸ�ֵ��password
       
        //base64����
        password=base64.encode(password)  //���Ѿ��ӹ��ܵ�password����base64����
   